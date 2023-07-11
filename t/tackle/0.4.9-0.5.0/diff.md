# Comparing `tmp/tackle-0.4.9.tar.gz` & `tmp/tackle-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tackle-0.4.9.tar", last modified: Tue Dec 20 16:27:37 2022, max compression
+gzip compressed data, was "dist/tackle-0.5.0.tar", last modified: Tue Jul 11 17:59:01 2023, max compression
```

## Comparing `tackle-0.4.9.tar` & `tackle-0.5.0.tar`

### file list

```diff
@@ -1,920 +1,965 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-12-20 16:27:06.000000 tackle-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-20 16:27:06.000000 tackle-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2022-12-20 16:27:37.000000 tackle-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2022-12-20 16:27:06.000000 tackle-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2022-12-20 16:27:06.000000 tackle-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-20 16:27:37.000000 tackle-0.4.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4814 2022-12-20 16:27:06.000000 tackle-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    64360 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/collections/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/collections/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/hooks/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/hooks/distinct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/hooks/list_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/hooks/map_to_list_key_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/hooks/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/notes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/collections/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/tests/concatenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/tests/distinct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/tests/list-keys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/tests/sort-in-place.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/tests/sort-map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/collections/tests/test_provider_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/command/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/command/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/hooks/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/hooks/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/command/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/exit-ignore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/exit-long.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/exit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/interactive.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/list-dir.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/multi-line-cmd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/command/tests/test_provider_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/console/
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/console/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/hooks/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/hooks/prints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/hooks/table.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/console/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/markdown.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/pprint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/print.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/table_split.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/test_provider_console_print.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/console/tests/test_provider_console_rich.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/context/
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/.tackle.meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/context/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/append.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/hooks/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/context/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/append-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/append-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/append.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/delete.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/get.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/keys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/pop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/set.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/test_provider_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/update-2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/context/tests/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/datetime/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/datetime/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/datetime/hooks/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/datetime/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/datetime/tests/date_now.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/datetime/tests/test_provider_datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/environment/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/environment/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/environment/hooks/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/environment/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/environment/tests/envs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/environment/tests/test_provider_envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/hooks/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/hooks/zips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/tests/file/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/file/chmod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/file/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/file/remove.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/file/shred.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/file/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/file/test_provider_system_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/tests/zips/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/tests/zips/stuff/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/files/tests/zips/stuff/stuff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/stuff/stuff/motings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/stuff/things
--rw-r--r--   0 runner    (1001) docker     (123)      436 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/stuff.zip
--rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/test_provider_system_zips.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/unzip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/zip-dir.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/files/tests/zips/zip-file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/hooks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/hooks/file_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/hooks/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/hooks/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/hooks/update_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/file_update/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/file_update/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/file_update/file_update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/file_update/test_hook_file_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/copy-without-render.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/generate-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/looped-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/looped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/missing-file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/plain-src-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/plain-src-path.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/plain-src.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-dir-file-base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-dir-file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/contents/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/contents/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-error/file/{{foo}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-exception.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-file-additional-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render-file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/models/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/models/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/models/stuff-{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/models/stuff.py.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/no-render/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/no-render/dir/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/no-render/dir/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/{{stuff}}/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/render_src/{{stuff}}/stuff-{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-if-file-exists.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-input/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-input/skip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-input/there.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-output/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-output/skip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-output/there.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/skip-overwrite-files.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/tackle-provider-remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/plain_src/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/plain_src/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/plain_src/models/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/plain_src/models/stuff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/stuff-{{stuff}}.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/models/stuff-{{things}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/models/stuff.py.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/stuff-{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/types/type.tf
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/generate/unknown-variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/jinja/existing-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/jinja/tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/jinja/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/jinja/templates/things.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/expected-output.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/file.md
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/multi-line.md
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/multi-line.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/git/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/hooks/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/hooks/gits.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/hooks/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/hooks/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/git/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/tests/meta-flat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/tests/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/tests/repo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/git/tests/test_provider_git_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/ini/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ini/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/ini/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ini/hooks/ini.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/ini/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ini/tests/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ini/tests/test_provider_ini.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/json/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/json/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/json/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/json/hooks/jsons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/json/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/json/tests/json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/json/tests/read.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/json/tests/test_provider_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/json/tests/write.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/kubernetes/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/hooks/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/hooks/context.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/tests/context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/tests/kubeconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/tests/kubeconfig2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/kubernetes/tests/test_provider_k8s_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/logic/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/logic/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/hooks/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/hooks/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/hooks/while.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/logic/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/logic/tests/assertion/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/assertion/assert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/assertion/test_provider_logic_assert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/logic/tests/match/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/block-if.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/block-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/cases.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/lists.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/test_provider_logic_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/value-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/match/wrong-hook-type.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/logic/tests/while/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/logic/tests/while/while.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/find_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/listdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/hooks/symlinks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/a-path/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/a-path/path1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/a-path/path1/path2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/a-path/path1/path2/thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/a-path/thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/base-dir-name.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/dirs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/dirs/args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/dirs/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/flatten/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/flatten/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/flatten/test_provider_paths_flatten_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/glob.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dir/.hidden-stuff
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dir/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dir/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/.hidden-stuff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/dir1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/dir1/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/dir1/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/dir2/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/dir2/things.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/dirs/things.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/listdir/test_provider_system_listdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/parent.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/somedir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/somedir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/somedir/src.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/src.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/symlink/test_provider_system_symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/paths/tests/test_provider_system_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/postgres/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/postgres/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/postgres/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/postgres/hooks/query.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/postgres/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/rawlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/hooks/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/list_checked.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/list_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/map_checked.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/map_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/map_normal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/map_normal_checked.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/tackle-my-provider/
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/tackle-my-provider/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/confirm/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/confirm/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/confirm/test_provider_pyinquirer_confirm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/input/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/input/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/input/test_provider_prompt_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/password/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/password/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/password/test_provider_prompt_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/list_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/map_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/no-msg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/prompts/tests/select/test_prompt_provider_select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ssh/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/ssh/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ssh/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ssh/hooks/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ssh/hooks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/ssh/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/strings/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/strings/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/hooks/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/hooks/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/hooks/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/hooks/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/strings/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/strings/tests/b64/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/b64/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/b64/test_provider_strings_b64.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/strings/tests/random/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/random/random.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/random/test_provider_system_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/strings/tests/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/strings/join.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/strings/split.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/strings/tests/strings/test_provider_system_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/import.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/provider_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/run_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/tackle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/hooks/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/block-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/block-logic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/block-merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/embedded-blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/embedded-lists.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/fake-tackle/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/fake-tackle/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/looped-context-other.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/looped-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/looped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/test_provider_tackle_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/block/tmp-context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/debug/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/debug/test_provider_tackle_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/declarative-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/kubectl.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/ls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/flatten/ubuntu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/expanded-list-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/expanded-string.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/function-import.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/local.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test-provider/context_provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test-provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test-provider/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test-provider/hooks/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test-provider/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      968 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/import/test_provider_tackle_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/provider_docs/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/provider_docs/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/run_hook/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/run_hook/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/run_hook/test_provider_tackle_run_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/block-tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/fixture/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/fixture/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/fixture/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/kwargs-default-hook-arg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/kwargs-default-hook-target.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/kwargs-default-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/kwargs-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/local-no-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/local-prior-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/tackle/tests/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/variable/test_provider_tackle_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/tackle/tests/variable/var.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/toml/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/toml/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/hooks/tomls.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/toml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/tests/read.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/tests/test_provider_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/tests/working.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/toml/tests/write.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/types/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/types/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/types/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/types/hooks/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/types/hooks/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/types/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/types/tests/castings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/types/tests/test_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/types/tests/type.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/web/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/hooks/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/hooks/request.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/web/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/tests/delete.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/tests/get.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/tests/patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/tests/post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/tests/put.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/web/tests/test_requests_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/yaml/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/hooks/yaml_in_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/hooks/yamls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/providers/yaml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/append.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/before.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/filter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/list_yaml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/list_yaml_read.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/merge_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/merge_in_place.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/read.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/remove_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/remove_str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/test_provider_system_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/update_in_place.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/write.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/yamldecode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/providers/yaml/tests/yamlencode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/special_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2022-12-20 16:27:06.000000 tackle-0.4.9/tackle/utils/zipfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34567 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-20 16:27:37.000000 tackle-0.4.9/tackle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/cli/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/fixtures/.tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/cli/fixtures/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/fixtures/dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/fixtures/global-kwarg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/fixtures/help-mixed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/fixtures/input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/fixtures/tackle-hello.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/test_cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/cli/test_cli_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/exceptions/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/bad-extension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/calling-tackle-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/calling-tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/missing-quote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/unknown-argument-extra.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/unknown-argument.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/unknown-named-argument.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/unknown-variable-call-tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/unknown-variable-call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/fixtures/unknown-variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/exceptions/test_tackle_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/macros/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/macros/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/macros/fixtures/func-inputs-basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/macros/test_macros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/main/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/.tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/block-input-overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/block-input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/dict-input-overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/dict-input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/func-exec-input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/func-input.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/main/fixtures/home/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/home/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/home/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/main/fixtures/k8s/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/main/fixtures/k8s/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/k8s/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/fixtures/k8s/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/main/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/.hooks/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/child/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/child/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/child/dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/child/dir/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/context-provider-list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/cookiecutter-new-hook/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/cookiecutter-new-hook/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/cookiecutter-new-hook/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/cookiecutter-new-hook/hooks/stuff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/global.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-install-dep.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/test-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-provider/context_provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/test-provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-provider/hooks/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/test-provider-2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/test-provider-2/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-provider-2/hooks/stuff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/test-provider-reqs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/models/fixtures/test-provider-reqs/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-provider-reqs/hooks/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-provider-reqs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/test-provider-reqs/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/text2art.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/fixtures/unknown-hook-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/hook-dirs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/models/test_models_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/a-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/a-tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/exceptions/calling_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/calling_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/calling_dir/calling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/empty-with-functions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/empty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/function-input-validation-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/hook-input-validation-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/merge-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/exceptions/out-of-range-arg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/ansible-playbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/arg-types-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/arg-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/block-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/block.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/ansible-parse-call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/ansible-parse-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/ansible-parse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/empty-block-exception.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/nested-dict-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/nested-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/nested-for-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/nested-for.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/single-level-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/blocks/single-level.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/bug-mixed-flags-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/bug-mixed-flags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/calling-context-inner.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/calling-context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/dir/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/document-hooks-expected.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/document-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/dunder-key.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/duplicate-values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/embedded_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/empty-elements.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/empty-hooks-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/empty-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/inner-tackle-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/inner-tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/input-key/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/input-key/child/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/input-key/child/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/input-key/child/calling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/input-key/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/k8s-deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/list-list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/macros/compact-hook-macro.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/macros/list-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/map-lists-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/map-lists.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/map-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/map-root-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/map-root.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/match-case-logic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-dict-loop-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-dict-loop-exception.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-key-simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-list-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-list-value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-petstore-compact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-petstore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-simple-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/merge-simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/outer-tackle-arg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/outer-tackle-list-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/outer-tackle-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/outer-tackle-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/outer-tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/petstore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/private-context-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/private-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/private-hooks-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/private-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/ruamel-parsing-error-braces.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/fixtures/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/templates/file.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/toml.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/toml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/var-hook-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/fixtures/var-hook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/exceptions/hook-kwarg-missing-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/exceptions/hook-kwarg-missing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/exceptions/missing-field.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/exceptions/str-value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/exceptions/try-in-default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/.hooks/base-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/extends-visible.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/extends.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-args-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-exec-args-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-exec-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-exec-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-exec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/field-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/passed-context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/.hooks/some-hooks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/a-tackle/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/a-tackle/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/call-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-call-func-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-call-func.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-default-hook-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-default-hook-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-default-hook-embedded.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-default-hook-no-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-hook-no-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-hook-type-unknown.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/cli-no-default-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/compact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/default-method-json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/default-method-self.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/extends.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-bad-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-require.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-dict-error-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-dict-error-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-dict-error-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-list-error-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-list-error-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-list-error-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-str-error-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-str-error-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-exceptions/field-types-str-error-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-type-or-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/field-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/flatten.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider/a-dir/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider/tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-hook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-hook/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-hook/a-dir/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-hook/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-hook/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-hook/tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-method/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-method/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-method/a-dir/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-method/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-method/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/func-provider-method/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/list-call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-base-validate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-call-from-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-call-no-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-embed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-inherit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-maintain-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-nested-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-nested-override.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/method-single.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/no-exec-type-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/no-exec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/return-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/return-render.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/return-str-not-found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/return.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/supplied-args-param-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/supplied-args-param-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/supplied-kwargs-param-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/fixtures/supplied-kwargs-param-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_functions_args_kwargs_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_functions_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_functions_field_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/functions/test_functions_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/parser/method-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/method-fixtures/list-comprehension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/method-fixtures/method-else.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/method-fixtures/method-except.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/method-fixtures/method-try.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/method-fixtures/method-when.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/method-fixtures/try-validation-except.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_parser_args_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_parser_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_parser_hook_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_parser_macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_parser_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_parser_parse_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/parser/test_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/render/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/render/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/call-function-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/call-function.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/render/fixtures/dir/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/dir/stuff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/globals.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/hooks-args-too-many-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/hooks-args-wrong-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/hooks-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/hooks-missing-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/is-defined.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/multi-line-block-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/multi-line-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/multiple-hook-renders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/render-with-filters-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/render-with-filters.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/special-variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/unknown-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/fixtures/unknown-variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/test_render_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/render/test_special_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/test_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/files/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/bad.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/bad.stuff
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/bad.things
--rw-r--r--   0 runner    (1001) docker     (123)      234 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/documents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/fixtures/ok.toml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/files/test_utils_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/bad-zip-file.zip
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/empty.zip
--rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/fake-repo-tmpl.zip
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/not-a-repo.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/protected-fake-repo-tmpl.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/fixtures/valid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/fixtures/valid/tackle-input/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/valid/tackle-input/tackle.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/fixtures/valid/yaml-input/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/fixtures/valid/yaml-input/cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/test_unzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/test_utils_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/test_utils_dicts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:27:37.000000 tackle-0.4.9/tests/utils/vcs/
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/vcs/test_vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2022-12-20 16:27:06.000000 tackle-0.4.9/tests/utils/vcs/test_vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 17:58:34.000000 tackle-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 17:58:34.000000 tackle-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-11 17:59:01.000000 tackle-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-11 17:58:34.000000 tackle-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 17:58:34.000000 tackle-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 17:59:01.000000 tackle-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4821 2023-07-11 17:58:34.000000 tackle-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74797 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/collections/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/distinct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/list_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/map_to_list_key_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/notes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/collections/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/concatenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/distinct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/list-keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/sort-in-place.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/sort-map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/test_provider_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/command/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/hooks/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/hooks/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/command/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/exit-ignore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/exit-long.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/exit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/interactive.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/list-dir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/multi-line-cmd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/test_provider_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/console/
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/console/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/console/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/markdown.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/pprint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/print.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/table_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/test_provider_console_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/test_provider_console_rich.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/.tackle.meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/context/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/context/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/append-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/append-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/append.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/get.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/pop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/set.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/test_provider_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/update-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/datetime/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/hooks/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/datetime/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/tests/date_now.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/tests/test_provider_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/environment/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/hooks/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/environment/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/tests/envs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/tests/test_provider_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/hooks/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/hooks/zips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/chmod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/remove.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/shred.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/test_provider_system_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/zips/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/stuff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/stuff/motings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/things
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/test_provider_system_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/unzip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/zip-dir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/zip-file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/file_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/update_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/file_update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/test_hook_file_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/copy-without-render.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/generate-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/looped-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/looped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/missing-file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/plain-src-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/plain-src-path.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/plain-src.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-dir-file-base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-dir-file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/contents/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/file/{{foo}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-exception.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-file-additional-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/stuff-{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/stuff.py.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/no-render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/no-render/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/no-render/dir/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/{{stuff}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/{{stuff}}/stuff-{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-if-file-exists.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-input/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-input/skip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-input/there.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-output/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-output/skip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-output/there.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-overwrite-files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/tackle-provider-remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/models/stuff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/stuff-{{stuff}}.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/stuff-{{things}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/stuff.py.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/stuff-{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/types/type.tf
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/unknown-variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/existing-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/templates/things.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/expected-output.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/file.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/multi-line.md
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/multi-line.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/git/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/gits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/git/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/meta-flat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/repo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/test_provider_git_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ini/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ini/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/hooks/ini.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ini/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/tests/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/tests/test_provider_ini.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/json/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/hooks/jsons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/json/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/read.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/test_provider_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/write.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/test_provider_k8s_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/hooks/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/hooks/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/hooks/while.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/assertion/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/assertion/assert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/assertion/test_provider_logic_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/match/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/block-loop-match-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/block-match-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block-if.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block-merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-dict-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/cases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/default-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/default-underscore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-block-loop-merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-malformed-regex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-non-existant-key.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-wrong-hook-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/lists.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/test_provider_logic_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/while/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/while/while.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/find_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/listdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/symlinks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/path1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/path1/path2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/path1/path2/thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/base-dir-name.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/flatten/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/flatten/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/flatten/test_provider_paths_flatten_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/glob.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/.hidden-stuff
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/.hidden-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/.hidden-dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/.hidden-stuff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir1/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir1/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir2/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir2/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/test_provider_system_listdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/parent.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/somedir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/somedir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/somedir/src.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/src.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/test_provider_system_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/test_provider_system_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/postgres/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/hooks/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/rawlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/list_checked.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/list_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_checked.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_normal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_normal_checked.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/confirm/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/confirm/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/confirm/test_provider_pyinquirer_confirm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/input/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/input/test_provider_prompt_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/password/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/password/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/password/test_provider_prompt_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/list_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/map_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/no-msg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/test_prompt_provider_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ssh/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/hooks/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/hooks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/b64/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/b64/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/b64/test_provider_strings_b64.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/random/random.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/random/test_provider_system_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/join.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/test_provider_system_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/provider_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/run_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/tackle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-logic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-loop-block-nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-loop-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/embedded-blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/embedded-lists.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/fake-tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/fake-tackle/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/looped-context-other.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/looped-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/looped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/test_provider_tackle_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/tmp-context.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/debug/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/debug/test_provider_tackle_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/declarative-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/kubectl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/ls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/ubuntu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/expanded-list-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/expanded-string.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/function-import.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/local.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/context_provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/hooks/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test_provider_tackle_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/run_hook/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/run_hook/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/run_hook/test_provider_tackle_run_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/block-tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default-hook-arg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default-hook-target.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/local-no-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/local-prior-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/variable/test_provider_tackle_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/variable/var.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/toml/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/toml/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/hooks/tomls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/toml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/read.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/test_provider_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/working.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/write.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/types/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/hooks/casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/hooks/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/types/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/tests/castings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/tests/test_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/tests/type.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/web/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/hooks/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/hooks/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/get.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/put.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/test_requests_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/yaml/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/hooks/yaml_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/hooks/yamls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/yaml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/append.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/before.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/filter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/list_yaml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/list_yaml_read.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/merge_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/merge_in_place.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/read.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/remove_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/remove_str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/test_provider_system_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/update_in_place.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/write.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/yamldecode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/yamlencode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/special_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/zipfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36132 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/cli/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/.tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/cli/fixtures/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/global-kwarg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/help-mixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/tackle-hello.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/test_cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/test_cli_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/exceptions/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/bad-extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/calling-tackle-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/calling-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/missing-quote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-argument-extra.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-argument.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-named-argument.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-variable-call-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-variable-call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/test_tackle_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/.hooks/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/cli-fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/cli-fixtures/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/a-dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-call-func-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-call-func.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-embedded.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-no-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-hook-no-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-hook-type-unknown.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-no-default-hook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/composition-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/composition-fixtures/enum-basic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/extends-missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/field-bad-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/field-require.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/hook-kwarg-missing-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/hook-kwarg-missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/missing-field.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/no-exec-type-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/return-str-not-found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/str-value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/try-in-default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/extends-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/extends-fixtures/embedded-extends.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/extends-fixtures/extends-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/extends-fixtures/extends.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/.hooks/base-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/extends-visible.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/extends.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-args-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec-args-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/passed-context.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/.hooks/some-hooks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/a-tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/a-tackle/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/call-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/compact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/default-method-json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/default-method-self.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/extends.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-list-error-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-list-error-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-list-error-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-str-error-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-str-error-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-str-error-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/flatten.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/list-call.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/methods/method-embed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/no-exec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/return-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/return-render.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/return.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-args-param-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-args-param-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-kwargs-param-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-kwargs-param-str-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-kwargs-param-str.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/method-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-base-validate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-call-from-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-call-no-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-calll-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-embed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-inherit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-maintain-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-nested-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-nested-override.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-single.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_args_kwargs_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_field_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/types-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/base-embed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/dict-base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/enum-basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/enum-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/list-base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/macros/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/macros/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/macros/fixtures/func-inputs-basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/macros/test_macros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/.tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/block-input-overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/block-input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/dict-input-overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/dict-input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/func-exec-input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/func-input.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/home/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/home/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/home/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/k8s/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/k8s/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/k8s/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/k8s/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/.hooks/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/child/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/child/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/child/dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/child/dir/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/context-provider-list.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/hooks/stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/global.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-install-dep.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider/context_provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider/hooks/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-2/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-2/hooks/stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/hooks/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/text2art.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/unknown-hook-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/hook-dirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/test_models_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/base-method-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/list-comprehension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-dict-loop-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-dict-loop-exception.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-loop-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-loop-value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-else.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-except.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-try.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-when.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/try-validation-except.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/a-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/a-tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/calling_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/calling_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/calling_dir/calling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/empty-hook-call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/empty-with-functions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/function-input-validation-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/hook-input-validation-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/merge-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/out-of-range-arg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/.old/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/.old/merge-key-simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/ansible-playbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/arg-types-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/arg-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/block-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/block.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse-call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/empty-block-exception.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-dict-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-for-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-for.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/single-level-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/single-level.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/bug-mixed-flags-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/bug-mixed-flags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/calling-context-inner.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/calling-context.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/dir/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/document-hooks-expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/document-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/dunder-key.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/duplicate-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/embedded_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/empty-elements.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/empty-hooks-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/empty-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/inner-tackle-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/inner-tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/input-key/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/input-key/child/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/input-key/child/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/input-key/child/calling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/input-key/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/k8s-deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/list-list.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/macros/compact-hook-macro.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/macros/list-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-lists-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-lists.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-root-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-root.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/match-case-logic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-petstore-compact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-petstore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-simple-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-arg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-list-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/petstore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-context-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-hooks-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/ruamel-parsing-error-braces.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/templates/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/toml.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/toml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/var-hook-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/var-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_args_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_base_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_hook_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_parse_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/render/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/call-function-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/call-function.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/render/fixtures/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/dir/stuff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/globals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-args-too-many-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-args-wrong-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-missing-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/is-defined.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/multi-line-block-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/multi-line-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/multiple-hook-renders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/render-with-filters-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/render-with-filters.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/special-variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/unknown-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/unknown-variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_render_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_special_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/test_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/files/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/bad.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/bad.stuff
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/bad.things
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/documents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/ok.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/test_utils_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/bad-zip-file.zip
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/empty.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/fake-repo-tmpl.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/not-a-repo.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/protected-fake-repo-tmpl.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/valid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/valid/tackle-input/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/valid/tackle-input/tackle.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/valid/yaml-input/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/valid/yaml-input/cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_unzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_utils_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_utils_dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/vcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/vcs/test_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/vcs/test_vcs_provider.py
```

### Comparing `tackle-0.4.9/LICENSE` & `tackle-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/PKG-INFO` & `tackle-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: tackle
-Version: 0.4.9
+Version: 0.5.0
 Summary: Tackle is a declarative DSL for building modular workflows and code generators. Tool is plugins based and can easily be extended by writing additional hooks or importing external providers that can be turned into a self documenting CLI, all out of yaml, json, toml.
 Home-page: https://github.com/robcxyz/tackle
 Author: Rob Cannon
 Author-email: robc.io.opensource@gmail.com
 License: BSD
 Description: <img align="right" width="280" height="280" src="https://raw.githubusercontent.com/sudoblockio/tackle/main/docs/assets/logo-box.png">
         
         # tackle
         
         [![pypi](https://img.shields.io/pypi/v/tackle.svg)](https://pypi.python.org/pypi/tackle)
         [![python](https://img.shields.io/pypi/pyversions/tackle.svg)](https://pypi.python.org/pypi/tackle)
         [![codecov](https://codecov.io/gh/sudoblockio/tackle/branch/main/graphs/badge.svg?branch=main)](https://codecov.io/github/sudoblockio/tackle?branch=main)
         [![codeql](https://github.com/sudoblockio/tackle/actions/workflows/codeql.yml/badge.svg)](https://github.com/sudoblockio/tackle/actions/workflows/codeql.yml)
-        [![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/success?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
-        [![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/test?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
-        [![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/utilization?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
         
         [//]: # ([![main-tests]&#40;https://github.com/sudoblockio/tackle/actions/workflows/main.yml/badge.svg&#41;]&#40;https://github.com/sudoblockio/tackle/actions&#41;)
         
         * [Documentation](https://sudoblockio.github.io/tackle)
         * [Discord](https://discord.gg/7uVUfUVD7K)
         * [PyPI](https://pypi.org/project/tackle/)
         * [BSD License](LICENSE)
         
         [//]: # (* [Slack]&#40;https://join.slack.com/t/slack-y748219/shared_invite/zt-1cqreswyd-5qDBE53QlY97mQOI6DhcKw&#41;)
         
-        Tackle is an experimental general purpose configuration language for building modular code generators and declarative CLIs. Built as a fork of [cookiecutter](https://github.com/cookiecutter/cookiecutter), it can make any config file dynamic or into a CLI with both strong and weakly typed programmable flow control common to a general purpose programming language. Basically you can write a fully functional Turing-complete program out of a config file. It's wild.
+        Tackle is an experimental general purpose configuration language for building modular code generators and declarative CLIs. Built as a fork of [cookiecutter](https://github.com/cookiecutter/cookiecutter), it can make any config file into a CLI with both strong and weakly typed programmable flow control common to a general purpose programming language. Basically you can write a fully functional Turing-complete program out of a config file. It's wild.
         
         **With tackle, you can build:**
         - Modular code generators / repo scaffolding tools that can be updated over time
         - Interactive glue code for infrastructure-as-code deployment strategies
         - Generic utilities like SSH helpers and dotfile managers
         - Combinations of all of the above and anything else you can think of
         
@@ -50,29 +47,30 @@
           - Read and write [yaml](https://sudoblockio.github.io/tackle/providers/Yaml/) / [toml](https://sudoblockio.github.io/tackle/providers/Toml/) / [json](https://sudoblockio.github.io/tackle/providers/Json/) [files](https://sudoblockio.github.io/tackle/providers/Files/)
           - [Make http calls](https://sudoblockio.github.io/tackle/providers/Web/)
           - [Run arbitrary system commands](https://sudoblockio.github.io/tackle/providers/Command/)
           - [Manipulate the context](https://sudoblockio.github.io/tackle/providers/Context/)
           - [Run other tackle files](https://sudoblockio.github.io/tackle/providers/Tackle/tackle/)
         - Modular design allows creating / importing new hooks easy
           - Supports both [python](https://sudoblockio.github.io/tackle/python-hooks/) and [declarative](https://sudoblockio.github.io/tackle/declarative-hooks/) hooks which can be imported / called / defined in-line or within jinja templates
+          - Hooks can be composed of other hooks allowing complex objects to be validated and operated against
         
         ### Install
         
         > Note: tackle can install dependencies on its own. Check [docs](https://sudoblockio.github.io/tackle/installation#best-installation-method) for advanced installation methods to isolate tackle from your system python.
         
         ```shell
         python -m venv env && source env/bin/activate
         pip install tackle
         ```
         
         **Quick Demo:** `tackle sudoblockio/tackle-hello-world`
         
         ### Hello world
         
-        Check out the [docs](https://sudoblockio.github.io/tackle/hello-worlds/) for >10 hello worlds that demonstrate the various aspects of the syntax with the simplest one using the [print](https://sudoblockio.github.io/tackle/providers/Console/print/) hook, one of [>100 hooks](https://sudoblockio.github.io/tackle/installation#best-installation-method).
+        Check out the [docs](https://sudoblockio.github.io/tackle/hello-worlds/) for >10 hello worlds that demonstrate the various aspects of the syntax with the simplest one using the [print](https://sudoblockio.github.io/tackle/providers/Console/print/) hook, one of [>100 hooks](https://sudoblockio.github.io/tackle/providers/Collections/).
         
         **hello.yaml**
         ```yaml
         # Any time a key ends with `->`, we are calling a hook
         hw->: print Hello world!
         ```
         
@@ -96,14 +94,15 @@
             - world!
           if: item != 'cruel'
         # Or combinations of the above with other methods like try/except
         ```
         
         New hooks can be [made in python](https://sudoblockio.github.io/tackle/python-hooks/) which under the hood is a [pydantic](https://github.com/pydantic/pydantic) model.
         
+        **.hooks/hello.py**
         ```python
         from tackle import BaseHook
         
         class Greeter(BaseHook):
             hook_type: str = "greeter"
             target: str
             args: list = ['target']
@@ -111,61 +110,65 @@
               expression = f"Hello {self.target}"
               print(expression)
               return expression
         ```
         
         Or can be [defined inline within your tackle file, imported remotely, or in a `hooks` directory.](https://sudoblockio.github.io/tackle/declarative-hooks/).
         
+        **.hooks/hello.yaml**
         ```yaml
         # Keys ending with `<-` mean we are creating a hook / method
         greeter<-:
           target: str
           args: ['target']
           exec<-:
             expression->: var Hello {{target}}  # var hook renders variables
             p->: print {{expression}}
           return: expression
         ```
         
         And both can be [called the same way](https://sudoblockio.github.io/tackle/writing-tackle-files/).
         
+        **tackle.yaml**
         ```yaml
         hello: world!
         With a flag->: greeter --target {{hello}}
         Target in argument->: greeter {{hello}}
         Expanded fields:
           ->: greeter
           target: {{hello}}
         Jinja template->: {{ greeter(hello) }}
         # Or combinations jinja and compact / expanded hooks allowing chaining of hook calls.
         ```
         
-        With the declarative hooks being callable from the command line:
+        With the declarative hooks being [callable from the command line](https://sudoblockio.github.io/tackle/declarative-cli/):
         
         ```shell
         tackle hello.yaml greeter --target world!
         # Or from a github repo
         tackle sudoblockio/tackle-hello-world greeter --target world!
         ```
         
         Documentation can be embedded into the hooks.
         
+        **hello.yaml**
         ```yaml
         <-:
           help: This is the default hook
           target:
-            type: str
+            type: union[str, int]
             default->: input
             description: The thing to say hello to
           exec<-:
             greeting->: select Who to greet? --choices ['world',target]
             hi->: greeter --target {{greeting}}
           greeting-method<-:
             help: A method that greets
             # ... Greeting options / logic
+            extends: greeter
         greeter<-:
           help: A reusable greeter object
           target: str
           exec<-:
             hi->: print Hello {{target}}
         ```
         
@@ -179,26 +182,26 @@
         options:
             --target [str] The thing to say hello to
         methods:
             greeting-method     A method that greets
             greeter     A reusable greeter object
         ```
         
-        Hooks can be imported, linked, and/or combined creating a web of CLIs.
+        Hooks can be imported [within a tackle provider](https://sudoblockio.github.io/tackle/declarative-cli/#importing-hooks) or [through hooks](https://sudoblockio.github.io/tackle/providers/Tackle/import/), [linked](https://sudoblockio.github.io/tackle/providers/Tackle/tackle/), and/or combined with [inheritance](https://sudoblockio.github.io/tackle/declarative-hooks/#extending-hooks) or [composition](https://sudoblockio.github.io/tackle/declarative-hooks/#extending-hooks) creating a web of CLIs.
         
         ### Use Cases
         
         - [Code Generation](https://sudoblockio.github.io/tackle/tutorials/code-generation/)
         
         **WIP Tutorials**
         
-        - [Declarative Utilities]()
-        - [Infrastructure-as-Code Management]()
-        - [Kubernetes Manifest Management]()
-        - [Toolchain Management]()
+        - Declarative Utilities
+        - Infrastructure-as-Code Management
+        - Kubernetes Manifest Management
+        - Toolchain Management
         
         [//]: # (- [Repo Management]&#40;&#41; - wip)
         
         ### Topics
         
         - [Writing Tackle Files](https://sudoblockio.github.io/tackle/writing-tackle-files/)
         - [Creating Providers](https://sudoblockio.github.io/tackle/creating-providers/)
@@ -210,16 +213,15 @@
         - [Declarative CLIs](https://sudoblockio.github.io/tackle/declarative-cli/)
         
         ### Known Issues
         
         - **Windows Support**
           - tackle is lacking some windows support as shown in the [failed tests](https://github.com/sudoblockio/tackle/actions/workflows/main-windows.yml). If you are a windows user, it is highly recommended to use WSL. **Please get in touch** if you are motivated to fix these tests to make tackle fully cross-platform. It probably isn't that hard to fix them as they mostly are due to differences in how windows handles paths.
         - **Whitespaces**
-          - tackle relies heavily on parsing based on whitespaces which if you are not careful can easily bite you. Whenever you need to have some whitespaces preserved, make sure to quote the entire expression.
-        
+          - tackle relies heavily on parsing based on whitespaces which if you are not careful can easily bite you. Whenever you need to have some whitespaces preserved, make sure to quote the entire expression. Future work will be put in to overhaul the [regex based parser](https://github.com/sudoblockio/tackle/blob/main/tackle/utils/command.py#L52) with a PEG parser like [parsimonious](https://github.com/erikrose/parsimonious).
         
         ### Contributing
         
         Contributions are welcome but please be advised of the following notes.
         
         - This project uses [conventional commits](https://www.conventionalcommits.org/) which generates the [changelog](./CHANGELOG.md) with [release-please-action](https://github.com/google-github-actions/release-please-action) in the [release](https://github.com/sudoblockio/tackle/blob/main/.github/workflows/release.yml) CI workflow. If commits have been made outside of this convention they will be squashed accordingly.
         - For making changes to providers, please include test coverage using the existing fixtures and patterns from prior tests or communicate any suggestions that deviate from this style. It definitely can be improved but consistency is more important than making directed improvements. Tests should be runnable from the test's directory and via `make test`.
@@ -250,16 +252,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: web
-Provides-Extra: toml
 Provides-Extra: ssh
-Provides-Extra: console
 Provides-Extra: git
-Provides-Extra: postgres
 Provides-Extra: kubernetes
+Provides-Extra: web
+Provides-Extra: postgres
+Provides-Extra: toml
+Provides-Extra: console
 Provides-Extra: dev
 Provides-Extra: all
```

### Comparing `tackle-0.4.9/README.md` & `tackle-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 
 # tackle
 
 [![pypi](https://img.shields.io/pypi/v/tackle.svg)](https://pypi.python.org/pypi/tackle)
 [![python](https://img.shields.io/pypi/pyversions/tackle.svg)](https://pypi.python.org/pypi/tackle)
 [![codecov](https://codecov.io/gh/sudoblockio/tackle/branch/main/graphs/badge.svg?branch=main)](https://codecov.io/github/sudoblockio/tackle?branch=main)
 [![codeql](https://github.com/sudoblockio/tackle/actions/workflows/codeql.yml/badge.svg)](https://github.com/sudoblockio/tackle/actions/workflows/codeql.yml)
-[![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/success?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
-[![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/test?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
-[![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/utilization?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
 
 [//]: # ([![main-tests]&#40;https://github.com/sudoblockio/tackle/actions/workflows/main.yml/badge.svg&#41;]&#40;https://github.com/sudoblockio/tackle/actions&#41;)
 
 * [Documentation](https://sudoblockio.github.io/tackle)
 * [Discord](https://discord.gg/7uVUfUVD7K)
 * [PyPI](https://pypi.org/project/tackle/)
 * [BSD License](LICENSE)
 
 [//]: # (* [Slack]&#40;https://join.slack.com/t/slack-y748219/shared_invite/zt-1cqreswyd-5qDBE53QlY97mQOI6DhcKw&#41;)
 
-Tackle is an experimental general purpose configuration language for building modular code generators and declarative CLIs. Built as a fork of [cookiecutter](https://github.com/cookiecutter/cookiecutter), it can make any config file dynamic or into a CLI with both strong and weakly typed programmable flow control common to a general purpose programming language. Basically you can write a fully functional Turing-complete program out of a config file. It's wild.
+Tackle is an experimental general purpose configuration language for building modular code generators and declarative CLIs. Built as a fork of [cookiecutter](https://github.com/cookiecutter/cookiecutter), it can make any config file into a CLI with both strong and weakly typed programmable flow control common to a general purpose programming language. Basically you can write a fully functional Turing-complete program out of a config file. It's wild.
 
 **With tackle, you can build:**
 - Modular code generators / repo scaffolding tools that can be updated over time
 - Interactive glue code for infrastructure-as-code deployment strategies
 - Generic utilities like SSH helpers and dotfile managers
 - Combinations of all of the above and anything else you can think of
 
@@ -42,29 +39,30 @@
   - Read and write [yaml](https://sudoblockio.github.io/tackle/providers/Yaml/) / [toml](https://sudoblockio.github.io/tackle/providers/Toml/) / [json](https://sudoblockio.github.io/tackle/providers/Json/) [files](https://sudoblockio.github.io/tackle/providers/Files/)
   - [Make http calls](https://sudoblockio.github.io/tackle/providers/Web/)
   - [Run arbitrary system commands](https://sudoblockio.github.io/tackle/providers/Command/)
   - [Manipulate the context](https://sudoblockio.github.io/tackle/providers/Context/)
   - [Run other tackle files](https://sudoblockio.github.io/tackle/providers/Tackle/tackle/)
 - Modular design allows creating / importing new hooks easy
   - Supports both [python](https://sudoblockio.github.io/tackle/python-hooks/) and [declarative](https://sudoblockio.github.io/tackle/declarative-hooks/) hooks which can be imported / called / defined in-line or within jinja templates
+  - Hooks can be composed of other hooks allowing complex objects to be validated and operated against
 
 ### Install
 
 > Note: tackle can install dependencies on its own. Check [docs](https://sudoblockio.github.io/tackle/installation#best-installation-method) for advanced installation methods to isolate tackle from your system python.
 
 ```shell
 python -m venv env && source env/bin/activate
 pip install tackle
 ```
 
 **Quick Demo:** `tackle sudoblockio/tackle-hello-world`
 
 ### Hello world
 
-Check out the [docs](https://sudoblockio.github.io/tackle/hello-worlds/) for >10 hello worlds that demonstrate the various aspects of the syntax with the simplest one using the [print](https://sudoblockio.github.io/tackle/providers/Console/print/) hook, one of [>100 hooks](https://sudoblockio.github.io/tackle/installation#best-installation-method).
+Check out the [docs](https://sudoblockio.github.io/tackle/hello-worlds/) for >10 hello worlds that demonstrate the various aspects of the syntax with the simplest one using the [print](https://sudoblockio.github.io/tackle/providers/Console/print/) hook, one of [>100 hooks](https://sudoblockio.github.io/tackle/providers/Collections/).
 
 **hello.yaml**
 ```yaml
 # Any time a key ends with `->`, we are calling a hook
 hw->: print Hello world!
 ```
 
@@ -88,14 +86,15 @@
     - world!
   if: item != 'cruel'
 # Or combinations of the above with other methods like try/except
 ```
 
 New hooks can be [made in python](https://sudoblockio.github.io/tackle/python-hooks/) which under the hood is a [pydantic](https://github.com/pydantic/pydantic) model.
 
+**.hooks/hello.py**
 ```python
 from tackle import BaseHook
 
 class Greeter(BaseHook):
     hook_type: str = "greeter"
     target: str
     args: list = ['target']
@@ -103,61 +102,65 @@
       expression = f"Hello {self.target}"
       print(expression)
       return expression
 ```
 
 Or can be [defined inline within your tackle file, imported remotely, or in a `hooks` directory.](https://sudoblockio.github.io/tackle/declarative-hooks/).
 
+**.hooks/hello.yaml**
 ```yaml
 # Keys ending with `<-` mean we are creating a hook / method
 greeter<-:
   target: str
   args: ['target']
   exec<-:
     expression->: var Hello {{target}}  # var hook renders variables
     p->: print {{expression}}
   return: expression
 ```
 
 And both can be [called the same way](https://sudoblockio.github.io/tackle/writing-tackle-files/).
 
+**tackle.yaml**
 ```yaml
 hello: world!
 With a flag->: greeter --target {{hello}}
 Target in argument->: greeter {{hello}}
 Expanded fields:
   ->: greeter
   target: {{hello}}
 Jinja template->: {{ greeter(hello) }}
 # Or combinations jinja and compact / expanded hooks allowing chaining of hook calls.
 ```
 
-With the declarative hooks being callable from the command line:
+With the declarative hooks being [callable from the command line](https://sudoblockio.github.io/tackle/declarative-cli/):
 
 ```shell
 tackle hello.yaml greeter --target world!
 # Or from a github repo
 tackle sudoblockio/tackle-hello-world greeter --target world!
 ```
 
 Documentation can be embedded into the hooks.
 
+**hello.yaml**
 ```yaml
 <-:
   help: This is the default hook
   target:
-    type: str
+    type: union[str, int]
     default->: input
     description: The thing to say hello to
   exec<-:
     greeting->: select Who to greet? --choices ['world',target]
     hi->: greeter --target {{greeting}}
   greeting-method<-:
     help: A method that greets
     # ... Greeting options / logic
+    extends: greeter
 greeter<-:
   help: A reusable greeter object
   target: str
   exec<-:
     hi->: print Hello {{target}}
 ```
 
@@ -171,26 +174,26 @@
 options:
     --target [str] The thing to say hello to
 methods:
     greeting-method     A method that greets
     greeter     A reusable greeter object
 ```
 
-Hooks can be imported, linked, and/or combined creating a web of CLIs.
+Hooks can be imported [within a tackle provider](https://sudoblockio.github.io/tackle/declarative-cli/#importing-hooks) or [through hooks](https://sudoblockio.github.io/tackle/providers/Tackle/import/), [linked](https://sudoblockio.github.io/tackle/providers/Tackle/tackle/), and/or combined with [inheritance](https://sudoblockio.github.io/tackle/declarative-hooks/#extending-hooks) or [composition](https://sudoblockio.github.io/tackle/declarative-hooks/#extending-hooks) creating a web of CLIs.
 
 ### Use Cases
 
 - [Code Generation](https://sudoblockio.github.io/tackle/tutorials/code-generation/)
 
 **WIP Tutorials**
 
-- [Declarative Utilities]()
-- [Infrastructure-as-Code Management]()
-- [Kubernetes Manifest Management]()
-- [Toolchain Management]()
+- Declarative Utilities
+- Infrastructure-as-Code Management
+- Kubernetes Manifest Management
+- Toolchain Management
 
 [//]: # (- [Repo Management]&#40;&#41; - wip)
 
 ### Topics
 
 - [Writing Tackle Files](https://sudoblockio.github.io/tackle/writing-tackle-files/)
 - [Creating Providers](https://sudoblockio.github.io/tackle/creating-providers/)
@@ -202,16 +205,15 @@
 - [Declarative CLIs](https://sudoblockio.github.io/tackle/declarative-cli/)
 
 ### Known Issues
 
 - **Windows Support**
   - tackle is lacking some windows support as shown in the [failed tests](https://github.com/sudoblockio/tackle/actions/workflows/main-windows.yml). If you are a windows user, it is highly recommended to use WSL. **Please get in touch** if you are motivated to fix these tests to make tackle fully cross-platform. It probably isn't that hard to fix them as they mostly are due to differences in how windows handles paths.
 - **Whitespaces**
-  - tackle relies heavily on parsing based on whitespaces which if you are not careful can easily bite you. Whenever you need to have some whitespaces preserved, make sure to quote the entire expression.
-
+  - tackle relies heavily on parsing based on whitespaces which if you are not careful can easily bite you. Whenever you need to have some whitespaces preserved, make sure to quote the entire expression. Future work will be put in to overhaul the [regex based parser](https://github.com/sudoblockio/tackle/blob/main/tackle/utils/command.py#L52) with a PEG parser like [parsimonious](https://github.com/erikrose/parsimonious).
 
 ### Contributing
 
 Contributions are welcome but please be advised of the following notes.
 
 - This project uses [conventional commits](https://www.conventionalcommits.org/) which generates the [changelog](./CHANGELOG.md) with [release-please-action](https://github.com/google-github-actions/release-please-action) in the [release](https://github.com/sudoblockio/tackle/blob/main/.github/workflows/release.yml) CI workflow. If commits have been made outside of this convention they will be squashed accordingly.
 - For making changes to providers, please include test coverage using the existing fixtures and patterns from prior tests or communicate any suggestions that deviate from this style. It definitely can be improved but consistency is more important than making directed improvements. Tests should be runnable from the test's directory and via `make test`.
```

### Comparing `tackle-0.4.9/setup.py` & `tackle-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     )
     return provider_requirements
 
 
 INSTALL_REQUIREMENTS = [
     'Jinja2>3.0.0',
     # 'requests>=2.23.0',  # This would be needed if we allowed url sources
-    'pydantic>=1.8.0',
+    'pydantic>=1.8.0,<2.0.0',
     'InquirerPy>=0.3.3',
     'ruamel.yaml>=0.17.0',
     'rich>=12.6.0',
     'xdg==5.1.1',
 ]
 
 if sys.argv[-1] == 'readme':
```

### Comparing `tackle-0.4.9/tackle/cli.py` & `tackle-0.5.0/tackle/cli.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/exceptions.py` & `tackle-0.5.0/tackle/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,17 @@
 #
 # Parser exceptions
 #
 class TackleParserException(Exception):
     """Base parser exception class."""
 
     def __init__(self, extra_message: str, context: 'Union[Context, BaseContext]'):
+        if context.current_file is None:
+            context.current_file = context.calling_file
+
         self.message = (
             f"Error parsing input_file='{context.current_file}' at "
             f"key_path='{get_readable_key_path(key_path=context.key_path)}' \n"
             f"{extra_message}"
         )
         if not context.verbose:
             sys.tracebacklimit = 0
```

### Comparing `tackle-0.4.9/tackle/hooks.py` & `tackle-0.5.0/tackle/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,19 @@
 
 def import_from_path(
     context: 'Context',
     provider_path: str,
     hooks_dir_name: str = None,
     skip_on_error: bool = True,
 ):
-    """Append a provider with a given path."""
+    """
+    Update the public / private provider dicts with hooks found in the __init__.py,
+     as `hook_types = ["hook_type"]` which will be imported as LazyBaseHooks
+     provider (value).
+    """
     # Look for `.hooks` or `hooks` dir
     if hooks_dir_name is None:
         provider_contents = os.listdir(provider_path)
         if '.hooks' in provider_contents:
             hooks_dir_name = '.hooks'
         elif 'hooks' in provider_contents:
             hooks_dir_name = 'hooks'
@@ -151,28 +155,20 @@
         if file_contents is None:
             if context.verbose:
                 print(f"Skipping importing {file_path} as the context is empty.")
             return
         for k, v in file_contents.items():
             if re.match(r'^[a-zA-Z0-9\_]*(<\-)$', k):
                 hook_type = k[:-2]
-                # context.public_context[hook_type] = LazyBaseFunction(
-                #     function_dict=v,
-                #     # function_fields=[],
-                # )
                 context.public_hooks[hook_type] = LazyBaseFunction(
                     function_dict=v,
                     # function_fields=[],
                 )
             elif re.match(r'^[a-zA-Z0-9\_]*(<\_)$', k):
                 hook_type = k[:-2]
-                # context.private_context[hook_type] = LazyBaseFunction(
-                #     function_dict=v,
-                #     # function_fields=[],
-                # )
                 context.private_hooks[hook_type] = LazyBaseFunction(
                     function_dict=v,
                     # function_fields=[],
                 )
         return
 
     if os.path.basename(file_path).split('.')[-1] != "py":
@@ -224,16 +220,17 @@
      a hooks directory and importing all the relevant hooks into the context.
     """
     potential_hooks = listdir_absolute(path)
     for f in potential_hooks:
         if skip_on_error:
             try:
                 import_hook_from_path(context, mod_name, f)
-            except (ModuleNotFoundError, ConfigError, ImportError):
-                logger.debug(f"Skipping importing {f}")
+            except (ModuleNotFoundError, ConfigError, ImportError) as e:
+                if context.verbose:
+                    logger.info(f"Skipping importing {f} - {e}")
                 continue
         else:
             import_hook_from_path(context, mod_name, f)
 
 
 def import_with_fallback_install(
     context: 'Context',
```

### Comparing `tackle-0.4.9/tackle/macros.py` & `tackle-0.5.0/tackle/macros.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING
 
 from tackle.utils.dicts import (
     nested_get,
     nested_delete,
     nested_set,
     get_target_and_key,
-    smush_key_path,
+    remove_arrows_from_key_path,
 )
 
 from tackle import exceptions
 from tackle.models import BaseHook
 
 if TYPE_CHECKING:
     from tackle.models import Context
@@ -64,14 +64,17 @@
     ]
     input_dict = nested_get(
         element=context.input_context,
         keys=indexed_key_path[:-1],
     )
     value = input_dict[indexed_key_path[-1]]
 
+    if value is None:
+        raise exceptions.HookCallException("Empty hook call found.", context=context)
+
     for k, v in list(input_dict.items()):
         if k == indexed_key_path[-1]:
             nested_set(context.input_context, key_path, {arrow[0]: 'block'})
             nested_delete(context.input_context, indexed_key_path)
         else:
             input_dict[k] = input_dict.pop(k)
 
@@ -106,15 +109,15 @@
     arrow = context.key_path[-1][-2:]
 
     extra_keys = len(context.key_path) - len(context.key_path_block)
     old_key_path = context.key_path[-extra_keys:]
 
     value = nested_get(
         element=context.input_context,
-        keys=smush_key_path(old_key_path)[:-1],
+        keys=remove_arrows_from_key_path(old_key_path)[:-1],
     )
 
     replacement = {context.key_path[-1]: new_key[0]}
     for k, v in list(value.items()):
         value[replacement.get(k, k)] = (
             value.pop(k) if k != context.key_path[-1] else {arrow: value.pop(k)}
         )
@@ -154,14 +157,15 @@
         context.input_context = {arrow: 'var', 'input': element}
         context.key_path = base_key_path
 
     return {arrow: 'var'}
 
 
 def raise_on_private_hook(k: str, context: 'Context', func_name: str):
+    # TODO: Remove this and turn it into marking the field as non-exportable
     raise exceptions.MalformedFunctionFieldException(
         f"The field {k} can not be a private hook call (ie ending in '_>') as there is "
         f"no situation this makes sense.",
         function_name=func_name,
         context=context,
     )
 
@@ -205,14 +209,15 @@
         elif '->' in v:
             func_dict[k] = {'default': v}
 
         elif '_>' in v:
             raise_on_private_hook(k, context=context, func_name=func_name)
 
         elif 'default->' in v:
+            # TODO: Generalize this so that all fields are parsed
             new_value = func_dict[k].pop('default->')
             func_dict[k]['default'] = {'->': new_value}
 
         elif 'default_>' in v:
             raise_on_private_hook(k, context=context, func_name=func_name)
 
     return func_dict
```

### Comparing `tackle-0.4.9/tackle/main.py` & `tackle-0.5.0/tackle/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Union
 
 from tackle.models import Context
-from tackle.parser import update_source
+from tackle.parser import parse_source
 from tackle.utils.paths import find_nearest_tackle_file
 from tackle.utils.files import read_config_file
 from tackle import exceptions
 
 
 def get_global_kwargs(kwargs):
     """Check for unknown kwargs and return so that they can be consumed later."""
@@ -77,11 +77,11 @@
                     f"be a path to an file. Exiting.",
                     context=context,
                 )
         elif isinstance(overrides, dict):
             context.override_context.update(overrides)
 
     # Main loop
-    output = update_source(context)
+    output = parse_source(context)
     if output is None:
         return context.public_context
     return output
```

### Comparing `tackle-0.4.9/tackle/models.py` & `tackle-0.5.0/tackle/models.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/parser.py` & `tackle-0.5.0/tackle/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,41 @@
+"""
+`parser.py` is the core parser for tackle. It does the following steps
+
+- Reads in a tackle provider and loads its / hooks
+- Iterate through any keys on the tackle file
+  - Perform macros on conditions to
+  - Copy input values over to an output dictionary
+  - Find hook calls
+- Run the hook
+  - Perform any logic (if / else / for etc)
+  - Call the actual hook
+  - Insert the output into the appropriate key within the output context
+"""
 from collections import OrderedDict
+import enum
 from functools import partialmethod
 import os
 from pydantic import Field, create_model, ValidationError
 from pydantic.main import ModelMetaclass
 from pydantic.fields import ModelField
 from pydoc import locate
 from pathlib import Path
 import re
 from ruamel.yaml.constructor import CommentedKeyMap, CommentedMap
 from ruamel.yaml.parser import ParserError
+import typing
 from typing import Type, Any, Union, Callable, Optional
 
 from tackle import exceptions
 from tackle.hooks import (
     import_from_path,
     import_with_fallback_install,
-    LazyImportHook,
     LazyBaseFunction,
+    LazyImportHook,
 )
 from tackle.macros import (
     var_hook_macro,
     blocks_macro,
     compact_hook_call_macro,
     list_to_var_macro,
     function_field_to_parseable_macro,
@@ -31,23 +46,24 @@
     BaseFunction,
     FunctionInput,
     BaseContext,
 )
 from tackle.render import render_variable
 from tackle.settings import settings
 from tackle.utils.dicts import (
+    get_readable_key_path,
+    get_set_temporary_context,
+    get_target_and_key,
     nested_get,
     nested_delete,
     nested_set,
     encode_list_index,
     decode_list_index,
     set_key,
-    get_target_and_key,
-    smush_key_path,
-    get_readable_key_path,
+    remove_arrows_from_key_path,
     cleanup_unquoted_strings,
 )
 from tackle.utils.command import unpack_args_kwargs_string
 from tackle.utils.files import read_config_file
 from tackle.utils.help import run_help
 from tackle.utils.imports import get_public_or_private_hook
 from tackle.utils.render import wrap_jinja_braces
@@ -72,171 +88,133 @@
     'try',
     'except',
     'chdir',
     'merge',
 ]
 
 
-def get_hook(hook_type, context: 'Context') -> Type[BaseHook]:
-    """
-    Get the hook from providers. Qualify if the hook is a method and if it is a lazy
-    hook (ie has requirements that have not been installed), install them.
-    """
-    if '.' in hook_type:
-        # When the hook type has a period in it, we are calling a hook's method. Here we
-        # are going to split up the call into methods denoted by periods, and do logic
-        # to support inheriting base properties into methods. To do this we need to
-        # instantiate the base and use the `function_fields` list to inform which
-        # fields will be inherited. See `create_function_model` function for more info.
-        hook_parts = hook_type.split('.')
-
-        # Extract the base hook.
-        hook_type = hook_parts.pop(0)
-        h = get_public_or_private_hook(context, hook_type)
-        if h is None:
-            exceptions.raise_unknown_hook(context, hook_type)
-
-        # TODO: To support calling python hook methods, put a conditional here to
-        #  determine if hook is of type BaseHook / LazyImportHook and perform logic
-        #  separate from the declarative hook.
-        for method in hook_parts:
-            new_hook = None
-
-            # TODO: Fix this -> https://github.com/sudoblockio/tackle/issues/113
-            # When hooks are in `hooks` dir we apparently need to instantiate the base
-            if isinstance(h, LazyBaseFunction):
-                h = create_function_model(
-                    context=context,
-                    func_name=method,
-                    func_dict=h.function_dict.copy(),
-                )
-
-            try:
-                new_hook = h.__fields__[method].default
-            except (IndexError, KeyError):
-                # Raise error - method not found
-                exceptions.raise_unknown_hook(context, method, method=True)
-
-            # Update method with values from base class so that fields can be inherited
-            # from the base hook. function_fields is a list of those fields that aren't
-            # methods / special vars (ie args, return, etc).
-            for i in h.__fields__['function_fields'].default:
-                if i not in new_hook.function_dict:
-                    # Base method should not override child.
-                    new_hook.function_dict[i] = h.__fields__['function_dict'].default[i]
-                    if new_hook.function_fields is None:
-                        new_hook.function_fields = []
-
-                    new_hook.function_fields.append(i)
-
-            # Methods that are of type LazyBaseFunction which need to have the base
-            # instantiated before getting the hook. Allows nested methods for functions.
-            if isinstance(new_hook, LazyBaseFunction):
-                new_hook = create_function_model(
-                    context=context,
-                    func_name=h.__fields__[method].name,
-                    func_dict=new_hook.function_dict.copy(),
-                )
+def get_hook(
+    context: 'Context',
+    hook_type: str,
+    args: list,
+    kwargs: dict,
+) -> Optional[Type[BaseHook]]:
+    """Gets the hook from the context and calls enrich_hook."""
+    hook = get_public_or_private_hook(context=context, hook_type=hook_type)
+    if hook is None:
+        return None
+    return enrich_hook(
+        context=context,
+        hook=hook,
+        args=args,
+        kwargs=kwargs,
+    )
 
-            h = new_hook
 
-    else:
-        h = get_public_or_private_hook(context, hook_type)
-    if h is None:
-        # Raise exception for unknown hook
-        exceptions.raise_unknown_hook(context, hook_type)
-
-    # LazyImportHook in hook ref when declared in provider __init__.hook_types
-    elif isinstance(h, LazyImportHook):
-        # Install the requirements which will convert all the hooks in that provider
-        #  to actual hooks
-        import_with_fallback_install(
+def enrich_hook(
+    context: 'Context',
+    hook: ModelMetaclass,
+    args: list,
+    kwargs: dict,
+) -> Type[BaseHook]:
+    """
+    Take a hook and enrich it by lining up the args with potential methods / hook args /
+     kwargs. For methods, it recognizes the arg is a method, compiles the method hook
+     with the attributes of the base hook making it inherit them.
+    """
+    # This gets hit when you use an imported declarative hook
+    if isinstance(hook, LazyBaseFunction):
+        hook = create_function_model(
             context=context,
-            mod_name=h.mod_name,
-            path=h.hooks_path,
+            func_name=context.input_string,
+            func_dict=hook.function_dict.copy(),
         )
-        h = get_public_or_private_hook(context, hook_type)
-    # TODO: Refactor this whole function so this is not repeated
-    #  Make it so hook is split right away and evaluated in one loop
-    elif isinstance(h, LazyBaseFunction):
-        h = create_function_model(
+    elif isinstance(hook, LazyImportHook):
+        import_with_fallback_install(
             context=context,
-            func_name=hook_type,
-            func_dict=h.function_dict.copy(),
+            mod_name=hook.mod_name,
+            path=hook.hooks_path,
         )
+        hook = get_public_or_private_hook(context=context, hook_type=hook.hook_type)
 
-    return h
-
-
-def evaluate_for(hook_dict: dict, Hook: ModelMetaclass, context: 'Context'):
-    """Run the parse_hook function in a loop and return a list of outputs."""
-    loop_targets = render_variable(context, wrap_jinja_braces(hook_dict['for']))
-
-    if len(loop_targets) == 0:
-        return
-
-    hook_dict.pop('for')
-
-    # Need add an empty list in the value so we have something to append to
-    if 'merge' not in hook_dict:
-        target_context, key_path = get_target_and_key(context)
-        nested_set(target_context, key_path, [])
-    elif not hook_dict['merge']:
-        target_context, key_path = get_target_and_key(context)
-        # If we are merging into a list / dict, we don't want init a list
-        nested_set(target_context, key_path, [])
-
-    # Account for nested contexts and justify the new keys based on the key path within
-    #  blocks by trimming the key_path_block from the key_path.
-    if len(context.key_path_block) != 0:
-        tmp_key_path = context.key_path[
-            len(context.key_path_block) - len(context.key_path) :
-        ]  # noqa
-        if context.temporary_context is None:
-            context.temporary_context = {} if isinstance(tmp_key_path[0], str) else []
-        tmp_key_path = [i for i in tmp_key_path if i not in ('->', '_>')]
-        nested_set(context.temporary_context, tmp_key_path, [])
-
-    for i, l in (
-        enumerate(loop_targets)
-        if not render_variable(context, hook_dict.get('reverse', None))
-        else reversed(list(enumerate(loop_targets)))
-    ):
-        if context.existing_context is None:
-            context.existing_context = {}
-        # Create temporary variables in the context to be used in the loop.
-        context.existing_context.update({'index': i, 'item': l})
-        # Append the index to the keypath
-        context.key_path.append(encode_list_index(i))
-
-        # Reparse the hook with the new temp vars in place
-        parse_hook(hook_dict.copy(), Hook, context, append_hook_value=True)
-        context.key_path.pop()
+    # Handle args
+    for n, arg in enumerate(args):
+        # If help and last arg
+        if arg == 'help' and n == len(args):
+            run_help(context, hook)
+
+        # When arg inputs are not hashable then they are actual arguments which will be
+        # consumed later
+        elif isinstance(arg, (list, dict)):
+            # TODO: Check how this logic works with `args` condition below which works
+            #  for bypassing the processing of args for later logic
+            pass
 
-    # Remove temp variables
-    try:
-        context.existing_context.pop('item')
-        context.existing_context.pop('index')
-    except KeyError:
-        pass
+        # If arg in methods, compile hook
+        elif arg in hook.__fields__ and hook.__fields__[arg].type_ == Callable:
+            method = hook.__fields__[arg].default
+            # Update method with values from base class so that fields can be inherited
+            # from the base hook. function_fields is a list of those fields that aren't
+            # methods / special vars (ie args, return, etc).
+            for i in hook.__fields__['function_fields'].default:
+                # Base method should not override child.
+                if i not in method.function_dict:
+                    method.function_dict[i] = hook.__fields__['function_dict'].default[
+                        i
+                    ]
+                    if method.function_fields is None:
+                        method.function_fields = []
+                    method.function_fields.append(i)
 
+            # Methods are of type LazyBaseFunction which need to have the base
+            # instantiated before getting the hook. Allows nested methods for functions.
+            # if isinstance(method, LazyBaseFunction):
+            method = create_function_model(
+                context=context,
+                func_name=arg,
+                func_dict=method.function_dict.copy(),
+            )
+            # args = args[1:]
+            args.pop(0)
+            hook = method
+
+            if len(args) != 0:
+                return enrich_hook(
+                    context=context, hook=method, args=args, kwargs=kwargs
+                )
+        elif 'args' in hook.__fields__:
+            # The hook takes positional args
+            pass
+        else:
+            raise exceptions.UnknownInputArgumentException(
+                f"Unknown arg supplied `{arg}`",
+                context=context,
+            )
 
-def evaluate_if(hook_dict: dict, context: 'Context', append_hook_value: bool) -> bool:
-    """Evaluate the if/when condition and return bool."""
-    if hook_dict.get('when', None) is not None:
-        result = render_variable(context, wrap_jinja_braces(hook_dict['when']))
-        hook_dict.pop('when')
-        return result
-    if hook_dict.get('for', None) is not None and not append_hook_value:
-        # We qualify `if` conditions within for loop logic
-        return True
-    if hook_dict.get('if', None) is None:
-        return True
+    # Handle kwargs
+    for k, v in kwargs.items():
+        if k == 'args':
+            # TODO: I thought this would work
+            # args.append(v)
+            # But just passing works. Reason is the above duplicates the arg. No idea...
+            pass
+        elif k == 'kwargs':
+            pass
+        elif k in hook.__fields__:
+            # TODO: consolidate with `update_hook_with_kwargs_and_flags` - same same
+            if hook.__fields__[k].type_ == bool:
+                # Handle flags where default is true
+                if hook.__fields__[k].default:
+                    hook.__fields__[k].default = False
+                else:
+                    hook.__fields__[k].default = True
+            else:
+                hook.__fields__[k].default = v
 
-    return render_variable(context, wrap_jinja_braces(hook_dict['if']))
+    return hook
 
 
 def merge_block_output(
     hook_output_value: Any,
     context: Context,
     append_hook_value: bool = False,
 ):
@@ -246,14 +224,15 @@
     """
     if append_hook_value:
         # TODO: https://github.com/sudoblockio/tackle/issues/66
         #  Allow merging into lists
         if isinstance(context.key_path_block[-1], bytes):
             # An exception maybe needed here or this error is snubbed.
             pass
+        # set_key(context=context, value=hook_output_value)
         raise exceptions.AppendMergeException(
             "Can't merge from for loop.", context=context
         ) from None
 
     # 66 - Should qualify dict here
     target_context, key_path = get_target_and_key(context)
     indexed_block_output = nested_get(element=hook_output_value, keys=key_path)
@@ -278,25 +257,33 @@
         key_path = context.key_path[:-2] + [context.key_path[-1]]
     else:
         # Compact key
         key_path = context.key_path[:-1] + [context.key_path[-1][-2:]]
 
     if append_hook_value:
         if isinstance(key_path[-3], bytes):
-            set_key(context=context, value=hook_output_value, key_path=key_path[:-1])
+            # We are merging into a list so we need to keep track of the starting
+            # index from which we are merging into, the incremented position.
+            incremented_position = encode_list_index(
+                decode_list_index(key_path[-3]) + decode_list_index(key_path[-1])
+            )
+            tmp_key_path = key_path[:-3] + [incremented_position] + [key_path[-2]]
+            set_key(context=context, value=hook_output_value, key_path=tmp_key_path)
         elif isinstance(hook_output_value, (str, int, float, bool)):
             raise exceptions.AppendMergeException(
                 "Can't merge str/int/float/bool into dict from for loop.",
                 context=context,
             ) from None
+        elif isinstance(hook_output_value, dict):
+            # We are merging into a dict
+            for k, v in hook_output_value.items():
+                tmp_key_path = key_path[:-3] + [key_path[-2]] + [k]
+                set_key(context=context, value=v, key_path=tmp_key_path)
         else:
-            # TODO: This needs fixing for merging from loop into dict
-            #  https://github.com/robcxyz/tackle/issues/107
-            tmp_key_path = key_path[:-3] + [key_path[-2]]
-            set_key(context=context, value=hook_output_value, key_path=tmp_key_path)
+            raise NotImplementedError("Please raise issue with example if seeing this.")
         return
 
     # Can't merge into top level keys without merging k/v individually
     if len(key_path) == 1:
         # This is only valid for dict output
         if isinstance(hook_output_value, (dict, OrderedDict)):
             for k, v in hook_output_value.items():
@@ -310,30 +297,35 @@
             for k, v in hook_output_value.items():
                 set_key(context=context, value=v, key_path=key_path + [k])
         else:
             set_key(context=context, value=hook_output_value, key_path=key_path)
 
 
 def run_hook_in_dir(hook: Type[BaseHook]) -> Any:
+    """Run the `exec` method in a dir is `chdir` is specified."""
     if hook.chdir:
         path = os.path.abspath(os.path.expanduser(hook.chdir))
         if os.path.isdir(path):
             # Use contextlib to switch dirs
             with work_in(os.path.abspath(os.path.expanduser(hook.chdir))):
-                return hook.exec()
+                return hook.exec()  # noqa
         else:
             raise exceptions.HookUnknownChdirException(
                 f"The specified path='{path}' to change to was not found.",
                 hook=hook,
             ) from None
     else:
-        return hook.exec()
+        return hook.exec()  # noqa
 
 
-def render_hook_vars(hook_dict: dict, Hook: ModelMetaclass, context: 'Context'):
+def render_hook_vars(
+    context: 'Context',
+    hook_dict: dict,
+    Hook: ModelMetaclass,
+):
     """Render the hook variables."""
     for key, value in list(hook_dict.items()):
         if key not in Hook.__fields__ and key not in BASE_METHODS:
             # If the hook has a `kwargs` field, then map it to that field.
             if Hook.__fields__['kwargs'].default is not None:
                 default_kwargs = Hook.__fields__['kwargs'].default
                 if default_kwargs not in hook_dict:
@@ -382,20 +374,24 @@
             elif ('{{' in value and '}}' in value) or ('{%' in value and '%}'):
                 hook_dict[key] = render_variable(context, value)
 
         elif isinstance(value, (list, dict)):
             hook_dict[key] = render_variable(context, value)
 
 
-def parse_sub_context(context: 'Context', hook_dict: dict, target: str):
+def parse_sub_context(
+    context: 'Context',
+    hook_dict: dict,
+    target: str,
+):
     """
     Reparse a subcontext as in the case with `else` and `except` where you have to
-    handle the negative side of the either `if` or `try`. Works on both looped and
-    normal runs by checking the last item in the key path. Then overwrites the input
-    with a new context.
+     handle the negative side of the either `if` or `try`. Works on both looped and
+     normal runs by checking the last item in the key path. Then overwrites the input
+     with a new context.
     """
     hook_target = hook_dict[target]
     if isinstance(hook_target, str):
         set_key(
             context=context,
             value=render_variable(context, hook_dict[target]),
         )
@@ -419,149 +415,289 @@
         )
         updated_item = [
             hook_dict[target] if i == decode_list_index(context.key_path[-1]) else None
             for i in range(decode_list_index(context.key_path[-1]) + 1)
         ]
         # TODO: Figure out wtf is going on here...
         input_dict[indexed_key_path[-3]] = updated_item
-        walk_sync(
+        walk_element(
             context,
             element=input_dict[indexed_key_path[-3]][
                 decode_list_index(context.key_path[-1])
             ],
         )
 
     else:
         input_dict = nested_get(
             element=context.input_context,
             keys=indexed_key_path[:-2],
         )
         arrow = context.key_path[-1]
         input_dict[indexed_key_path[-2]] = {arrow: 'block', 'items': hook_dict[target]}
-        walk_sync(context, element=input_dict[indexed_key_path[-2]])
+        walk_element(context, element=input_dict[indexed_key_path[-2]])
 
 
-def parse_hook(
-    hook_dict, Hook: ModelMetaclass, context: 'Context', append_hook_value: bool = None
+def new_hook(
+    context: 'Context',
+    hook_dict: dict,
+    Hook: ModelMetaclass,
 ):
-    """Parse input dict for loop and when logic and calls hooks."""
-    if evaluate_if(hook_dict, context, append_hook_value):
+    """Create a new instantiated hook."""
+    # TODO: WIP - https://github.com/sudoblockio/tackle/issues/104
+    tmp_no_input = None if 'no_input' not in hook_dict else hook_dict.pop('no_input')
+
+    skip_output = Hook.__fields__['skip_output']  # Use later
+    try:
+        hook = Hook(
+            **hook_dict,
+            no_input=context.no_input if tmp_no_input is None else tmp_no_input,
+            temporary_context={} if skip_output.default else context.temporary_context,
+            key_path=context.key_path,
+            key_path_block=context.key_path_block,
+            input_context=context.input_context,
+            public_context=context.public_context,
+            private_context=context.private_context,
+            existing_context=context.existing_context,
+            calling_directory=context.calling_directory,
+            current_file=context.input_file,
+            calling_file=context.calling_file,
+            public_hooks=context.public_hooks,
+            private_hooks=context.private_hooks,
+            verbose=context.verbose,
+            env_=context.env_,
+            is_hook_call=True,
+            override_context=context.override_context,
+        )
+    except TypeError as e:
+        # TODO: Improve -> This is an error when we have multiple of the same
+        #  base attribute. Should not conflict in the future when we do
+        #  composition on the context but for now, catching common error.
+        # TODO: WIP - https://github.com/sudoblockio/tackle/issues/104
+        raise exceptions.UnknownInputArgumentException(
+            str(e) + " - Can't assign duplicate base fields.", context=context
+        ) from None
 
-        if 'for' in hook_dict:
-            # This runs the current function in a loop with `append_hook_value` set so
-            # that keys are appended in the loop.
-            evaluate_for(hook_dict, Hook, context)
+    except ValidationError as e:
+        # Handle any try / except logic
+        if 'try' in hook_dict and hook_dict['try']:
+            if 'except' in hook_dict and hook_dict['except']:
+                parse_sub_context(context, hook_dict, target='except')
             return
 
-        else:
-            # Render the remaining hook variables
-            render_hook_vars(hook_dict, Hook, context)
+        msg = str(e)
+        if Hook.identifier.startswith('tackle.providers'):
+            id_list = Hook.identifier.split('.')
+            provider_doc_url_str = id_list[2].title()
+            # Replace the validated object name (ex PrintHook) with the
+            # hook_type field that users would more easily know.
+            msg = msg.replace(id_list[-1], f"{hook_dict['hook_type']} hook")
+
+            msg += (
+                f"\n Check the docs for more information on the hook -> "
+                f"https://sudoblockio.github.io/tackle/providers/"
+                f"{provider_doc_url_str}/{hook_dict['hook_type']}/"
+            )
+        raise exceptions.HookParseException(str(msg), context=context) from None
+    return hook
+
 
-            # TODO: WIP - https://github.com/sudoblockio/tackle/issues/104
-            tmp_no_input = (
-                None if 'no_input' not in hook_dict else hook_dict.pop('no_input')
+def update_hook_with_kwargs_field(context: 'Context', hook_dict: dict):
+    """
+    In order to facilitate instantiating objects with dicts, a `kwargs` key can be used
+     to load the object. For instance `->: a_hook --kwargs a_dict`
+    """
+    hook_kwargs = hook_dict.pop('kwargs')
+    if isinstance(hook_kwargs, dict):
+        hook_dict.update(hook_kwargs)
+    elif isinstance(hook_kwargs, str):
+        try:
+            hook_dict.update(
+                render_variable(context=context, raw=wrap_jinja_braces(hook_kwargs))
             )
-            try:
-                hook = Hook(
-                    **hook_dict,
-                    input_context=context.input_context,
-                    public_context=context.public_context,
-                    private_context=context.private_context,
-                    temporary_context=context.temporary_context,
-                    existing_context=context.existing_context,
-                    no_input=context.no_input if tmp_no_input is None else tmp_no_input,
-                    calling_directory=context.calling_directory,
-                    calling_file=context.calling_file,
-                    public_hooks=context.public_hooks,
-                    private_hooks=context.private_hooks,
-                    key_path=context.key_path,
-                    verbose=context.verbose,
-                    env_=context.env_,
-                    is_hook_call=True,
-                    override_context=context.override_context,
-                )
-            except TypeError as e:
-                # TODO: Improve -> This is an error when we have multiple of the same
-                #  base attribute. Should not conflict in the future when we do
-                #  composition on the context but for now, catching common error.
-                # TODO: WIP - https://github.com/sudoblockio/tackle/issues/104
-                raise exceptions.UnknownInputArgumentException(
-                    str(e) + " - Can't assign duplicate base fields.", context=context
-                ) from None
+        except ValueError:
+            raise exceptions.UnknownArgumentException(
+                "The parameter `kwargs` should be either a map or a string "
+                "reference to a map.",
+                context=context,
+            ) from None
+    else:
+        raise exceptions.UnknownArgumentException(
+            "The parameter `kwargs` should be either a map or a string reference "
+            "to a map.",
+            context=context,
+        ) from None
 
-            except ValidationError as e:
-                # Handle any try / except logic
-                if 'try' in hook_dict and hook_dict['try']:
-                    if 'except' in hook_dict and hook_dict['except']:
-                        parse_sub_context(context, hook_dict, target='except')
-                    return
-
-                msg = str(e)
-                if Hook.identifier.startswith('tackle.providers'):
-                    id_list = Hook.identifier.split('.')
-                    provider_doc_url_str = id_list[2].title()
-                    # Replace the validated object name (ex PrintHook) with the
-                    # hook_type field that users would more easily know.
-                    msg = msg.replace(id_list[-1], f"{hook_dict['hook_type']} hook")
-
-                    msg += (
-                        f"\n Check the docs for more information on the hook -> "
-                        f"https://sudoblockio.github.io/tackle/providers/"
-                        f"{provider_doc_url_str}/{hook_dict['hook_type']}/"
-                    )
-                raise exceptions.HookParseException(str(msg), context=context) from None
 
-            # Main exec logic
-            if hook.try_:
-                try:
-                    hook_output_value = run_hook_in_dir(hook)
-                except Exception as e:
-                    if hook.verbose:
-                        print(e)
-                    if hook.except_:
-                        parse_sub_context(context, hook_dict, target='except')
-                    return
-            else:
-                # Normal hook run
-                hook_output_value = run_hook_in_dir(hook)
+def parse_hook_execute(
+    context: 'Context',
+    hook_dict: dict,
+    Hook: ModelMetaclass,
+    append_hook_value: bool = None,
+):
+    """Parse the remaining arguments such as try/except and merge"""
+    if 'kwargs' in hook_dict:
+        update_hook_with_kwargs_field(context=context, hook_dict=hook_dict)
 
-            if hook.skip_output:
-                if hook.merge:
-                    merge_block_output(
-                        hook_output_value=hook_output_value,
-                        context=context,
-                        append_hook_value=append_hook_value,
-                    )
-                return
-            elif hook.merge:
-                merge_output(
-                    hook_output_value=hook_output_value,
-                    context=context,
-                    append_hook_value=append_hook_value,
-                )
-            else:
-                set_key(
-                    context=context,
-                    value=hook_output_value,
-                )
+    # Render the remaining hook variables
+    render_hook_vars(context=context, hook_dict=hook_dict, Hook=Hook)
+
+    # Instantiate the hook
+    hook = new_hook(context=context, hook_dict=hook_dict, Hook=Hook)
+    if hook is None:
+        return
+
+    # Main exec logic
+    if hook.try_:
+        try:
+            hook_output_value = run_hook_in_dir(hook)
+        except Exception as e:
+            if hook.verbose:
+                print(e)
+            if hook.except_:
+                parse_sub_context(context=context, hook_dict=hook_dict, target='except')
+            return
+    else:
+        # Normal hook run
+        hook_output_value = run_hook_in_dir(hook)
 
+    if hook.skip_output:
+        # hook property that is only true for `block`/`match` hooks which write to the
+        # contexts themselves, thus their output is normally skipped except for merges.
+        if hook.merge:
+            # In this case we take the public context and overwrite the current context
+            # with the output indexed back one key.
+            merge_block_output(
+                hook_output_value=hook_output_value,
+                context=context,
+                append_hook_value=append_hook_value,
+            )
+        elif context.temporary_context is not None:
+            # Write the indexed output to the `temporary_context` as it was only written
+            # to the `public_context` and not maintained between items in a list
+            if not isinstance(context.key_path[-1], bytes):
+                get_set_temporary_context(context)
+
+    elif hook.merge:
+        merge_output(
+            hook_output_value=hook_output_value,
+            context=context,
+            append_hook_value=append_hook_value,
+        )
+    else:
+        set_key(
+            context=context,
+            value=hook_output_value,
+        )
+
+
+def evaluate_for(context: 'Context', hook_dict: dict, Hook: ModelMetaclass):
+    """Run the parse_hook function in a loop with temporary variables."""
+    loop_targets = render_variable(context, wrap_jinja_braces(hook_dict['for']))
+    if len(loop_targets) == 0:
+        return
+    hook_dict.pop('for')
+
+    # Need add an empty list in the value so we have something to append to except when
+    # we are merging.
+    if 'merge' not in hook_dict:
+        set_key(context=context, value=[])
+    elif not hook_dict['merge']:
+        set_key(context=context, value=[])
+
+    for i, l in (
+        enumerate(loop_targets)
+        if not render_variable(context, hook_dict.get('reverse', None))
+        else reversed(list(enumerate(loop_targets)))
+    ):
+        if context.existing_context is None:
+            context.existing_context = {}
+        # Create temporary variables in the context to be used in the loop.
+        context.existing_context.update({'index': i, 'item': l})
+        # Append the index to the keypath
+        context.key_path.append(encode_list_index(i))
+
+        # Reparse the hook with the new temp vars in place
+        parse_hook(
+            context=context,
+            hook_dict=hook_dict.copy(),
+            hook=Hook,
+            append_hook_value=True,
+        )
+        context.key_path.pop()
+
+    # Remove temp variables
+    try:
+        context.existing_context.pop('item')
+        context.existing_context.pop('index')
+    except KeyError:
+        pass
+
+
+def parse_hook_loop(
+    context: 'Context',
+    hook_dict: dict,
+    hook: ModelMetaclass,
+    append_hook_value: bool = None,
+):
+    if 'for' in hook_dict:
+        # This runs the current function in a loop with `append_hook_value` set so
+        # that keys are appended in the loop.
+        evaluate_for(context, hook_dict, hook)
+    else:
+        parse_hook_execute(
+            context=context,
+            hook_dict=hook_dict,
+            Hook=hook,
+            append_hook_value=append_hook_value,
+        )
+
+
+def evaluate_if(hook_dict: dict, context: 'Context', append_hook_value: bool) -> bool:
+    """Evaluate the if/when condition and return bool."""
+    if hook_dict.get('when', None) is not None:
+        result = render_variable(context, wrap_jinja_braces(hook_dict['when']))
+        hook_dict.pop('when')
+        return result
+    if hook_dict.get('for', None) is not None and not append_hook_value:
+        # We qualify `if` conditions within for loop logic
+        return True
+    if hook_dict.get('if', None) is None:
+        return True
+
+    return render_variable(context, wrap_jinja_braces(hook_dict['if']))
+
+
+def parse_hook(
+    context: 'Context',
+    hook_dict: dict,
+    hook: ModelMetaclass,
+    append_hook_value: bool = None,
+):
+    """Parse input dict for loop and when logic and calls hooks."""
+    if evaluate_if(hook_dict, context, append_hook_value):
+        parse_hook_loop(
+            context=context,
+            hook_dict=hook_dict,
+            hook=hook,
+            append_hook_value=append_hook_value,
+        )
     elif 'else' in hook_dict:
         parse_sub_context(context, hook_dict, target='else')
 
 
 def evaluate_args(
     args: list,
     hook_dict: dict,
     Hook: ModelMetaclass,  # noqa
     context: 'BaseContext' = None,  # For error handling
 ):
     """
     Associate hook arguments provided in the call with hook attributes. Parses the
-    hook's `args` attribute to know how to map arguments are mapped to where and
-    deal with rendering by default.
+     hook's `args` attribute to know how to map arguments are mapped to where and
+     deal with rendering by default.
 
     TODO: This needs to be re-thought. Right now we parse the inputs without regard
      for the types of the argument mapping. What could be better is if we know the types
      of the arg mapping ahead of time and then try to assemble the most logical mapping
      afterwards. So if the mapping consists of a [str, list], then if the first
      args are strs then we can ignore the list part. Right now it would just join all
      the strings together if they are part of last arg mapping.
@@ -639,15 +775,15 @@
                     raise exceptions.UnknownArgumentException(
                         f"The hook {hook_dict['hook_type']} takes the following indexed"
                         f"arguments -> {hook_args} which does not map to the arg {v}.",
                         context=context,
                     ) from None
 
 
-def run_hook(context: 'Context'):
+def run_hook_at_key_path(context: 'Context'):
     """
     Run the hook by qualifying the input argument and matching the input params with the
      hook's `_args` which are then overlayed into a hook kwargs. Also interprets
      special cases where you have a string or list input of renderable variables.
     """
     if isinstance(context.input_string, str):
         args, kwargs, flags = unpack_args_kwargs_string(context.input_string)
@@ -666,92 +802,80 @@
             set_key(
                 context=context,
                 value=render_variable(context, v),
                 key_path=context.key_path + [encode_list_index(i)],
             )
         return
 
-    # Look up the hook from the imported providers
-    Hook = get_hook(first_arg, context)
-
     if context.key_path[-1] in ('->', '_>'):
         # We have an expanded or mixed (with args) hook expression and so there will be
         # additional properties in adjacent keys. Trim key_path_block for blocks
         try:
             hook_dict = nested_get(
                 context.input_context,
-                smush_key_path(context.key_path[:-1][len(context.key_path_block) :]),
+                remove_arrows_from_key_path(
+                    context.key_path[:-1][len(context.key_path_block) :]
+                ),
             ).copy()
         except KeyError as e:
             raise exceptions.UnknownHookTypeException(
                 f"Key: {e} - Unknown", context=context
             ) from None
         # Need to replace arrow keys as for the time being (pydantic 1.8.2) - multiple
         # aliases for the same field (type) can't be specified so doing this hack
         if '->' in hook_dict:
             hook_dict.pop('->')
         else:
             hook_dict.pop('_>')
     else:
         # Hook is a compact expression - Can only be a string
         hook_dict = {}
-    hook_dict['hook_type'] = first_arg
 
+    # Look up the hook from the imported providers
+    hook = get_hook(
+        context=context,
+        hook_type=first_arg,
+        args=args,
+        kwargs=kwargs,
+    )
+    if hook is None:
+        exceptions.raise_unknown_hook(context, first_arg)
+
+    hook_dict['hook_type'] = hook.__fields__['hook_type'].default
+
+    # `args` can be a kwarg (ie `tackle --args foo`) and is manually added to args var
     if 'args' in kwargs:
         # For calling hooks, you can manually provide the hook with args. Useful for
         # creating declarative hooks that
         hook_args = kwargs.pop('args')
         if isinstance(hook_args, list):
             args += hook_args
         else:
             args += [hook_args]
 
     # Associate hook arguments provided in the call with hook attributes
-    evaluate_args(args=args, hook_dict=hook_dict, Hook=Hook, context=context)
+    evaluate_args(args=args, hook_dict=hook_dict, Hook=hook, context=context)
     # Add any kwargs
     for k, v in kwargs.items():
         hook_dict[k] = v
     for i in flags:
         hook_dict[i] = True
-
-    if 'kwargs' in hook_dict:
-        hook_kwargs = hook_dict.pop('kwargs')
-        if isinstance(hook_kwargs, dict):
-            hook_dict.update(hook_kwargs)
-        elif isinstance(hook_kwargs, str):
-            try:
-                hook_dict.update(
-                    render_variable(context=context, raw=wrap_jinja_braces(hook_kwargs))
-                )
-            except ValueError:
-                error_msg = (
-                    "The parameter `kwargs` should be either a map or a string "
-                    "reference to a map."
-                )
-                raise exceptions.UnknownArgumentException(
-                    error_msg, context=context
-                ) from None
-        else:
-            error_msg = (
-                "The parameter `kwargs` should be either a map or a string reference "
-                "to a map."
-            )
-            raise exceptions.UnknownArgumentException(
-                error_msg, context=context
-            ) from None
-
     # Cleanup any unquoted fields -> common mistake that is hard to debug producing a
     #  nested dict that breaks parsing / hook calls. Ex foo: {{bar}} -> foo: "{{bar}}"
     cleanup_unquoted_strings(hook_dict)
 
     # Main parser
-    parse_hook(hook_dict, Hook, context)
+    parse_hook(
+        context=context,
+        hook_dict=hook_dict,
+        hook=hook,
+    )
 
 
-def walk_sync(context: 'Context', element):
+def walk_element(context: 'Context', element):
     """
     Traverse an object looking for hook calls and running those hooks. Here we are
      keeping track of which keys are traversed in a list called `key_path` with strings
      as dict keys and byte encoded integers for list indexes.
     """
     if len(context.key_path) != 0:
         # Handle compact expressions - ie key->: hook_type args
@@ -764,22 +888,22 @@
 
     if isinstance(element, dict):
         # Handle expanded expressions - ie key:\n  ->: hook_type args
         if '->' in element.keys():
             # Public hook calls
             context.key_path.append('->')
             context.input_string = element['->']
-            run_hook(context)
+            run_hook_at_key_path(context)
             context.key_path.pop()
             return
         elif '_>' in element.keys():
             # Private hook calls
             context.key_path.append('_>')
             context.input_string = element['_>']
-            run_hook(context)
+            run_hook_at_key_path(context)
             context.key_path.pop()
             return
         elif element == {}:
             set_key(context=context, value={})
             return
 
         for k, v in element.copy().items():
@@ -817,29 +941,29 @@
                 #  then we have an empty hook which will cause an ambiguous
                 #  ValidationError for missing field
                 if 'items' not in value:
                     raise exceptions.EmptyBlockException(
                         "Empty block hook.", context=context
                     ) from None
 
-                walk_sync(context, value)
+                walk_element(context, value)
                 context.key_path.pop()
             else:
                 # Recurse
-                walk_sync(context, v)
+                walk_element(context, v)
                 context.key_path.pop()
     # Non-hook calls recurse through inputs
     elif isinstance(element, list):
         # Handle empty lists
         if len(element) == 0:
             set_key(context=context, value=element)
         else:
             for i, v in enumerate(element.copy()):
                 context.key_path.append(encode_list_index(i))
-                walk_sync(context, v)
+                walk_element(context, v)
                 context.key_path.pop()
     else:
         set_key(context=context, value=element)
 
 
 def update_input_context(input_dict: dict, update_dict: dict) -> dict:
     """
@@ -876,17 +1000,17 @@
                 }
     return input_dict
 
 
 def update_hook_with_kwargs_and_flags(hook: ModelMetaclass, kwargs: dict) -> dict:
     """
     For consuming kwargs / flags, once the hook has been identified when calling hooks
-    via CLI actions, this function matches the kwargs / flags with the hook and returns
-    any unused kwargs / flags for use in the outer context. Note that flags are kwargs
-    as they have already been merged by now.
+     via CLI actions, this function matches the kwargs / flags with the hook and returns
+     any unused kwargs / flags for use in the outer context. Note that flags are kwargs
+     as they have already been merged by now.
     """
     for k, v in kwargs.copy().items():
         if k in hook.__fields__:
             if hook.__fields__[k].type_ == bool:
                 # Flags -> These are evaluated as the inverse of whatever is the default
                 if hook.__fields__[k].default:  # ie -> True
                     hook.__fields__[k].default = False
@@ -896,15 +1020,15 @@
                 # Kwargs
                 hook.__fields__[k].default = v
             hook.__fields__[k].required = False  # Otherwise will complain
             kwargs.pop(k)
     return kwargs
 
 
-def find_run_hook_method(
+def run_declarative_hook(
     context: 'Context', hook: ModelMetaclass, args: list, kwargs: dict
 ) -> Any:
     """
     Given a hook with args, find if the hook has methods and if it does not, apply the
      args to the hook based on the `args` field mapping. Calls the hook.
     """
     kwargs = update_hook_with_kwargs_and_flags(
@@ -920,55 +1044,89 @@
         unknown_args = ' '.join([f"{k}={v}" for k, v in kwargs.items()])
         raise exceptions.UnknownInputArgumentException(
             f"The args {unknown_args} not recognized when running the hook/method "
             f"{hook_name}. Exiting.",
             context=context,
         ) from None
 
+    if isinstance(hook, LazyBaseFunction):
+        hook = create_function_model(
+            context=context,
+            func_name=context.input_string,
+            func_dict=hook.function_dict.copy(),
+        )
+
+    # Handle args
     arg_dict = {}
     num_popped = 0
     for i, arg in enumerate(args.copy()):
+        # For running hooks in tackle files (ie not in `hooks` dir), we run this logic
+        # as the hook is already compiled.
         if arg in hook.__fields__ and hook.__fields__[arg].type_ == Callable:
             # Consume the args
             args.pop(i - num_popped)
             num_popped += 1
 
             # Gather the function's dict so it can be compiled into a runnable hook
             func_dict = hook.__fields__[arg].default.function_dict.copy()
 
             # Add inheritance from base function fields
             for j in hook.__fields__['function_fields'].default:
                 # Base method should not override child.
                 if j not in func_dict:
                     func_dict[j] = hook.__fields__[j]
 
-            new_hook = create_function_model(
+            hook = create_function_model(
                 context=context,
                 func_name=hook.__fields__[arg].name,
                 func_dict=func_dict,
             )
+        elif isinstance(hook, LazyBaseFunction) and (
+            arg + '<-' in hook.function_dict or arg + '<_' in hook.function_dict
+        ):
+            # Consume the args
+            args.pop(i - num_popped)
+            num_popped += 1
 
-            hook = new_hook
+            # Gather the function's dict so it can be compiled into a runnable hook
+            if arg + '<-' in hook.function_dict:
+                func_dict = hook.function_dict[arg + '<-']
+            else:
+                func_dict = hook.function_dict[arg + '<_']
+
+            # Add inheritance from base function fields
+            if hook.function_fields is not None:
+                for j in hook.function_fields:
+                    # Base method should not override child.
+                    if j not in func_dict:
+                        func_dict[j] = hook.function_dict[j]
+            hook = create_function_model(
+                context=context,
+                func_name=arg,
+                func_dict=func_dict,
+            )
 
         elif arg == 'help':
             # Exit 0
             run_help(context=context, hook=hook)
-        # elif 'args' not in hook.__fields__:
+
         elif hook.__fields__['args'].default == []:  # noqa
+            # Throw error as we have nothing to map the arg to
             hook_name = hook.identifier.split('.')[-1]
             if hook_name == '':
                 msg = "default hook"
             else:
                 msg = f"hook='{hook_name}'"
             raise exceptions.UnknownInputArgumentException(
                 f"The {msg} was supplied the arg='{arg}' and does not take any "
                 "arguments. Exiting.",
                 context=context,
             ) from None
 
+    # Handle the `args` field which maps to args
     if 'args' in hook.__fields__:
         evaluate_args(args, arg_dict, Hook=hook, context=context)
 
     try:
         Hook = hook(**kwargs, **arg_dict)
     except ValidationError as e:
         raise exceptions.MalformedFunctionFieldException(
@@ -982,14 +1140,16 @@
 def raise_if_args_exist(
     context: 'Context', hook: ModelMetaclass, args: list, kwargs: dict, flags: list
 ):
     """
     Raise an error if not all the args / kwargs / flags have been consumed which would
      mean the user supplied extra vars and should be yelled at.
     """
+    # TODO: Refactor into own file
+
     msgs = []
     if len(args) != 0:
         msgs.append(f"args {', '.join(args)}")
     if len(kwargs) != 0:
         missing_kwargs = ', '.join([f"{k}={v}" for k, v in kwargs.items()])
         msgs.append(f"kwargs {missing_kwargs}")
     if len(flags) != 0:
@@ -1010,15 +1170,17 @@
             raise exceptions.UnknownSourceException(
                 f"Could not find source = {args[0]} or as key / hook in parent tackle "
                 f"file.",
                 context=context,
             ) from None
 
 
-def run_source(context: 'Context', args: list, kwargs: dict, flags: list) -> Optional:
+def parse_source_args(
+    context: 'Context', args: list, kwargs: dict, flags: list
+) -> Optional:
     """
     Process global args/kwargs/flags based on if the args relate to the default hook or
      some public hook (usually declarative). Once the hook has been identified, the
      args/kwargs/flags are consumed and if there are any args left, an error is raised.
     """
     # Tackle is called both through the CLI and as a package and so to preserve args /
     # kwargs we merge them here.
@@ -1036,14 +1198,15 @@
         #  the inverse of what the default is
         kwargs.update({i: True for i in context.global_flags})
         context.global_flags = None
 
     # For CLI calls, this logic lines up the args with methods / method args and
     # integrates the kwargs / flags into the call
     if len(args) == 0 and context.default_hook:  # Default hook (no args)
+        # TODO: Refactor into own file
         # Add kwargs / flags (already merged into kwargs) to default hook
         kwargs = update_hook_with_kwargs_and_flags(
             hook=context.default_hook,
             kwargs=kwargs,
         )
         # Run the default hook as there are no args. The outer context is then parsed
         #  as otherwise it would be unreachable.
@@ -1068,37 +1231,38 @@
             flags=flags,
         )
     elif len(args) == 1 and args[0] == 'help' and context.default_hook is not None:
         run_help(context=context, hook=context.default_hook)
     elif len(args) == 1 and args[0] == 'help':
         run_help(context=context)
     elif len(args) != 0:  # With args
+        # TODO: Refactor into own file
         # Prioritize public_hooks (ie non-default hook) because if the hook exists,
         # then we should consume the arg there instead of using the arg as an arg for
         # default hook because otherwise the public hook would be unreachable.
-        if args[0] in context.public_hooks:  #
+        if args[0] in context.public_hooks:
             # Search within the public hook for additional args that could be
             # interpreted as methods which always get priority over consuming the arg
             # as an arg within the hook itself.
             public_hook = args.pop(0)  # Consume arg
-            context.public_context = find_run_hook_method(
+            context.public_context = run_declarative_hook(
                 context=context,
                 hook=context.public_hooks[public_hook],
                 args=args,
                 kwargs=kwargs,
             )
             raise_if_args_exist(  # Raise if there are any args left
                 context=context,
                 hook=context.public_hooks[public_hook],
                 args=args,
                 kwargs=kwargs,
                 flags=flags,
             )
         elif context.default_hook:
-            context.public_context = find_run_hook_method(
+            context.public_context = run_declarative_hook(
                 context=context, hook=context.default_hook, args=args, kwargs=kwargs
             )
             raise_if_args_exist(  # Raise if there are any args left
                 context=context,
                 hook=context.default_hook,
                 args=args,
                 kwargs=kwargs,
@@ -1140,15 +1304,15 @@
                 # TODO improve -> Should give help by default?
                 f"Only functions are declared in {context.input_string} tackle file. Must"
                 f" provide an argument such as [] or run `tackle {context.input_string}"
                 f" help` to see more options.",
                 context=context,
             ) from None
     else:
-        walk_sync(context, context.input_context.copy())
+        walk_element(context, context.input_context.copy())
 
 
 def parse_tmp_context(context: Context, element: Any, existing_context: dict):
     """
     Parse an arbitrary element. Only used for declarative hook field defaults and in
      the `run_hook` hook in the tackle provider.
     """
@@ -1161,23 +1325,43 @@
         existing_context=existing_context,
         input_context=element,
         key_path=['->'],
         key_path_block=['->'],
         no_input=context.no_input,
         calling_directory=context.calling_directory,
         calling_file=context.calling_file,
+        # current_file=context.current_file,
         verbose=context.verbose,
         env_=context.env_,
         override_context=context.override_context,
     )
-    walk_sync(context=tmp_context, element=element)
+    walk_element(context=tmp_context, element=element)
 
     return tmp_context.public_context
 
 
+def get_complex_field(
+    field: Any,
+) -> Type:
+    """
+    Takes an input field such as `list[str]` which can include uncalled hooks and calls
+     those hooks before returning the  field. Works recursively to find nested hooks
+     within types.
+    """
+    if isinstance(field, list):
+        for i, v in enumerate(field):
+            field[i] = get_complex_field(v)
+    elif isinstance(field, dict):
+        for k, v in field.items():
+            field[k] = get_complex_field(v)
+    elif isinstance(field, BaseFunction):
+        field = field.exec()
+    return field
+
+
 def function_walk(
     self: 'Context',
     input_element: Union[list, dict],
     return_: Union[list, dict] = None,
 ) -> Any:
     """
     Walk an input_element for a function and either return the whole context or one or
@@ -1187,15 +1371,15 @@
     if input_element == {}:
         # If there is no `exec` method, input_element is {} so we infer that the
         # input fields are to be returned. This is useful if the user would like to
         # validate a dict easily with a function and is the only natural meaning of
         # a function call without an exec method.
         input_element = {}
         for i in self.function_fields:
-            input_element[i] = getattr(self, i)
+            input_element[i] = get_complex_field(getattr(self, i))
 
     if self.public_context:
         existing_context = self.public_context.copy()
         existing_context.update(self.existing_context)
     else:
         existing_context = {}
 
@@ -1210,69 +1394,211 @@
             existing_context.update(output)
             try:
                 input_element[i] = output[i]
             except KeyError:
                 raise exceptions.FunctionCallException(
                     f"Error parsing declarative hook field='{i}'. Must produce an "
                     f"output for the field's default.",
-                    function=self,
+                    function=self,  # noqa
                 ) from None
         else:
-            existing_context.update({i: getattr(self, i)})
+            # Otherwise just the value itself
+            existing_context.update({i: get_complex_field(getattr(self, i))})
 
     tmp_context = Context(
         public_hooks=self.public_hooks,
         private_hooks=self.private_hooks,
         existing_context=existing_context,
         public_context={},
         input_context=input_element,
         key_path=[],
         no_input=self.no_input,
         calling_directory=self.calling_directory,
         calling_file=self.calling_file,
         env_=self.env_,
         override_context=self.override_context,
     )
-    walk_sync(context=tmp_context, element=input_element.copy())
+    walk_element(context=tmp_context, element=input_element.copy())
 
     if return_:
         return_ = render_variable(tmp_context, return_)
         if isinstance(return_, str):
             if return_ in tmp_context.public_context:
                 return tmp_context.public_context[return_]
             else:
                 raise exceptions.FunctionCallException(
                     f"Return value '{return_}' is not found " f"in output.",
-                    function=self,
+                    function=self,  # noqa
                 ) from None
         elif isinstance(return_, list):
             if isinstance(tmp_context, list):
                 # TODO: This is not implemented (ie list outputs)
                 raise exceptions.FunctionCallException(
                     f"Can't have list return {return_} for " f"list output.",
-                    function=self,
+                    function=self,  # noqa
                 ) from None
             output = {}
             for i in return_:
                 # Can only return top level keys right now
                 if i in tmp_context.public_context:
                     output[i] = tmp_context.public_context[i]
                 else:
                     raise exceptions.FunctionCallException(
                         f"Return value '{i}' in return {return_} not found in output.",
-                        function=self,
+                        function=self,  # noqa
                     ) from None
             return tmp_context.public_context[return_]
         else:
             raise NotImplementedError(f"Return must be of list or string {return_}.")
     return tmp_context.public_context
 
 
+LITERAL_TYPES: set = {'str', 'int', 'float', 'bool', 'dict', 'list'}  # strings to match
+
+
+def parse_function_type(
+    context: Context,
+    type_str: str,
+    func_name: str,
+):
+    """
+    Parse the `type` field within a declarative hook and use recursion to parse the
+     string into real types.
+    """
+    type_str = type_str.strip()
+    # Check if it's a generic type with type arguments
+    if '[' in type_str:
+        # Strip the brackets. Base type will then have subtypes
+        base_type_str, type_args_str_raw = type_str.split('[', 1)
+        type_args_str = type_args_str_raw.rsplit(']', 1)[0]
+        # Get list of types separated by commas but not within brackets.
+        # ie `'dict[str, Base], Base'` -> `['dict[str, Base]', 'Base']`
+        type_args = [
+            parse_function_type(
+                context=context,
+                type_str=arg,
+                func_name=func_name,
+            )
+            for arg in re.split(r',(?![^[\]]*])', type_args_str)
+        ]
+        # Get base type
+        base_type = parse_function_type(
+            context=context,
+            type_str=base_type_str,
+            func_name=func_name,
+        )
+
+        if len(type_args) == 0:
+            return base_type
+        elif base_type == typing.Optional:
+            # Optional only takes a single arg
+            if len(type_args) == 1:
+                return base_type[type_args[0]]
+            else:
+                raise exceptions.MalformedFunctionFieldException(
+                    "The type `Optional` only takes one arg.",
+                    context=context,
+                    function_name=func_name,
+                ) from None
+        else:
+            return base_type[tuple(type_args)]
+
+    # Check if it's a generic type without type arguments
+    if hasattr(typing, type_str):
+        return getattr(typing, type_str)
+    elif type_str not in LITERAL_TYPES:
+        hook = get_public_or_private_hook(context=context, hook_type=type_str)
+        if hook is None:
+            try:
+                type_ = getattr(typing, type_str.title())
+            except AttributeError:
+                raise exceptions.MalformedFunctionFieldException(
+                    f"The type `{type_str}` is not recognized. Must be in python's "
+                    f"`typing` module.",
+                    context=context,
+                    function_name=func_name,
+                ) from None
+            return type_
+        elif isinstance(hook, LazyBaseFunction):
+            # We have a hook we need to build
+            return create_function_model(
+                context=context,
+                func_name=type_str,
+                func_dict=hook.function_dict.copy(),
+            )
+        else:
+            return hook
+    # Treat it as a plain name - Safe eval as already qualified as literal
+    return eval(type_str)
+
+
+def function_extends_merge_hook(
+    context: 'Context',
+    func_name: str,
+    func_dict: dict,
+    extends: str,
+):
+    base_hook = get_hook(
+        context=context,
+        hook_type=extends,
+        # TODO: this would change if allowing extends to get instantiated with
+        #  actual vars. Should be done when allowing dicts for extends.
+        args=[],
+        kwargs={},
+    )
+    if base_hook is None:
+        raise exceptions.MalformedFunctionFieldException(
+            f"In the declarative hook `{func_name}`, the 'extends' reference to "
+            f"`{extends}` can not be found.",
+            function_name=func_name,
+            context=context,
+        ) from None
+    return {**base_hook().function_dict, **func_dict}
+
+
+def function_extends(
+    context: 'Context',
+    func_name: str,
+    func_dict: dict,
+):
+    """
+    Implement the `extends` functionality which takes either a string reference or list
+     of string references to declarative hooks whose fields will be merged together.
+    """
+    extends = func_dict.pop('extends')
+    if isinstance(extends, str):
+        return function_extends_merge_hook(
+            context=context,
+            func_name=func_name,
+            func_dict=func_dict,
+            extends=extends,
+        )
+
+    elif isinstance(extends, list):
+        for i in extends:
+            if not isinstance(i, str):
+                break
+            return function_extends_merge_hook(
+                context=context,
+                func_name=func_name,
+                func_dict=func_dict,
+                extends=i,
+            )
+    raise exceptions.MalformedFunctionFieldException(
+        "The field `extends` can only be a string or list of string references to "
+        "hooks to merge together.",
+        context=context,
+        function_name=func_name,
+    ) from None
+
+
 def create_function_model(
-    context: 'Context', func_name: str, func_dict: dict
+    context: 'Context',
+    func_name: str,
+    func_dict: dict,
 ) -> Type[BaseFunction]:
     """Create a model from the function input dict."""
     if func_name.endswith(('<-', '<_')):
         func_name = func_name[:-2]
 
     if func_dict is None:
         raise exceptions.EmptyFunctionException(
@@ -1292,17 +1618,19 @@
     # Apply overrides to input fields
     for k, v in context.override_context.items():
         if k in func_dict:
             func_dict[k] = v
 
     # Implement inheritance
     if 'extends' in func_dict and func_dict['extends'] is not None:
-        base_hook = get_hook(func_dict['extends'], context)
-        func_dict = {**base_hook().function_dict, **func_dict}
-        func_dict.pop('extends')
+        func_dict = function_extends(
+            context=context,
+            func_name=func_name,
+            func_dict=func_dict,
+        )
 
     # Persisted with object for `extends`. Used later
     function_dict = func_dict.copy()
 
     # fmt: off
     # Validate raw input params against pydantic object where values will be used later
     exec_ = {}
@@ -1327,51 +1655,72 @@
         help=func_dict.pop('help') if 'help' in func_dict else None,
         # TODO: Build validators
         # validators_=func_dict.pop('validators') if 'validators' in func_dict else None,
     )
 
     # fmt: on
     new_func = {'hook_type': func_name, 'function_fields': []}
-    literals = ('str', 'int', 'float', 'bool', 'dict', 'list')  # strings to match
+
+    # First pass through the func_dict to parse out the methods
+    for k, v in func_dict.copy().items():
+        if k.endswith(('<-', '<_')):
+            # Implement method which is instantiated later in `enrich_hook`
+            new_func[k[:-2]] = (Callable, LazyBaseFunction(function_dict=v))
+            func_dict.pop(k)
+            continue
+
     # Create function fields from anything left over in the function dict
     for k, v in func_dict.items():
         if v is None:
             # TODO: Why skip? Would be ignored. Empty keys mean something right?
             continue
 
         if k.endswith(('->', '_>')):
             raise NotImplementedError
         elif k.endswith(('<-', '<_')):
-            # Implement method which is instantiated later in `get_hook`
+            # Implement method which is instantiated later in `enrich_hook`
             new_func[k[:-2]] = (Callable, LazyBaseFunction(function_dict=v))
             continue
 
         elif isinstance(v, dict):
-            if 'type' in v:
-                # TODO: Qualify type in enum -> Type
-                type_ = v['type']
-                if type_ not in literals:
+            if 'enum' in v:
+                if 'type' in v:
                     raise exceptions.MalformedFunctionFieldException(
-                        f"Function field {k} with type={v} unknown. Must be one of {','.join(literals)}",
+                        'Enums are implicitly typed.',
+                        context=context,
                         function_name=func_name,
+                    )
+                enum_type = enum.Enum(k, {i: i for i in v['enum']})
+                if 'default' in v:
+                    new_func[k] = (enum_type, v['default'])
+                else:
+                    new_func[k] = (enum_type, ...)
+            elif 'type' in v:
+                type_ = v['type']
+                if type_ in LITERAL_TYPES:
+                    parsed_type = locate(type_).__name__
+                else:
+                    parsed_type = parse_function_type(
                         context=context,
-                    ) from None
+                        type_str=type_,
+                        func_name=func_name,
+                    )
                 if 'description' in v:
                     v = dict(v)
                     v['description'] = v['description'].__repr__()
-                new_func[k] = (type_, Field(**v))
+                new_func[k] = (parsed_type, Field(**v))
             elif 'default' in v:
                 if isinstance(v['default'], dict) and '->' in v['default']:
                     # For hooks in the default fields.
                     new_func[k] = (Any, Field(**v))
                 else:
                     new_func[k] = (type(v['default']), Field(**v))
             else:
                 new_func[k] = (dict, v)
-        elif v in literals:
+        elif isinstance(v, str) and v in LITERAL_TYPES:
             new_func[k] = (locate(v).__name__, Field(...))
         elif isinstance(v, (str, int, float, bool)):
             new_func[k] = v
         elif isinstance(v, list):
             new_func[k] = (list, v)
         elif isinstance(v, ModelField):
             # Is encountered when inheritance is imposed and calling function methods
@@ -1432,17 +1781,21 @@
 
 def extract_functions(context: 'Context'):
     """
     Iterate through all the keys along baseline of tackle file and extract / compile
      all the keys that reference functions.
     """
     for k, v in context.input_context.copy().items():
-        if re.match(r'^[a-zA-Z0-9\_]*(<\-|<\_)$', k):
+        if re.match(r'^[a-zA-Z0-9\_]*(<\-|<\_)$', k):  # noqa
             # TODO: RM arrow and put in associated access modifier namespace
-            Function = create_function_model(context, k, v)
+            Function = create_function_model(
+                context=context,
+                func_name=k,
+                func_dict=v,
+            )
             function_name = k[:-2]
             arrow = k[-2:]
             if function_name == "":
                 # Function is the default hook
                 context.default_hook = Function
                 context.input_context.pop(k)
             elif arrow == '<-':  # public hook
@@ -1479,15 +1832,15 @@
     try:
         context.input_context = read_config_file(path)
     except FileNotFoundError:
         raise exceptions.UnknownSourceException(
             f"Could not find file in {path}.", context=context
         ) from None
     except ParserError as e:
-        raise exceptions.TackleFileInitialParsingException(e) from None
+        raise exceptions.TackleFileInitialParsingException(e) from None  # noqa
 
     if context.input_context is None:
         raise exceptions.EmptyTackleFileException(
             f"Tackle file found at {path} is empty.", context=context
         ) from None
 
     # Import the hooks and install requirements.txt if there is a ModuleNotFound error
@@ -1514,15 +1867,15 @@
 
     if context.directory:
         context.input_file = os.path.join(context.input_file, context.directory)
 
     extract_base_file(context)
 
 
-def update_source(context: 'Context'):
+def parse_source(context: 'Context'):
     """
     Locate the repository directory from a template reference. This is the main parser
     for determining the source of the context and calls the succeeding parsing
     functions. The parsing order has the following order of precedence.
 
     If the template wasn't given then use the file in that parent directory.
     If the template refers to a zip file or zip url, download / unzip as the context.
@@ -1580,8 +1933,8 @@
 
         args.insert(0, first_arg)
 
     # We always change directory into the source that is being called. Needs to be this
     # or would be very confusing if writing a provider to always refer to it's own path.
     with work_in(context.input_dir):
         # Main parsing logic
-        return run_source(context, args, kwargs, flags)
+        return parse_source_args(context, args, kwargs, flags)
```

### Comparing `tackle-0.4.9/tackle/providers/collections/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/collections/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/collections/hooks/distinct.py` & `tackle-0.5.0/tackle/providers/collections/hooks/distinct.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/collections/hooks/list_key.py` & `tackle-0.5.0/tackle/providers/collections/hooks/list_key.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/collections/hooks/map_to_list_key_values.py` & `tackle-0.5.0/tackle/providers/collections/hooks/map_to_list_key_values.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/collections/hooks/sort.py` & `tackle-0.5.0/tackle/providers/collections/hooks/sort.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/collections/tests/sort-in-place.yaml` & `tackle-0.5.0/tackle/providers/collections/tests/sort-in-place.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/collections/tests/test_provider_collections.py` & `tackle-0.5.0/tackle/providers/collections/tests/test_provider_collections.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/command/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/command/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/command/hooks/command.py` & `tackle-0.5.0/tackle/providers/command/hooks/command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/command/tests/test_provider_command.py` & `tackle-0.5.0/tackle/providers/command/tests/test_provider_command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/console/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/console/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/console/hooks/markdown.py` & `tackle-0.5.0/tackle/providers/console/hooks/markdown.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/console/hooks/prints.py` & `tackle-0.5.0/tackle/providers/console/hooks/prints.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/console/hooks/table.py` & `tackle-0.5.0/tackle/providers/console/hooks/table.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/context/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/append.py` & `tackle-0.5.0/tackle/providers/context/hooks/append.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/delete.py` & `tackle-0.5.0/tackle/providers/context/hooks/delete.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/get.py` & `tackle-0.5.0/tackle/providers/context/hooks/get.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/keys.py` & `tackle-0.5.0/tackle/providers/context/hooks/keys.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/pop.py` & `tackle-0.5.0/tackle/providers/context/hooks/pop.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/sets.py` & `tackle-0.5.0/tackle/providers/context/hooks/sets.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/update.py` & `tackle-0.5.0/tackle/providers/context/hooks/update.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/hooks/values.py` & `tackle-0.5.0/tackle/providers/context/hooks/values.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/tests/append-loop.yaml` & `tackle-0.5.0/tackle/providers/context/tests/append-loop.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/tests/test_provider_context.py` & `tackle-0.5.0/tackle/providers/context/tests/test_provider_context.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/tests/update-2.yaml` & `tackle-0.5.0/tackle/providers/context/tests/update-2.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/context/tests/update.yaml` & `tackle-0.5.0/tackle/providers/context/tests/update.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/datetime/hooks/dates.py` & `tackle-0.5.0/tackle/providers/datetime/hooks/dates.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/environment/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/environment/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/environment/hooks/envs.py` & `tackle-0.5.0/tackle/providers/environment/hooks/envs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/environment/tests/test_provider_envs.py` & `tackle-0.5.0/tackle/providers/environment/tests/test_provider_envs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/files/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/files/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/files/hooks/file.py` & `tackle-0.5.0/tackle/providers/files/hooks/file.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/files/hooks/zips.py` & `tackle-0.5.0/tackle/providers/files/hooks/zips.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/files/tests/file/test_provider_system_file.py` & `tackle-0.5.0/tackle/providers/files/tests/file/test_provider_system_file.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/files/tests/zips/test_provider_system_zips.py` & `tackle-0.5.0/tackle/providers/files/tests/zips/test_provider_system_zips.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/generate/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/hooks/file_update.py` & `tackle-0.5.0/tackle/providers/generate/hooks/file_update.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/hooks/generate.py` & `tackle-0.5.0/tackle/providers/generate/hooks/generate.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/hooks/jinja.py` & `tackle-0.5.0/tackle/providers/generate/hooks/jinja.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/hooks/update_section.py` & `tackle-0.5.0/tackle/providers/generate/hooks/update_section.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py` & `tackle-0.5.0/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py` & `tackle-0.5.0/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py` & `tackle-0.5.0/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/git/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/git/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/git/hooks/github.py` & `tackle-0.5.0/tackle/providers/git/hooks/github.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/git/hooks/gits.py` & `tackle-0.5.0/tackle/providers/git/hooks/gits.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/git/hooks/meta.py` & `tackle-0.5.0/tackle/providers/git/hooks/meta.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/git/tests/test_provider_git_hooks.py` & `tackle-0.5.0/tackle/providers/git/tests/test_provider_git_hooks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/ini/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/ini/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/ini/hooks/ini.py` & `tackle-0.5.0/tackle/providers/ini/hooks/ini.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/ini/tests/test_provider_ini.py` & `tackle-0.5.0/tackle/providers/ini/tests/test_provider_ini.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/json/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/json/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/json/hooks/jsons.py` & `tackle-0.5.0/tackle/providers/json/hooks/jsons.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/kubernetes/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/kubernetes/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/kubernetes/hooks/context.py` & `tackle-0.5.0/tackle/providers/kubernetes/hooks/context.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/kubernetes/tests/kubeconfig.yaml` & `tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/kubernetes/tests/kubeconfig2.yaml` & `tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig2.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/logic/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/logic/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/logic/hooks/assertion.py` & `tackle-0.5.0/tackle/providers/logic/hooks/assertion.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/logic/hooks/while.py` & `tackle-0.5.0/tackle/providers/logic/hooks/while.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/logic/tests/match/block-loop.yaml` & `tackle-0.5.0/tackle/providers/logic/tests/match/case-block-loop.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
   ->: match matcher
   case:
     blocker->:
       for:
         - stuff
         - things
       value: True
-      a_dict:
-        stuff->: "{{case}}"
+      dict:
+        stuff->: "{{item}}"
       list:
         - stuff
         - things
       hook-expanded:
         ->: literal expanded
       hook-compact->: literal compact
```

### Comparing `tackle-0.4.9/tackle/providers/logic/tests/match/loop.yaml` & `tackle-0.5.0/tackle/providers/logic/tests/match/loop.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 cases:
   - value
   - a_dict
   - list
   - hook-dict
   - hook-expanded
   - hook-compact
-#  - block
+  - block
 
 matches:
   ->: match
   for: cases
   value: "{{item}}"
   case:
     value: True
@@ -28,27 +28,27 @@
       hook-dict-expanded:
         ->: literal expanded
       hook-dict-compact->: literal compact
 
     hook-expanded:
       ->: literal expanded
     hook-compact->: literal compact
-#    block->:
-#      for:
-#        - stuff
-#        - things
-#      value: True
-#      a_dict:
-#        stuff->: "{{item}}"
-#      list:
-#        - stuff
-#        - things
-#      hook-expanded:
-#        ->: literal expanded
-#      hook-compact->: literal compact
+    block->:
+      for:
+        - stuff
+        - things
+      value: True
+      a_dict:
+        stuff->: "{{item}}"
+      list:
+        - stuff
+        - things
+      hook-expanded:
+        ->: literal expanded
+      hook-compact->: literal compact
 
 
 expected:
   - True
   - stuff: things
   -
     - stuff
@@ -77,8 +77,8 @@
 #        stuff: things
 #      list:
 #        - stuff
 #        - things
 #      hook-expanded: expanded
 #      hook-compact: compact
 
-assert->: assert "{{matches}}" "{{expected}}"
+#assert->: assert "{{matches}}" "{{expected}}"
```

### Comparing `tackle-0.4.9/tackle/providers/logic/tests/match/test_provider_logic_match.py` & `tackle-0.5.0/tests/parser/test_parser_parse_hook.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,60 @@
+"""High level tests for parser logic."""
 import pytest
-from tackle import tackle
-from tackle.exceptions import HookCallException
 
+from tackle.main import tackle
+from tackle.utils.files import read_config_file
 
-def test_hook_match_loop(change_dir):
-    """Run a loop of different match cases."""
-    output = tackle('loop.yaml')
-    # Assertions in fixture
-    assert output
-
-
-# TODO: https://github.com/sudoblockio/tackle/issues/66
-#  Add merge to loop functions
-# def test_hook_match_block_loop(change_dir):
-#     """Check that we can merge from a looped block into a looped match."""
-#     output = tackle('block-loop.yaml')
-#     # Assertions in fixture
-#     assert output
-
-# TODO: https://github.com/sudoblockio/tackle/issues/66
-#  Fix basic block macro functionality
-# def test_hook_match_block_if(change_dir):
-#     """Check that any kind of first level block makes sense."""
-#     output = tackle('block-if.yaml')
-#     # TODO: Assertions in fixture
-#     assert output
-
-
-def test_hook_match_cases(change_dir):
-    """Run the source and check that the hooks imported the demo module."""
-    output = tackle('cases.yaml')
-    assert output['matched_dict'] == 'this'
-    assert output['fallback_dict'] == 'foo'
-
-
-def test_hook_match_value_list(change_dir):
-    """
-    Edge case where in match hooks one can have a single value trying to be merged into
-    a temporary context which does not make sense.
-    """
-    output = tackle('value-list.yaml')
-    # Assertions in file
-    assert output
-
-
-def test_hook_match_value_lists(change_dir):
-    """
-    Edge case where in match hooks one can have a single value trying to be merged into
-    a temporary context which does not make sense.
-    """
-    o = tackle('lists.yaml')
-    assert o
-
-
-def test_hook_match_value_wrong_hook_type(change_dir):
-    """
-    Edge case where in match hooks one can have a single value trying to be merged into
-    a temporary context which does not make sense.
+FIXTURES = [
+    ('map.yaml', 'map-output.yaml'),
+    ('map-lists.yaml', 'map-lists-output.yaml'),
+    ('arg-types.yaml', 'arg-types-output.yaml'),
+    ('empty-elements.yaml', 'empty-elements.yaml'),
+    ('map-root.yaml', 'map-root-output.yaml'),
+    ('private-hooks.yaml', 'private-hooks-output.yaml'),
+    ('outer-tackle.yaml', 'outer-tackle-output.yaml'),
+    ('outer-tackle-list.yaml', 'outer-tackle-list-output.yaml'),
+    ('merge-simple.yaml', 'merge-simple-output.yaml'),
+    ('merge-petstore-compact.yaml', 'petstore.yaml'),
+    ('private-context.yaml', 'private-context-output.yaml'),
+    # Non tackle things
+    ('k8s-deployment.yaml', 'k8s-deployment.yaml'),
+    ('ansible-playbook.yaml', 'ansible-playbook.yaml'),
+    ('docker-compose.yml', 'docker-compose.yml'),
+    ('list-list.yaml', 'list-list.yaml'),
+    ('var-hook.yaml', 'var-hook-output.yaml'),
+    ('toml.toml', 'toml.yaml'),
+    # # Broken
+    # # TODO: https://github.com/robcxyz/tackle/issues/52
+    # ('bug-mixed-flags.yaml', 'bug-mixed-flags.yaml'),
+    # ('document-hooks.yaml', 'document-hooks-expected.yaml'),
+]
+
+
+@pytest.mark.parametrize("fixture,expected_output", FIXTURES)
+def test_main_expected_output(change_curdir_fixtures, fixture, expected_output):
+    """Input equals output."""
+    expected_output = read_config_file(expected_output)
+    output = tackle(fixture)
+    assert output == expected_output
+
+
+def test_parser_ruamel_braces(change_curdir_fixtures):
+    """
+    Validate super hack for ruamel parsing error where `stuff->: {{things}}`
+    (no quotes), ruamel interprets as:
+    'stuff': ordereddict([(ordereddict([('things', None)]), None)]).
+    """
+    output = tackle('ruamel-parsing-error-braces.yaml', verbose=True)
+    assert output['stuff'] == 'things'
+    assert output['a']['b'] is None
+    assert output['one'] == 'two'
+
+
+def test_parser_duplicate_values(change_curdir_fixtures):
+    """
+    Validate that when we give a hook with duplicate values as what was set in the
+     initial run (ie a tackle hook with `no_input` set), that we take the value from the
+     hook.
     """
-    with pytest.raises(HookCallException):
-        tackle('wrong-hook-type.yaml')
+    output = tackle('duplicate-values.yaml', verbose=True)
+    assert output['local']['two_args']
```

### Comparing `tackle-0.4.9/tackle/providers/paths/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/paths/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/hooks/dirs.py` & `tackle-0.5.0/tackle/providers/paths/hooks/dirs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/hooks/find_in.py` & `tackle-0.5.0/tackle/providers/paths/hooks/find_in.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/hooks/flatten.py` & `tackle-0.5.0/tackle/providers/paths/hooks/flatten.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/hooks/globs.py` & `tackle-0.5.0/tackle/providers/paths/hooks/globs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/hooks/paths.py` & `tackle-0.5.0/tackle/providers/paths/hooks/paths.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/hooks/symlinks.py` & `tackle-0.5.0/tackle/providers/paths/hooks/symlinks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py` & `tackle-0.5.0/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/tests/flatten/tackle.yaml` & `tackle-0.5.0/tackle/providers/paths/tests/flatten/tackle.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/paths/tests/test_provider_system_path.py` & `tackle-0.5.0/tackle/providers/paths/tests/test_provider_system_path.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/postgres/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/postgres/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/postgres/hooks/query.py` & `tackle-0.5.0/tackle/providers/postgres/hooks/query.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/prompts/.tackle.meta.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -109,18 +109,22 @@
       content->: file tests/checkbox/map_normal.yaml
       output: |
         ? What you do?  (<up>, <down> to move, <space> to select, <a> to toggle, <i> to invert)
          ❯○ stuff
           ● things
 
   checkbox:
-    - description: The basic versions of the `select` can be called in these ways
-      content->: "{{select_content}}"
-      output_text->: "{{select_output_text}}"
-      output->: "{{select_output}}"
+    - description: The basic versions of the `checkbox` hook can be called in these ways
+      content->: "{{checkbox_content}}"
+      output_text->: "{{checkbox_output_text}}"
+      output->: "{{checkbox_output}}"
 
-    - description: Other versions can use custom prompts for the choices
+    - description: Other versions can use custom prompts for the choices and output the key.
       content->: file tests/checkbox/map.yaml
+      output_text: |
+        ? What you do?
+        ❯ ◉ I do stuff
+          ◉ I do things
       output: |
-        ? What you do?  (Use arrow keys)
-         ❯ I do stuff
-           I do things
+        selection:
+          - stuff
+          - things
```

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/checkbox.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/checkbox.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/confirm.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/confirm.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/editor.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/editor.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/expand.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/expand.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/input.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/input.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/password.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/password.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/rawlist.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/rawlist.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/hooks/select.py` & `tackle-0.5.0/tackle/providers/prompts/hooks/select.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE` & `tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py` & `tackle-0.5.0/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/prompts/tests/select/test_prompt_provider_select.py` & `tackle-0.5.0/tackle/providers/prompts/tests/select/test_prompt_provider_select.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/ssh/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/ssh/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/ssh/hooks/interactive.py` & `tackle-0.5.0/tackle/providers/ssh/hooks/interactive.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/ssh/hooks/ssh.py` & `tackle-0.5.0/tackle/providers/ssh/hooks/ssh.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/strings/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/strings/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/strings/hooks/b64.py` & `tackle-0.5.0/tackle/providers/strings/hooks/b64.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/strings/hooks/randoms.py` & `tackle-0.5.0/tackle/providers/strings/hooks/randoms.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/strings/hooks/regex.py` & `tackle-0.5.0/tackle/providers/strings/hooks/regex.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/strings/hooks/strings.py` & `tackle-0.5.0/tackle/providers/strings/hooks/strings.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/strings/tests/strings/test_provider_system_split.py` & `tackle-0.5.0/tackle/providers/strings/tests/strings/test_provider_system_split.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/tackle/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/block.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 
 from tackle.models import BaseHook, Context, Field
-from tackle.parser import walk_sync
+from tackle.parser import walk_element
 
 
 class BlockHook(BaseHook):
     """
     Hook for blocks of hooks. This is a special case where `items` are parsed like a
      normal context with the added benefit of maintaining a `temporary_context` so that
      items on the same level can be accessed in memory / rendered. Normally executed
@@ -37,10 +37,10 @@
             key_path_block=self.key_path.copy(),
             no_input=self.no_input,
             calling_directory=self.calling_directory,
             calling_file=self.calling_file,
             verbose=self.verbose,
             override_context=self.override_context,
         )
-        walk_sync(context=tmp_context, element=self.items.copy())
+        walk_element(context=tmp_context, element=self.items.copy())
 
         return self.public_context
```

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/debug.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/debug.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/flatten.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/flatten.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/import.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/import.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/provider_docs.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/provider_docs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/run_hook.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/run_hook.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/tackle.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/tackle.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/hooks/variable.py` & `tackle-0.5.0/tackle/providers/tackle/hooks/variable.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/tests/flatten/kubectl.yaml` & `tackle-0.5.0/tackle/providers/tackle/tests/flatten/kubectl.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/tests/flatten/ls.yaml` & `tackle-0.5.0/tackle/providers/tackle/tests/flatten/ls.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py` & `tackle-0.5.0/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/tests/import/test_provider_tackle_import.py` & `tackle-0.5.0/tackle/providers/tackle/tests/import/test_provider_tackle_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from tackle import tackle
 from tackle.models import Context
-from tackle.parser import update_source
+from tackle.parser import parse_source
 
 FIXTURES = [
     'expanded-string.yaml',
     'expanded-list-dict.yaml',
     'local.yaml',
     'function-import.yaml',
 ]
@@ -14,15 +14,15 @@
 
 @pytest.mark.parametrize("target", FIXTURES)
 def test_provider_system_hook_import(change_dir, target):
     """Run the source and check that the hooks imported the demo module."""
     context = Context(input_string=target)
     # num_providers = len(context.provider_hooks.keys())
     num_providers = len(context.private_hooks.keys())
-    update_source(context)
+    parse_source(context)
     # assert num_providers < len(context.provider_hooks.keys())
     assert num_providers < len(context.private_hooks.keys())
     # assert 'tackle.providers.tackle-demos' in context.providers.hook_types
 
 
 def test_provider_system_hook_import_local(change_dir):
     """Assert local import of hook is valid."""
```

### Comparing `tackle-0.4.9/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py` & `tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py` & `tackle-0.5.0/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/toml/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/toml/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/toml/hooks/tomls.py` & `tackle-0.5.0/tackle/providers/toml/hooks/tomls.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/types/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/types/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/types/hooks/casting.py` & `tackle-0.5.0/tackle/providers/types/hooks/casting.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/types/hooks/type.py` & `tackle-0.5.0/tackle/providers/types/hooks/type.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/types/tests/test_provider_types.py` & `tackle-0.5.0/tackle/providers/types/tests/test_provider_types.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/web/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/web/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/web/hooks/browser.py` & `tackle-0.5.0/tackle/providers/web/hooks/browser.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/web/hooks/request.py` & `tackle-0.5.0/tackle/providers/web/hooks/request.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/web/tests/test_requests_provider.py` & `tackle-0.5.0/tackle/providers/web/tests/test_requests_provider.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/yaml/.tackle.meta.yaml` & `tackle-0.5.0/tackle/providers/yaml/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/yaml/hooks/yaml_in_place.py` & `tackle-0.5.0/tackle/providers/yaml/hooks/yaml_in_place.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/yaml/hooks/yamls.py` & `tackle-0.5.0/tackle/providers/yaml/hooks/yamls.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/providers/yaml/tests/test_provider_system_yaml.py` & `tackle-0.5.0/tackle/providers/yaml/tests/test_provider_system_yaml.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/render.py` & `tackle-0.5.0/tackle/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,23 +96,26 @@
             # that it can be called within the jinja globals along with the wrapped exec
             jinja_method.set_method(k, jinja_method.wrapped_exec)
 
             add_jinja_hook_methods(context, jinja_method)
 
 
 # wrapped_exec calls exec on the `hook` integrating any positional args
-def render_string(context: 'Context', raw: str):
+def render_string(context: 'Context', raw: str) -> Any:
     """
     Render strings by first extracting renderable variables then build a render context
-    from the public_context, then existing context, and last looks up special variables.
-    After the value has been rendered it is returned as literal so as to preserve the
-    original type of the value.
+     from the public_context, then existing context, and last looks up special
+     variables. After the value has been rendered it is returned as literal so as to
+     preserve the original type of the value.
 
     :return: The literal value if the output is a string / list / dict / float / int
     """
+    if not isinstance(raw, str):
+        return raw
+
     if ('{{' not in raw) and ('{%' not in raw):
         return raw
 
     try:
         template = context.env_.from_string(raw)
     except TemplateSyntaxError as e:
         raise MalformedTemplateVariableException(
```

### Comparing `tackle-0.4.9/tackle/settings.py` & `tackle-0.5.0/tackle/settings.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/special_vars.py` & `tackle-0.5.0/tackle/special_vars.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/command.py` & `tackle-0.5.0/tackle/utils/command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/dicts.py` & `tackle-0.5.0/tackle/utils/dicts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Utils for modifying complex dictionaries generally based on an encoded key_path which is
 a list of strings for key value lookups and byte encoded integers for items in a list.
 """
 from typing import Union, Any, TYPE_CHECKING
+from enum import Enum
 from ruamel.yaml.constructor import CommentedKeyMap
 
 if TYPE_CHECKING:
     from tackle.models import Context
 
 
 def encode_list_index(list_index: int) -> bytes:
@@ -71,15 +72,15 @@
             readable_key_path.append(i)
     return '.'.join(readable_key_path)
 
 
 def nested_delete(element, keys):
     """
     Delete items in a generic element (list / dict) based on a key path in the form of
-    a list with strings for keys and byte encoded integers for indexes in a list.
+     a list with strings for keys and byte encoded integers for indexes in a list.
     """
     num_elements = len(keys)
 
     if num_elements == 1:
         if isinstance(keys[0], bytes):
             element.pop(decode_list_index(keys[0]))
             return element
@@ -139,28 +140,33 @@
         return element[keys[0]]
 
     if isinstance(keys[0], bytes):
         return nested_get(element[decode_list_index(keys[0])], keys[1:])
     return nested_get(element[keys[0]], keys[1:])
 
 
-def nested_set(element, keys, value, index: int = 0):
+def nested_set(element: Union[dict, list], keys: list, value: Any, index: int = 0):
     """
     Set the value of an arbitrary object based on a key_path in the form of a list
-    with strings for keys and byte encoded integers for indexes in a list. This function
-    recurses through the element until it is at the end of the keys where it sets it.
+     with strings for keys and byte encoded integers for indexes in a list. This
+     function recurses through the element until it is at the end of the keys where it
+     sets it.
 
     :param element: A generic dictionary or list
     :param keys: List of string and byte encoded integers.
     :param value: The value to set
     :param index: Index is only used when called recursively, not initially
     """
     num_elements = len(keys)
     # Check if we are at the last element of the list to insert the value
     if index == num_elements - 1:
+        # Check is value is enum and evaluate it as value so it is serializable.
+        if isinstance(value, Enum):
+            value = value.value
+
         if isinstance(keys[-1], bytes):
             element.insert(decode_list_index(keys[-1]), value)
         else:
             element[keys[-1]] = value
         return
 
     if isinstance(element, dict):
@@ -179,15 +185,19 @@
             element.insert(decode_list_index(keys[index]), [])
         else:
             element.insert(decode_list_index(keys[index]), {})
         element = element[decode_list_index(keys[index])]
     nested_set(element, keys, value, index + 1)
 
 
-def get_target_and_key(context: 'Context', key_path: list = None) -> (Any, list):
+def get_target_and_key(
+        context: 'Context',
+        key_path: list = None,
+) -> (Any, list):
+    """Get the target context and key to `set_key` from."""
     target_context = context.public_context
 
     if key_path is None:
         key_path = context.key_path
 
     output_key_path = []
     for i in key_path:
@@ -199,53 +209,85 @@
             target_context = context.private_context
         elif i != '->':
             output_key_path.append(i)
 
     return target_context, output_key_path
 
 
-def smush_key_path(key_path: list) -> list:
+def remove_arrows_from_key_path(
+        key_path: list
+) -> list:
     """Remove the arrows from a key path."""
     output = []
     for i in key_path:
         if i not in ('->', '_>'):
             output.append(i)
     return output
 
 
+def set_temporary_context(
+        context: 'Context',
+        value: Any,
+        key_path: list,
+) -> None:
+    tmp_key_path = key_path[(len(context.key_path_block) - len(key_path)):]
+
+    if context.temporary_context is None:
+        context.temporary_context = {} if isinstance(tmp_key_path[0], str) else []
+    tmp_key_path = [i for i in tmp_key_path if i not in ('->', '_>')]
+
+    if len(tmp_key_path) == 0:
+        # Nothing to set in tmp context
+        return
+
+    nested_set(context.temporary_context, tmp_key_path, value)
+
+
+def get_set_temporary_context(
+        context: 'Context',
+) -> None:
+    """
+    Used in hooks with indented contexts (ie block/match), it gets the output of the
+     target context (public / private) sets that value within the temporary context
+     so that it can be used for rendering.
+    """
+    target_context, set_key_path = get_target_and_key(
+        context=context,
+        key_path=context.key_path
+    )
+    value = nested_get(element=target_context, keys=set_key_path)
+    set_temporary_context(
+        context=context,
+        value=value,
+        key_path=context.key_path,
+    )
+
+
 def set_key(
-    context: 'Context',
-    value: Any,
-    key_path: list = None,
+        context: 'Context',
+        value: Any,
+        key_path: list = None,
 ):
     """
     Wrap nested_set to set keys for both public and private hook calls.
 
     For public hook calls, qualifies if the hook is compact form (ie key->) or expanded
-    (ie key: {->:..}) before setting the output. For private hook calls, the key and
-    all parent keys without additional objects are deleted later as they might be
-    used in rendering so they are added as well but their key paths are tracked for
-    later deletion.
+     (ie key: {->:..}) before setting the output. For private hook calls, the key and
+     all parent keys without additional objects are deleted later as they might be
+     used in rendering so they are added as well but their key paths are tracked for
+     later deletion.
     """
     if key_path is None:
         key_path = context.key_path
 
     target_context, set_key_path = get_target_and_key(context, key_path=key_path)
     nested_set(target_context, set_key_path, value)
 
     if len(context.key_path_block) != 0:
-        tmp_key_path = key_path[(len(context.key_path_block) - len(key_path)) :]
-        if context.temporary_context is None:
-            context.temporary_context = {} if isinstance(tmp_key_path[0], str) else []
-        tmp_key_path = [i for i in tmp_key_path if i not in ('->', '_>')]
-
-        if tmp_key_path:
-            # Assert that the list is not empty - handles cases where we are appending
-            #  a value from a list.
-            nested_set(context.temporary_context, tmp_key_path, value)
+        set_temporary_context(context=context, value=value, key_path=key_path)
 
 
 def _clean_item(element: Union[dict, list], item: Union[int, str], value: Any):
     if isinstance(value, dict):
         try:
             value_key = next(iter(value.keys()))
         except StopIteration:
@@ -274,15 +316,15 @@
         for i, v in enumerate(element):
             _clean_item(element, i, v)
 
 
 def merge(a, b, path=None, update=True):
     """
     See https://stackoverflow.com/questions/7204805/python-dictionaries-of-dictionaries-merge
-    Merges b into a
+     Merges b into a.
     """
     if path is None:
         path = []
     for key in b:
         if key in a:
             if isinstance(a[key], dict) and isinstance(b[key], dict):
                 merge(a[key], b[key], path + [str(key)])
```

### Comparing `tackle-0.4.9/tackle/utils/files.py` & `tackle-0.5.0/tackle/utils/files.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/help.py` & `tackle-0.5.0/tackle/utils/help.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/log.py` & `tackle-0.5.0/tackle/utils/log.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/paths.py` & `tackle-0.5.0/tackle/utils/paths.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/prompts.py` & `tackle-0.5.0/tackle/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/vcs.py` & `tackle-0.5.0/tackle/utils/vcs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle/utils/zipfile.py` & `tackle-0.5.0/tackle/utils/zipfile.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tackle.egg-info/PKG-INFO` & `tackle-0.5.0/tackle.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: tackle
-Version: 0.4.9
+Version: 0.5.0
 Summary: Tackle is a declarative DSL for building modular workflows and code generators. Tool is plugins based and can easily be extended by writing additional hooks or importing external providers that can be turned into a self documenting CLI, all out of yaml, json, toml.
 Home-page: https://github.com/robcxyz/tackle
 Author: Rob Cannon
 Author-email: robc.io.opensource@gmail.com
 License: BSD
 Description: <img align="right" width="280" height="280" src="https://raw.githubusercontent.com/sudoblockio/tackle/main/docs/assets/logo-box.png">
         
         # tackle
         
         [![pypi](https://img.shields.io/pypi/v/tackle.svg)](https://pypi.python.org/pypi/tackle)
         [![python](https://img.shields.io/pypi/pyversions/tackle.svg)](https://pypi.python.org/pypi/tackle)
         [![codecov](https://codecov.io/gh/sudoblockio/tackle/branch/main/graphs/badge.svg?branch=main)](https://codecov.io/github/sudoblockio/tackle?branch=main)
         [![codeql](https://github.com/sudoblockio/tackle/actions/workflows/codeql.yml/badge.svg)](https://github.com/sudoblockio/tackle/actions/workflows/codeql.yml)
-        [![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/success?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
-        [![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/test?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
-        [![Foresight Docs](https://api-public.service.runforesight.com/api/v1/badge/utilization?repoId=4abde40b-565a-4557-afc0-983461857bb4)](https://docs.runforesight.com/)
         
         [//]: # ([![main-tests]&#40;https://github.com/sudoblockio/tackle/actions/workflows/main.yml/badge.svg&#41;]&#40;https://github.com/sudoblockio/tackle/actions&#41;)
         
         * [Documentation](https://sudoblockio.github.io/tackle)
         * [Discord](https://discord.gg/7uVUfUVD7K)
         * [PyPI](https://pypi.org/project/tackle/)
         * [BSD License](LICENSE)
         
         [//]: # (* [Slack]&#40;https://join.slack.com/t/slack-y748219/shared_invite/zt-1cqreswyd-5qDBE53QlY97mQOI6DhcKw&#41;)
         
-        Tackle is an experimental general purpose configuration language for building modular code generators and declarative CLIs. Built as a fork of [cookiecutter](https://github.com/cookiecutter/cookiecutter), it can make any config file dynamic or into a CLI with both strong and weakly typed programmable flow control common to a general purpose programming language. Basically you can write a fully functional Turing-complete program out of a config file. It's wild.
+        Tackle is an experimental general purpose configuration language for building modular code generators and declarative CLIs. Built as a fork of [cookiecutter](https://github.com/cookiecutter/cookiecutter), it can make any config file into a CLI with both strong and weakly typed programmable flow control common to a general purpose programming language. Basically you can write a fully functional Turing-complete program out of a config file. It's wild.
         
         **With tackle, you can build:**
         - Modular code generators / repo scaffolding tools that can be updated over time
         - Interactive glue code for infrastructure-as-code deployment strategies
         - Generic utilities like SSH helpers and dotfile managers
         - Combinations of all of the above and anything else you can think of
         
@@ -50,29 +47,30 @@
           - Read and write [yaml](https://sudoblockio.github.io/tackle/providers/Yaml/) / [toml](https://sudoblockio.github.io/tackle/providers/Toml/) / [json](https://sudoblockio.github.io/tackle/providers/Json/) [files](https://sudoblockio.github.io/tackle/providers/Files/)
           - [Make http calls](https://sudoblockio.github.io/tackle/providers/Web/)
           - [Run arbitrary system commands](https://sudoblockio.github.io/tackle/providers/Command/)
           - [Manipulate the context](https://sudoblockio.github.io/tackle/providers/Context/)
           - [Run other tackle files](https://sudoblockio.github.io/tackle/providers/Tackle/tackle/)
         - Modular design allows creating / importing new hooks easy
           - Supports both [python](https://sudoblockio.github.io/tackle/python-hooks/) and [declarative](https://sudoblockio.github.io/tackle/declarative-hooks/) hooks which can be imported / called / defined in-line or within jinja templates
+          - Hooks can be composed of other hooks allowing complex objects to be validated and operated against
         
         ### Install
         
         > Note: tackle can install dependencies on its own. Check [docs](https://sudoblockio.github.io/tackle/installation#best-installation-method) for advanced installation methods to isolate tackle from your system python.
         
         ```shell
         python -m venv env && source env/bin/activate
         pip install tackle
         ```
         
         **Quick Demo:** `tackle sudoblockio/tackle-hello-world`
         
         ### Hello world
         
-        Check out the [docs](https://sudoblockio.github.io/tackle/hello-worlds/) for >10 hello worlds that demonstrate the various aspects of the syntax with the simplest one using the [print](https://sudoblockio.github.io/tackle/providers/Console/print/) hook, one of [>100 hooks](https://sudoblockio.github.io/tackle/installation#best-installation-method).
+        Check out the [docs](https://sudoblockio.github.io/tackle/hello-worlds/) for >10 hello worlds that demonstrate the various aspects of the syntax with the simplest one using the [print](https://sudoblockio.github.io/tackle/providers/Console/print/) hook, one of [>100 hooks](https://sudoblockio.github.io/tackle/providers/Collections/).
         
         **hello.yaml**
         ```yaml
         # Any time a key ends with `->`, we are calling a hook
         hw->: print Hello world!
         ```
         
@@ -96,14 +94,15 @@
             - world!
           if: item != 'cruel'
         # Or combinations of the above with other methods like try/except
         ```
         
         New hooks can be [made in python](https://sudoblockio.github.io/tackle/python-hooks/) which under the hood is a [pydantic](https://github.com/pydantic/pydantic) model.
         
+        **.hooks/hello.py**
         ```python
         from tackle import BaseHook
         
         class Greeter(BaseHook):
             hook_type: str = "greeter"
             target: str
             args: list = ['target']
@@ -111,61 +110,65 @@
               expression = f"Hello {self.target}"
               print(expression)
               return expression
         ```
         
         Or can be [defined inline within your tackle file, imported remotely, or in a `hooks` directory.](https://sudoblockio.github.io/tackle/declarative-hooks/).
         
+        **.hooks/hello.yaml**
         ```yaml
         # Keys ending with `<-` mean we are creating a hook / method
         greeter<-:
           target: str
           args: ['target']
           exec<-:
             expression->: var Hello {{target}}  # var hook renders variables
             p->: print {{expression}}
           return: expression
         ```
         
         And both can be [called the same way](https://sudoblockio.github.io/tackle/writing-tackle-files/).
         
+        **tackle.yaml**
         ```yaml
         hello: world!
         With a flag->: greeter --target {{hello}}
         Target in argument->: greeter {{hello}}
         Expanded fields:
           ->: greeter
           target: {{hello}}
         Jinja template->: {{ greeter(hello) }}
         # Or combinations jinja and compact / expanded hooks allowing chaining of hook calls.
         ```
         
-        With the declarative hooks being callable from the command line:
+        With the declarative hooks being [callable from the command line](https://sudoblockio.github.io/tackle/declarative-cli/):
         
         ```shell
         tackle hello.yaml greeter --target world!
         # Or from a github repo
         tackle sudoblockio/tackle-hello-world greeter --target world!
         ```
         
         Documentation can be embedded into the hooks.
         
+        **hello.yaml**
         ```yaml
         <-:
           help: This is the default hook
           target:
-            type: str
+            type: union[str, int]
             default->: input
             description: The thing to say hello to
           exec<-:
             greeting->: select Who to greet? --choices ['world',target]
             hi->: greeter --target {{greeting}}
           greeting-method<-:
             help: A method that greets
             # ... Greeting options / logic
+            extends: greeter
         greeter<-:
           help: A reusable greeter object
           target: str
           exec<-:
             hi->: print Hello {{target}}
         ```
         
@@ -179,26 +182,26 @@
         options:
             --target [str] The thing to say hello to
         methods:
             greeting-method     A method that greets
             greeter     A reusable greeter object
         ```
         
-        Hooks can be imported, linked, and/or combined creating a web of CLIs.
+        Hooks can be imported [within a tackle provider](https://sudoblockio.github.io/tackle/declarative-cli/#importing-hooks) or [through hooks](https://sudoblockio.github.io/tackle/providers/Tackle/import/), [linked](https://sudoblockio.github.io/tackle/providers/Tackle/tackle/), and/or combined with [inheritance](https://sudoblockio.github.io/tackle/declarative-hooks/#extending-hooks) or [composition](https://sudoblockio.github.io/tackle/declarative-hooks/#extending-hooks) creating a web of CLIs.
         
         ### Use Cases
         
         - [Code Generation](https://sudoblockio.github.io/tackle/tutorials/code-generation/)
         
         **WIP Tutorials**
         
-        - [Declarative Utilities]()
-        - [Infrastructure-as-Code Management]()
-        - [Kubernetes Manifest Management]()
-        - [Toolchain Management]()
+        - Declarative Utilities
+        - Infrastructure-as-Code Management
+        - Kubernetes Manifest Management
+        - Toolchain Management
         
         [//]: # (- [Repo Management]&#40;&#41; - wip)
         
         ### Topics
         
         - [Writing Tackle Files](https://sudoblockio.github.io/tackle/writing-tackle-files/)
         - [Creating Providers](https://sudoblockio.github.io/tackle/creating-providers/)
@@ -210,16 +213,15 @@
         - [Declarative CLIs](https://sudoblockio.github.io/tackle/declarative-cli/)
         
         ### Known Issues
         
         - **Windows Support**
           - tackle is lacking some windows support as shown in the [failed tests](https://github.com/sudoblockio/tackle/actions/workflows/main-windows.yml). If you are a windows user, it is highly recommended to use WSL. **Please get in touch** if you are motivated to fix these tests to make tackle fully cross-platform. It probably isn't that hard to fix them as they mostly are due to differences in how windows handles paths.
         - **Whitespaces**
-          - tackle relies heavily on parsing based on whitespaces which if you are not careful can easily bite you. Whenever you need to have some whitespaces preserved, make sure to quote the entire expression.
-        
+          - tackle relies heavily on parsing based on whitespaces which if you are not careful can easily bite you. Whenever you need to have some whitespaces preserved, make sure to quote the entire expression. Future work will be put in to overhaul the [regex based parser](https://github.com/sudoblockio/tackle/blob/main/tackle/utils/command.py#L52) with a PEG parser like [parsimonious](https://github.com/erikrose/parsimonious).
         
         ### Contributing
         
         Contributions are welcome but please be advised of the following notes.
         
         - This project uses [conventional commits](https://www.conventionalcommits.org/) which generates the [changelog](./CHANGELOG.md) with [release-please-action](https://github.com/google-github-actions/release-please-action) in the [release](https://github.com/sudoblockio/tackle/blob/main/.github/workflows/release.yml) CI workflow. If commits have been made outside of this convention they will be squashed accordingly.
         - For making changes to providers, please include test coverage using the existing fixtures and patterns from prior tests or communicate any suggestions that deviate from this style. It definitely can be improved but consistency is more important than making directed improvements. Tests should be runnable from the test's directory and via `make test`.
@@ -250,16 +252,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: web
-Provides-Extra: toml
 Provides-Extra: ssh
-Provides-Extra: console
 Provides-Extra: git
-Provides-Extra: postgres
 Provides-Extra: kubernetes
+Provides-Extra: web
+Provides-Extra: postgres
+Provides-Extra: toml
+Provides-Extra: console
 Provides-Extra: dev
 Provides-Extra: all
```

### Comparing `tackle-0.4.9/tackle.egg-info/SOURCES.txt` & `tackle-0.5.0/tackle.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -207,22 +207,32 @@
 tackle/providers/kubernetes/tests/test_provider_k8s_context.py
 tackle/providers/logic/.tackle.meta.yaml
 tackle/providers/logic/hooks/assertion.py
 tackle/providers/logic/hooks/match.py
 tackle/providers/logic/hooks/while.py
 tackle/providers/logic/tests/assertion/assert.yaml
 tackle/providers/logic/tests/assertion/test_provider_logic_assert.py
-tackle/providers/logic/tests/match/block-if.yaml
-tackle/providers/logic/tests/match/block-loop.yaml
+tackle/providers/logic/tests/match/block-loop-match-block.yaml
+tackle/providers/logic/tests/match/block-match-block.yaml
+tackle/providers/logic/tests/match/case-block-if.yaml
+tackle/providers/logic/tests/match/case-block-loop.yaml
+tackle/providers/logic/tests/match/case-block-merge.yaml
+tackle/providers/logic/tests/match/case-block.yaml
+tackle/providers/logic/tests/match/case-dict-hooks.yaml
+tackle/providers/logic/tests/match/case-dict.yaml
 tackle/providers/logic/tests/match/cases.yaml
+tackle/providers/logic/tests/match/default-hook.yaml
+tackle/providers/logic/tests/match/default-underscore.yaml
+tackle/providers/logic/tests/match/error-block-loop-merge.yaml
+tackle/providers/logic/tests/match/error-malformed-regex.yaml
+tackle/providers/logic/tests/match/error-non-existant-key.yaml
+tackle/providers/logic/tests/match/error-wrong-hook-type.yaml
 tackle/providers/logic/tests/match/lists.yaml
 tackle/providers/logic/tests/match/loop.yaml
 tackle/providers/logic/tests/match/test_provider_logic_match.py
-tackle/providers/logic/tests/match/value-list.yaml
-tackle/providers/logic/tests/match/wrong-hook-type.yaml
 tackle/providers/logic/tests/while/while.yaml
 tackle/providers/paths/.tackle.meta.yaml
 tackle/providers/paths/hooks/dirs.py
 tackle/providers/paths/hooks/find_in.py
 tackle/providers/paths/hooks/flatten.py
 tackle/providers/paths/hooks/globs.py
 tackle/providers/paths/hooks/listdir.py
@@ -244,14 +254,15 @@
 tackle/providers/paths/tests/listdir/test_provider_system_listdir.py
 tackle/providers/paths/tests/listdir/dir/.hidden-stuff
 tackle/providers/paths/tests/listdir/dir/stuff.txt
 tackle/providers/paths/tests/listdir/dir/things.py
 tackle/providers/paths/tests/listdir/dirs/.hidden-stuff
 tackle/providers/paths/tests/listdir/dirs/stuff.txt
 tackle/providers/paths/tests/listdir/dirs/things.py
+tackle/providers/paths/tests/listdir/dirs/.hidden-dir/.gitkeep
 tackle/providers/paths/tests/listdir/dirs/dir1/stuff.txt
 tackle/providers/paths/tests/listdir/dirs/dir1/things.py
 tackle/providers/paths/tests/listdir/dirs/dir2/stuff.txt
 tackle/providers/paths/tests/listdir/dirs/dir2/things.py
 tackle/providers/paths/tests/symlink/src.yaml
 tackle/providers/paths/tests/symlink/tackle.yaml
 tackle/providers/paths/tests/symlink/test_provider_system_symlink.py
@@ -320,14 +331,16 @@
 tackle/providers/tackle/hooks/literal.py
 tackle/providers/tackle/hooks/provider_docs.py
 tackle/providers/tackle/hooks/run_hook.py
 tackle/providers/tackle/hooks/tackle.py
 tackle/providers/tackle/hooks/variable.py
 tackle/providers/tackle/tests/block/block-list.yaml
 tackle/providers/tackle/tests/block/block-logic.yaml
+tackle/providers/tackle/tests/block/block-loop-block-nested.yaml
+tackle/providers/tackle/tests/block/block-loop-block.yaml
 tackle/providers/tackle/tests/block/block-merge.yaml
 tackle/providers/tackle/tests/block/block.yaml
 tackle/providers/tackle/tests/block/embedded-blocks.yaml
 tackle/providers/tackle/tests/block/embedded-lists.yaml
 tackle/providers/tackle/tests/block/list.yaml
 tackle/providers/tackle/tests/block/looped-context-other.yaml
 tackle/providers/tackle/tests/block/looped-context.yaml
@@ -447,14 +460,117 @@
 tests/exceptions/fixtures/tackle.yaml
 tests/exceptions/fixtures/unknown-argument-extra.yaml
 tests/exceptions/fixtures/unknown-argument.yaml
 tests/exceptions/fixtures/unknown-named-argument.yaml
 tests/exceptions/fixtures/unknown-variable-call-tackle.yaml
 tests/exceptions/fixtures/unknown-variable-call.yaml
 tests/exceptions/fixtures/unknown-variable.yaml
+tests/functions/test_function_calls.py
+tests/functions/test_functions.py
+tests/functions/test_functions_args_kwargs_hooks.py
+tests/functions/test_functions_cli.py
+tests/functions/test_functions_enums.py
+tests/functions/test_functions_exceptions.py
+tests/functions/test_functions_field_hooks.py
+tests/functions/test_functions_help.py
+tests/functions/test_functions_types.py
+tests/functions/.hooks/base.yaml
+tests/functions/cli-fixtures/cli-call-func-output.yaml
+tests/functions/cli-fixtures/cli-call-func.yaml
+tests/functions/cli-fixtures/cli-default-hook-args.yaml
+tests/functions/cli-fixtures/cli-default-hook-context.yaml
+tests/functions/cli-fixtures/cli-default-hook-embedded.yaml
+tests/functions/cli-fixtures/cli-default-hook-no-context.yaml
+tests/functions/cli-fixtures/cli-hook-no-context.yaml
+tests/functions/cli-fixtures/cli-hook-type-unknown.yaml
+tests/functions/cli-fixtures/cli-no-default-hook.yaml
+tests/functions/cli-fixtures/a-dir/.gitkeep
+tests/functions/composition-fixtures/enum-basic.yaml
+tests/functions/exceptions/extends-missing.yaml
+tests/functions/exceptions/field-bad-type.yaml
+tests/functions/exceptions/field-require.yaml
+tests/functions/exceptions/hook-kwarg-missing-default.yaml
+tests/functions/exceptions/hook-kwarg-missing.yaml
+tests/functions/exceptions/missing-field.yaml
+tests/functions/exceptions/no-exec-type-error.yaml
+tests/functions/exceptions/return-str-not-found.yaml
+tests/functions/exceptions/str-value.yaml
+tests/functions/exceptions/try-in-default.yaml
+tests/functions/extends-fixtures/embedded-extends.yaml
+tests/functions/extends-fixtures/extends-list.yaml
+tests/functions/extends-fixtures/extends.yaml
+tests/functions/field-hooks-fixtures/extends-visible.yaml
+tests/functions/field-hooks-fixtures/extends.yaml
+tests/functions/field-hooks-fixtures/field-hooks-args-method.yaml
+tests/functions/field-hooks-fixtures/field-hooks-args.yaml
+tests/functions/field-hooks-fixtures/field-hooks-exec-args-method.yaml
+tests/functions/field-hooks-fixtures/field-hooks-exec-args.yaml
+tests/functions/field-hooks-fixtures/field-hooks-exec-method.yaml
+tests/functions/field-hooks-fixtures/field-hooks-exec.yaml
+tests/functions/field-hooks-fixtures/field-hooks-method.yaml
+tests/functions/field-hooks-fixtures/field-hooks.yaml
+tests/functions/field-hooks-fixtures/passed-context.yaml
+tests/functions/field-hooks-fixtures/.hooks/base-hook.yaml
+tests/functions/fixtures/call-output.yaml
+tests/functions/fixtures/call.yaml
+tests/functions/fixtures/compact.yaml
+tests/functions/fixtures/default-method-json.yaml
+tests/functions/fixtures/default-method-self.yaml
+tests/functions/fixtures/extends.yaml
+tests/functions/fixtures/field-types.yaml
+tests/functions/fixtures/flatten.yaml
+tests/functions/fixtures/list-call.yaml
+tests/functions/fixtures/no-exec.yaml
+tests/functions/fixtures/return-output.yaml
+tests/functions/fixtures/return-render.yaml
+tests/functions/fixtures/return.yaml
+tests/functions/fixtures/supplied-args-param-list.yaml
+tests/functions/fixtures/supplied-args-param-str.yaml
+tests/functions/fixtures/supplied-kwargs-param-dict.yaml
+tests/functions/fixtures/supplied-kwargs-param-str-loop.yaml
+tests/functions/fixtures/supplied-kwargs-param-str.yaml
+tests/functions/fixtures/.hooks/some-hooks.yaml
+tests/functions/fixtures/a-tackle/tackle.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-dict-error-default.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-dict-error-str.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-dict-error-type.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-list-error-default.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-list-error-str.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-list-error-type.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-str-error-default.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-str-error-str.yaml
+tests/functions/fixtures/field-type-exceptions/field-types-str-error-type.yaml
+tests/functions/fixtures/func-provider/tackle.yaml
+tests/functions/fixtures/func-provider-hook/tackle.yaml
+tests/functions/fixtures/func-provider-hook/a-dir/.gitkeep
+tests/functions/fixtures/func-provider-hook/hooks/funks.yaml
+tests/functions/fixtures/func-provider-method/tackle.yaml
+tests/functions/fixtures/func-provider-method/a-dir/.gitkeep
+tests/functions/fixtures/func-provider-method/hooks/funks.yaml
+tests/functions/fixtures/func-provider/a-dir/.gitkeep
+tests/functions/fixtures/func-provider/hooks/funks.yaml
+tests/functions/fixtures/methods/method-embed.yaml
+tests/functions/method-fixtures/method-args.yaml
+tests/functions/method-fixtures/method-base-validate.yaml
+tests/functions/method-fixtures/method-call-from-default.yaml
+tests/functions/method-fixtures/method-call-no-default.yaml
+tests/functions/method-fixtures/method-calll-default.yaml
+tests/functions/method-fixtures/method-embed.yaml
+tests/functions/method-fixtures/method-hook.yaml
+tests/functions/method-fixtures/method-inherit.yaml
+tests/functions/method-fixtures/method-maintain-context.yaml
+tests/functions/method-fixtures/method-nested-hook.yaml
+tests/functions/method-fixtures/method-nested-override.yaml
+tests/functions/method-fixtures/method-single.yaml
+tests/functions/types-fixtures/base-embed.yaml
+tests/functions/types-fixtures/base.yaml
+tests/functions/types-fixtures/dict-base.yaml
+tests/functions/types-fixtures/enum-basic.yaml
+tests/functions/types-fixtures/enum-types.yaml
+tests/functions/types-fixtures/list-base.yaml
 tests/macros/README.md
 tests/macros/test_macros.py
 tests/macros/fixtures/func-inputs-basic.yaml
 tests/main/test_main.py
 tests/main/fixtures/.tackle.yaml
 tests/main/fixtures/block-input-overrides.yaml
 tests/main/fixtures/block-input.yaml
@@ -484,30 +600,45 @@
 tests/models/fixtures/test-provider/context_provider.yaml
 tests/models/fixtures/test-provider-2/hooks/stuff.py
 tests/models/fixtures/test-provider-reqs/requirements.txt
 tests/models/fixtures/test-provider-reqs/tackle.yaml
 tests/models/fixtures/test-provider-reqs/hooks/hooks.py
 tests/models/fixtures/test-provider/hooks/thing.py
 tests/parser/test_parser_args_handler.py
+tests/parser/test_parser_base_methods.py
 tests/parser/test_parser_exceptions.py
 tests/parser/test_parser_hook_arguments.py
 tests/parser/test_parser_macros.py
-tests/parser/test_parser_methods.py
 tests/parser/test_parser_parse_hook.py
 tests/parser/test_source.py
-tests/parser/exceptions/a-list.yaml
-tests/parser/exceptions/a-tackle.yaml
-tests/parser/exceptions/empty-with-functions.yaml
-tests/parser/exceptions/empty.yaml
-tests/parser/exceptions/function-input-validation-error.yaml
-tests/parser/exceptions/hook-input-validation-error.yaml
-tests/parser/exceptions/merge-error.yaml
-tests/parser/exceptions/out-of-range-arg.yaml
-tests/parser/exceptions/calling_dir/.gitkeep
-tests/parser/exceptions/calling_dir/calling.yaml
+tests/parser/base-method-fixtures/list-comprehension.yaml
+tests/parser/base-method-fixtures/merge-dict-loop-dict.yaml
+tests/parser/base-method-fixtures/merge-dict-loop-exception.yaml
+tests/parser/base-method-fixtures/merge-dict.yaml
+tests/parser/base-method-fixtures/merge-list-dict.yaml
+tests/parser/base-method-fixtures/merge-list-loop-dict.yaml
+tests/parser/base-method-fixtures/merge-list-loop-value.yaml
+tests/parser/base-method-fixtures/merge-list-loop.yaml
+tests/parser/base-method-fixtures/merge-list-value.yaml
+tests/parser/base-method-fixtures/method-else.yaml
+tests/parser/base-method-fixtures/method-except.yaml
+tests/parser/base-method-fixtures/method-try.yaml
+tests/parser/base-method-fixtures/method-when.yaml
+tests/parser/base-method-fixtures/try-validation-except.yaml
+tests/parser/exceptions-fixtures/a-list.yaml
+tests/parser/exceptions-fixtures/a-tackle.yaml
+tests/parser/exceptions-fixtures/empty-hook-call.yaml
+tests/parser/exceptions-fixtures/empty-with-functions.yaml
+tests/parser/exceptions-fixtures/empty.yaml
+tests/parser/exceptions-fixtures/function-input-validation-error.yaml
+tests/parser/exceptions-fixtures/hook-input-validation-error.yaml
+tests/parser/exceptions-fixtures/merge-error.yaml
+tests/parser/exceptions-fixtures/out-of-range-arg.yaml
+tests/parser/exceptions-fixtures/calling_dir/.gitkeep
+tests/parser/exceptions-fixtures/calling_dir/calling.yaml
 tests/parser/fixtures/ansible-playbook.yaml
 tests/parser/fixtures/arg-types-output.yaml
 tests/parser/fixtures/arg-types.yaml
 tests/parser/fixtures/args.yaml
 tests/parser/fixtures/block-output.yaml
 tests/parser/fixtures/block.yaml
 tests/parser/fixtures/bug-mixed-flags-output.yaml
@@ -530,19 +661,14 @@
 tests/parser/fixtures/map-lists-output.yaml
 tests/parser/fixtures/map-lists.yaml
 tests/parser/fixtures/map-output.yaml
 tests/parser/fixtures/map-root-output.yaml
 tests/parser/fixtures/map-root.yaml
 tests/parser/fixtures/map.yaml
 tests/parser/fixtures/match-case-logic.yaml
-tests/parser/fixtures/merge-dict-loop-dict.yaml
-tests/parser/fixtures/merge-dict-loop-exception.yaml
-tests/parser/fixtures/merge-key-simple.yaml
-tests/parser/fixtures/merge-list-loop.yaml
-tests/parser/fixtures/merge-list-value.yaml
 tests/parser/fixtures/merge-petstore-compact.yaml
 tests/parser/fixtures/merge-petstore.yaml
 tests/parser/fixtures/merge-simple-output.yaml
 tests/parser/fixtures/merge-simple.yaml
 tests/parser/fixtures/outer-tackle-arg.yaml
 tests/parser/fixtures/outer-tackle-list-output.yaml
 tests/parser/fixtures/outer-tackle-list.yaml
@@ -556,14 +682,15 @@
 tests/parser/fixtures/remote.yaml
 tests/parser/fixtures/ruamel-parsing-error-braces.yaml
 tests/parser/fixtures/toml.toml
 tests/parser/fixtures/toml.yaml
 tests/parser/fixtures/types.yaml
 tests/parser/fixtures/var-hook-output.yaml
 tests/parser/fixtures/var-hook.yaml
+tests/parser/fixtures/.old/merge-key-simple.yaml
 tests/parser/fixtures/blocks/ansible-parse-call.yaml
 tests/parser/fixtures/blocks/ansible-parse-output.yaml
 tests/parser/fixtures/blocks/ansible-parse.yaml
 tests/parser/fixtures/blocks/empty-block-exception.yaml
 tests/parser/fixtures/blocks/nested-dict-output.yaml
 tests/parser/fixtures/blocks/nested-dict.yaml
 tests/parser/fixtures/blocks/nested-for-output.yaml
@@ -573,106 +700,14 @@
 tests/parser/fixtures/dir/tackle.yaml
 tests/parser/fixtures/input-key/tackle.yaml
 tests/parser/fixtures/input-key/child/.gitkeep
 tests/parser/fixtures/input-key/child/calling.yaml
 tests/parser/fixtures/macros/compact-hook-macro.yaml
 tests/parser/fixtures/macros/list-block.yaml
 tests/parser/fixtures/templates/file.py
-tests/parser/functions/test_function_calls.py
-tests/parser/functions/test_functions.py
-tests/parser/functions/test_functions_args_kwargs_hooks.py
-tests/parser/functions/test_functions_cli.py
-tests/parser/functions/test_functions_exceptions.py
-tests/parser/functions/test_functions_field_hooks.py
-tests/parser/functions/test_functions_help.py
-tests/parser/functions/exceptions/hook-kwarg-missing-default.yaml
-tests/parser/functions/exceptions/hook-kwarg-missing.yaml
-tests/parser/functions/exceptions/missing-field.yaml
-tests/parser/functions/exceptions/str-value.yaml
-tests/parser/functions/exceptions/try-in-default.yaml
-tests/parser/functions/field-hooks-fixtures/extends-visible.yaml
-tests/parser/functions/field-hooks-fixtures/extends.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-args-method.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-args.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-exec-args-method.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-exec-args.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-exec-method.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-exec.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks-method.yaml
-tests/parser/functions/field-hooks-fixtures/field-hooks.yaml
-tests/parser/functions/field-hooks-fixtures/passed-context.yaml
-tests/parser/functions/field-hooks-fixtures/.hooks/base-hook.yaml
-tests/parser/functions/fixtures/call-output.yaml
-tests/parser/functions/fixtures/call.yaml
-tests/parser/functions/fixtures/cli-call-func-output.yaml
-tests/parser/functions/fixtures/cli-call-func.yaml
-tests/parser/functions/fixtures/cli-default-hook-args.yaml
-tests/parser/functions/fixtures/cli-default-hook-context.yaml
-tests/parser/functions/fixtures/cli-default-hook-embedded.yaml
-tests/parser/functions/fixtures/cli-default-hook-no-context.yaml
-tests/parser/functions/fixtures/cli-hook-no-context.yaml
-tests/parser/functions/fixtures/cli-hook-type-unknown.yaml
-tests/parser/functions/fixtures/cli-no-default-hook.yaml
-tests/parser/functions/fixtures/compact.yaml
-tests/parser/functions/fixtures/default-method-json.yaml
-tests/parser/functions/fixtures/default-method-self.yaml
-tests/parser/functions/fixtures/extends.yaml
-tests/parser/functions/fixtures/field-bad-type.yaml
-tests/parser/functions/fixtures/field-require.yaml
-tests/parser/functions/fixtures/field-type-or-default.yaml
-tests/parser/functions/fixtures/field-types.yaml
-tests/parser/functions/fixtures/flatten.yaml
-tests/parser/functions/fixtures/list-call.yaml
-tests/parser/functions/fixtures/method-args.yaml
-tests/parser/functions/fixtures/method-base-validate.yaml
-tests/parser/functions/fixtures/method-call-from-default.yaml
-tests/parser/functions/fixtures/method-call-no-default.yaml
-tests/parser/functions/fixtures/method-embed.yaml
-tests/parser/functions/fixtures/method-hook.yaml
-tests/parser/functions/fixtures/method-inherit.yaml
-tests/parser/functions/fixtures/method-maintain-context.yaml
-tests/parser/functions/fixtures/method-nested-hook.yaml
-tests/parser/functions/fixtures/method-nested-override.yaml
-tests/parser/functions/fixtures/method-single.yaml
-tests/parser/functions/fixtures/no-exec-type-error.yaml
-tests/parser/functions/fixtures/no-exec.yaml
-tests/parser/functions/fixtures/return-output.yaml
-tests/parser/functions/fixtures/return-render.yaml
-tests/parser/functions/fixtures/return-str-not-found.yaml
-tests/parser/functions/fixtures/return.yaml
-tests/parser/functions/fixtures/supplied-args-param-list.yaml
-tests/parser/functions/fixtures/supplied-args-param-str.yaml
-tests/parser/functions/fixtures/supplied-kwargs-param-dict.yaml
-tests/parser/functions/fixtures/supplied-kwargs-param-str.yaml
-tests/parser/functions/fixtures/.hooks/some-hooks.yaml
-tests/parser/functions/fixtures/a-tackle/tackle.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-dict-error-default.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-dict-error-str.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-dict-error-type.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-list-error-default.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-list-error-str.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-list-error-type.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-str-error-default.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-str-error-str.yaml
-tests/parser/functions/fixtures/field-type-exceptions/field-types-str-error-type.yaml
-tests/parser/functions/fixtures/func-provider/tackle.yaml
-tests/parser/functions/fixtures/func-provider-hook/tackle.yaml
-tests/parser/functions/fixtures/func-provider-hook/a-dir/.gitkeep
-tests/parser/functions/fixtures/func-provider-hook/hooks/funks.yaml
-tests/parser/functions/fixtures/func-provider-method/tackle.yaml
-tests/parser/functions/fixtures/func-provider-method/a-dir/.gitkeep
-tests/parser/functions/fixtures/func-provider-method/hooks/funks.yaml
-tests/parser/functions/fixtures/func-provider/a-dir/.gitkeep
-tests/parser/functions/fixtures/func-provider/hooks/funks.yaml
-tests/parser/method-fixtures/list-comprehension.yaml
-tests/parser/method-fixtures/method-else.yaml
-tests/parser/method-fixtures/method-except.yaml
-tests/parser/method-fixtures/method-try.yaml
-tests/parser/method-fixtures/method-when.yaml
-tests/parser/method-fixtures/try-validation-except.yaml
 tests/render/test_environment.py
 tests/render/test_extensions.py
 tests/render/test_render.py
 tests/render/test_render_exceptions.py
 tests/render/test_special_variables.py
 tests/render/fixtures/call-function-output.yaml
 tests/render/fixtures/call-function.yaml
```

### Comparing `tackle-0.4.9/tests/cli/test_cli.py` & `tackle-0.5.0/tests/cli/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 ]
 # fmt: on
 
 
 @pytest.mark.parametrize("input_string,output", INPUT_SOURCES)
 def test_cli_parse_args(mocker, change_dir_base, input_string, output):
     """Mock the main call and verify the args get passed in right through the CLI."""
-    mock = mocker.patch("tackle.main.update_source", autospec=True, return_value={})
+    mock = mocker.patch("tackle.main.parse_source", autospec=True, return_value={})
     main(input_string.split(' '))
 
     assert mock.called
     assert isinstance(mock.call_args[0][0], Context)
 
     context = mock.call_args[0][0].dict()
 
     for k, v in output.items():
         assert k in context
         assert context[k] == v
 
 
 def test_cli_parse_args_empty(mocker, change_curdir_fixtures):
     """When no arg is given we should find the closest tackle file."""
-    mock = mocker.patch("tackle.main.update_source", autospec=True, return_value={})
+    mock = mocker.patch("tackle.main.parse_source", autospec=True, return_value={})
     main([])
 
     assert mock.called
     assert isinstance(mock.call_args[0][0], Context)
     context = mock.call_args[0][0].dict()
     assert context['input_string'] == os.path.abspath('.tackle.yaml')
```

### Comparing `tackle-0.4.9/tests/cli/test_cli_args.py` & `tackle-0.5.0/tests/cli/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/cli/test_cli_commands.py` & `tackle-0.5.0/tests/cli/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/exceptions/test_tackle_exceptions.py` & `tackle-0.5.0/tests/exceptions/test_tackle_exceptions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/macros/test_macros.py` & `tackle-0.5.0/tests/macros/test_macros.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/main/test_main.py` & `tackle-0.5.0/tests/main/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from tackle import tackle
 from tackle.cli import main
 from tackle import exceptions
 
 
 def test_main_cli_call_mock(mocker):
     """Check the main function runs properly."""
-    mock = mocker.patch("tackle.main.update_source")
+    mock = mocker.patch("tackle.main.parse_source")
     main("stuff")
     assert mock.called
 
 
 def test_main_cli_call_empty(change_curdir_fixtures, mocker):
     """
     Check that when no arg is given that we find the closes tackle file which
     could be in the parent directory.
     """
-    mock = mocker.patch("tackle.main.update_source")
+    mock = mocker.patch("tackle.main.parse_source")
     main([])
     assert mock.called
     local_tackle = os.path.join(os.path.abspath('.'), '.tackle.yaml')
 
     if sys.version_info.minor > 7:
         assert mock.call_args.args[0].input_string == local_tackle
     # test was failing in 3.7/6
```

### Comparing `tackle-0.4.9/tests/models/fixtures/text2art.yaml` & `tackle-0.5.0/tests/models/fixtures/text2art.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/models/test_models.py` & `tackle-0.5.0/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/models/test_models_providers.py` & `tackle-0.5.0/tests/models/test_models_providers.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/block-output.yaml` & `tackle-0.5.0/tests/parser/fixtures/block-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/block.yaml` & `tackle-0.5.0/tests/parser/fixtures/block.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/blocks/ansible-parse-output.yaml` & `tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/blocks/ansible-parse.yaml` & `tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/blocks/nested-for-output.yaml` & `tackle-0.5.0/tests/parser/fixtures/blocks/nested-for-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/blocks/nested-for.yaml` & `tackle-0.5.0/tests/parser/fixtures/blocks/nested-for.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/docker-compose.yml` & `tackle-0.5.0/tests/parser/fixtures/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/empty-hooks-output.yaml` & `tackle-0.5.0/tests/parser/fixtures/empty-hooks-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/empty-hooks.yaml` & `tackle-0.5.0/tests/parser/fixtures/empty-hooks.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/fixtures/petstore.yaml` & `tackle-0.5.0/tests/parser/fixtures/petstore.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/functions/field-hooks-fixtures/extends-visible.yaml` & `tackle-0.5.0/tests/functions/field-hooks-fixtures/extends-visible.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/functions/fixtures/cli-default-hook-embedded.yaml` & `tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-embedded.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/functions/fixtures/cli-default-hook-no-context.yaml` & `tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-no-context.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/functions/fixtures/field-types.yaml` & `tackle-0.5.0/tests/functions/fixtures/field-types.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/functions/fixtures/method-nested-override.yaml` & `tackle-0.5.0/tests/functions/method-fixtures/method-nested-override.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -7,35 +7,35 @@
     home:
       type: str
 
     out<-:
       home: earth
 
 method_overlap_jinja->: "{{method_overlap.call.out()}}"
-method_overlap_compact->: method_overlap.call.out --home foo
+method_overlap_compact->: method_overlap call out --home foo
 
 attribute_override<-:
   home:
     default: bar
 
   call<-:
     home:
       default: baz
 
     out<-:
       home:
         default: bing
 
 attribute_override_jinja->: "{{attribute_override.call.out()}}"
-attribute_override_compact->: attribute_override.call.out
+attribute_override_compact->: attribute_override call out
 
 nested<-:
   home:
     default: bar
 
   call<-:
     out<-:
       home:
         default: baz
 
 nested_jinja->: "{{nested.call.out()}}"
-nexted_compact->: nested.call.out
+nexted_compact->: nested call out
```

### Comparing `tackle-0.4.9/tests/parser/functions/test_functions.py` & `tackle-0.5.0/tests/functions/test_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,118 +41,150 @@
 
 def test_function_extends(change_curdir_fixtures):
     """Check that we can extend a base function."""
     output = tackle('extends.yaml')
     assert output['t'] == ['hello', 'world']
 
 
-def test_function_method(change_curdir_fixtures):
+def test_function_method(chdir):
     """Check that methods work"""
+    chdir('method-fixtures')
     output = tackle('method-hook.yaml')
     assert output['t'] == {'in': 'foo', 'bar': 'baz'}
     assert output['t'] == output['jinja_method']
     assert output['jinja_base']['bar'] == 'foo'
 
 
-def test_function_method_simple(change_curdir_fixtures):
+def test_function_method_simple(chdir):
     """Check that we can create a method."""
+    chdir('method-fixtures')
     output = tackle('method-single.yaml')
     assert output['do'] == {"v": ["Hello", "world!"]}
 
 
-def test_function_method_embed(change_curdir_fixtures):
+def test_function_method_embed(chdir):
     """Check that we can create a method."""
+    chdir('method-fixtures')
     output = tackle('method-embed.yaml')
     assert output['do']['v'] == ['Hello', 'world!']
 
 
-def test_function_method_inherit(change_curdir_fixtures):
+def test_function_method_inherit(chdir):
     """Check that we can create a method."""
+    chdir('method-fixtures')
     output = tackle('method-inherit.yaml')
     assert output == {"t": "fooo"}
 
 
-def test_function_method_args(change_curdir_fixtures):
+def test_function_method_args(chdir):
     """Check that we can create a method that takes args."""
+    chdir('method-fixtures')
     output = tackle('method-args.yaml')
     assert output == {'foo': 'bar'}
 
 
-def test_function_method_call_from_default(change_curdir_fixtures):
+def test_function_method_call_from_default(chdir):
     """
     Check that we can create a method that takes args.
     See https://github.com/robcxyz/tackle/issues/99
     """
+    chdir('method-fixtures')
     output = tackle('method-call-from-default.yaml', target='foo')
     assert output['hi'] == 'Hello foo'
 
 
-def test_function_method_maintain_context(change_curdir_fixtures):
+def test_function_method_maintain_context(chdir):
     """Check a method that carries a context with it from the parent object."""
+    chdir('method-fixtures')
     output = tackle('method-maintain-context.yaml')
     assert output['do_greeter']['v'] == ['Hello', 'world!']
     assert output['jinja_call']['v'] == ['Hello', 'world!']
 
 
-def test_function_method_nested(change_curdir_fixtures):
+def test_function_method_nested(chdir):
     """Check that we can create a method."""
+    chdir('method-fixtures')
     output = tackle('method-nested-hook.yaml')
     assert output['jinja_method_home']['destination'] == "earth"
     assert output['jinja_method_home'] == output['t_home']
 
 
-def test_function_method_override(change_curdir_fixtures):
+def test_function_method_override(chdir):
     """
     Check that when we call methods that attributes are properly overridden if they
      exist in the base.
     """
+    chdir('method-fixtures')
     output = tackle('method-nested-override.yaml')
     assert output['method_overlap_jinja']['home'] == 'earth'
     assert output['method_overlap_compact']['home'] == 'foo'
     assert output['attribute_override_jinja']['home'] == 'bing'
     assert output['attribute_override_compact']['home'] == 'bing'
     assert output['nested_jinja']['home'] == 'baz'
     assert output['nexted_compact']['home'] == 'baz'
 
 
-def test_function_import_func_from_hooks_dir(change_curdir_fixtures):
+def test_function_import_func_from_hooks_dir_call_in_tackle(change_curdir_fixtures):
     """Assert that we can call functions from local hooks dir."""
     os.chdir('func-provider')
     o = tackle()
     assert o['compact'] == 'a-default'
     assert o['jinja_extension_default'] == 'a-default'
     assert o['jinja_extension'] == 'things'
     # assert o['jinja_filter'] == 'things'
 
 
 def test_function_import_func_from_hooks_dir_context_preserved(change_curdir_fixtures):
     """
     Check that when we run inside a nested dir, that a declarative hook carries context
-    such as calling_directory.
+     such as calling_directory.
     """
     os.chdir(os.path.join('func-provider-hook', 'a-dir'))
     o = tackle()
     assert o['compact'] == 'a-default'
     assert o['jinja_extension_default'] == 'a-default'
     assert o['jinja_extension'] == 'things'
     assert o['calling_dir'].endswith('a-dir')
 
 
-def test_function_import_func_from_hooks_dir_context_preserved2(change_curdir_fixtures):
+def test_function_import_func_from_hooks_dir_call_method(change_curdir_fixtures):
+    """Check that we can call a method on an imported hook from a hooks directory."""
+    os.chdir(os.path.join('func-provider-method', 'a-dir'))
+    o = tackle(a_field='an-arg')
+    assert o['t']['p'] == 'a-default'
+
+
+def test_function_import_func_from_hooks_dir_call_function_cli(change_curdir_fixtures):
     """
-    Check that when we run inside a nested dir, that a declarative hook carries context
-    such as calling_directory.
+    Check that we can call a function on an imported hook from a hooks directory when
+     calling with args like in CLI.
     """
     os.chdir(os.path.join('func-provider-method', 'a-dir'))
-    o = tackle()
-    assert o
+    o = tackle('a_funky')
+    assert o == 'a-default'
+
 
+def test_function_import_func_from_hooks_dir_call_method_cli(change_curdir_fixtures):
+    """Check that we can call a method on an imported hook from a hooks directory."""
+    os.chdir(os.path.join('func-provider-method', 'a-dir'))
+    o = tackle('a_funky', 'func_method')
+    assert o['p'] == 'a-default'
+
+
+def test_function_import_func_from_hooks_dir_method_main(change_curdir_fixtures):
+    """Check running a hook via main method."""
+    from tackle.cli import main
+
+    os.chdir(os.path.join('func-provider-method', 'a-dir'))
+    main(['a_funky'])
 
-def test_function_method_no_default(change_curdir_fixtures):
+
+def test_function_method_no_default(chdir):
     """Assert that method calls with base fields with no default can be run."""
+    chdir('method-fixtures')
     o = tackle('method-call-no-default.yaml')
     assert o['compact']['v'] == 'foo'
     assert o['compact'] == o['expanded']
     assert o['jinja_base']['word'] == 'foo'
     assert o['jinja_method']['v'] == 'foo'
 
 
@@ -164,7 +196,24 @@
 
 
 # TODO: Build compact hook macro
 # def test_function_compact(change_curdir_fixtures):
 #     """Check what compact hooks do."""
 #     output = tackle('compact.yaml')
 #     assert output
+
+@pytest.fixture()
+def extends_fixtures(chdir):
+    chdir('extends-fixtures')
+
+
+def test_function_extends_str(extends_fixtures):
+    """Check that we can extend a base function."""
+    output = tackle('extends.yaml')
+    assert output['t'] == ['hello', 'world']
+
+
+def test_function_extends_list(extends_fixtures):
+    """Check that we can extend a base function with a list of other functions."""
+    output = tackle('extends-list.yaml')
+    assert output['t'] == ['hello', 'dude']
+
```

### Comparing `tackle-0.4.9/tests/parser/functions/test_functions_args_kwargs_hooks.py` & `tackle-0.5.0/tests/functions/test_functions_args_kwargs_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,21 @@
      a dict that will update the field's values.
     """
     output = tackle('supplied-kwargs-param-str.yaml')
     assert output['kwarg']['bar'] == 'bing'
     assert output['kwarg'] == output['call']
 
 
+def test_function_supplied_kwargs_param_str_loop(change_curdir_fixtures):
+    """Check that we can use kwargs within a loop"""
+    output = tackle('supplied-kwargs-param-str-loop.yaml')
+    assert output['call'][0]['bar'] == 'bing'
+    assert len(output['call']) == 2
+
+
 def test_function_supplied_args_param_str(change_curdir_fixtures):
     """Test that we can populate a functions args with an `args` key as str."""
     output = tackle('supplied-args-param-str.yaml')
     assert output['call']['bar'] == 'bing'
 
 
 def test_function_supplied_args_param_list(change_curdir_fixtures):
```

### Comparing `tackle-0.4.9/tests/parser/functions/test_functions_cli.py` & `tackle-0.5.0/tests/functions/test_functions_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 FIXTURES = [
     ('cli-call-func.yaml', 'cli-call-func-output.yaml', 'func_a'),
 ]
 
 
 @pytest.mark.parametrize("fixture,expected_output,argument", FIXTURES)
-def test_function_model_extraction(
-    change_curdir_fixtures, fixture, expected_output, argument, capsys
-):
+def test_function_model_extraction(chdir, fixture, expected_output, argument, capsys):
+    chdir('cli-fixtures')
     main([fixture, argument, "-p"])
     output = capsys.readouterr().out
 
     yaml = YAML()
     with open(expected_output) as f:
         expected_output = yaml.load(f)
 
     assert json.loads(output) == expected_output
 
 
 @pytest.mark.parametrize("fixture,expected_output,argument", FIXTURES)
 def test_function_model_extraction_in_directory(
-    change_curdir_fixtures, chdir, fixture, expected_output, argument, capsys
+    chdir, fixture, expected_output, argument, capsys
 ):
+    chdir('cli-fixtures')
     yaml = YAML()
     with open(expected_output) as f:
         expected_output = yaml.load(f)
 
-    os.chdir("func-provider")
+    os.chdir("a-dir")
     main([fixture, argument, "-p", "--find-in-parent"])
     output = capsys.readouterr().out
 
     assert json.loads(output) == expected_output
 
 
 def test_function_cli_multiple_args(change_curdir_fixtures, capsys):
```

### Comparing `tackle-0.4.9/tests/parser/functions/test_functions_exceptions.py` & `tackle-0.5.0/tests/functions/test_functions_exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,49 @@
     ('return-str-not-found.yaml', exceptions.FunctionCallException),
     # Check that type checking works with no exec method.
     ('no-exec-type-error.yaml', exceptions.HookParseException),
     # Check args are required when they are not supplied.
     ('field-require.yaml', exceptions.HookParseException),
     # Check that type is one of literals.
     ('field-bad-type.yaml', exceptions.MalformedFunctionFieldException),
+    # Check when extends is used with a missing base.
+    ('extends-missing.yaml', exceptions.MalformedFunctionFieldException),
+    # Check when extends is a dict an error is thrown
+    ('extends-dict.yaml', exceptions.MalformedFunctionFieldException),
 ]
 
 
 @pytest.mark.parametrize("fixture,exception", EXCEPTION_FIXTURES)
-def test_function_raises_exceptions(change_curdir_fixtures, fixture, exception):
+def test_function_raises_exceptions(chdir, fixture, exception):
+    chdir('exceptions')
     with pytest.raises(exception):
         tackle(fixture)
 
 
+def test_function_method_base_validate(chdir):
+    """Check that when a method uses a base attribute, that validation still happens."""
+    chdir('method-fixtures')
+    with pytest.raises(Exception) as e:
+        tackle('method-base-validate.yaml')
+    assert 'string does not match regex' in e.value.message
+
+
 FIELD_TYPE_EXCEPTION_FIXTURES = [
     ('str', 'str'),
     ('dict', 'str'),
     ('list', 'str'),
     ('str', 'type'),
     ('dict', 'type'),
     ('list', 'type'),
     ('str', 'default'),
     ('dict', 'default'),
     ('list', 'default'),
 ]
 
 
-def test_function_method_base_validate(change_curdir_fixtures):
-    """Check that when a method uses a base attribute, that validation still happens."""
-    with pytest.raises(Exception) as e:
-        tackle('method-base-validate.yaml')
-    assert 'string does not match regex' in e.value.message
-
-
 @pytest.mark.parametrize("type_,field_input", FIELD_TYPE_EXCEPTION_FIXTURES)
 def test_function_raises_exceptions_field_types(chdir, type_, field_input):
     """Check that a validation error is returned for each type of field definition."""
     chdir(os.path.join('fixtures', 'field-type-exceptions'))
     with pytest.raises(exceptions.HookParseException):
         tackle(f'field-types-{type_}-error-{field_input}.yaml')
 
@@ -57,40 +63,46 @@
     catch that.
     """
     chdir('exceptions')
     with pytest.raises(exceptions.FunctionCallException):
         tackle('try-in-default.yaml')
 
 
-def test_parser_functions_raises_unknown_arg(change_curdir_fixtures):
+def test_parser_functions_raises_unknown_arg(chdir):
+    chdir('cli-fixtures')
     with pytest.raises(exceptions.UnknownInputArgumentException):
         tackle("cli-default-hook-no-context.yaml", 'NOT_HERE')
 
 
-def test_parser_functions_raises_unknown_kwarg(change_curdir_fixtures):
+def test_parser_functions_raises_unknown_kwarg(chdir):
+    chdir('cli-fixtures')
     with pytest.raises(exceptions.UnknownInputArgumentException):
         tackle("cli-default-hook-no-context.yaml", NOT_HERE='foo')
 
 
-def test_parser_functions_raises_unknown_flags(change_curdir_fixtures):
+def test_parser_functions_raises_unknown_flags(chdir):
+    chdir('cli-fixtures')
     with pytest.raises(exceptions.UnknownInputArgumentException):
         tackle("cli-default-hook-no-context.yaml", global_flags=['NOT_HERE'])
 
 
-def test_parser_functions_raises_unknown_arg_hook(change_curdir_fixtures):
+def test_parser_functions_raises_unknown_arg_hook(chdir):
+    chdir('cli-fixtures')
     with pytest.raises(exceptions.UnknownInputArgumentException):
         tackle("cli-hook-no-context.yaml", 'run', 'NOT_HERE')
 
 
-def test_parser_functions_raises_unknown_kwarg_hook(change_curdir_fixtures):
+def test_parser_functions_raises_unknown_kwarg_hook(chdir):
+    chdir('cli-fixtures')
     with pytest.raises(exceptions.UnknownInputArgumentException):
         tackle("cli-hook-no-context.yaml", 'run', NOT_HERE='foo')
 
 
-def test_parser_functions_raises_unknown_flags_hook(change_curdir_fixtures):
+def test_parser_functions_raises_unknown_flags_hook(chdir):
+    chdir('cli-fixtures')
     with pytest.raises(exceptions.UnknownInputArgumentException):
         tackle("cli-hook-no-context.yaml", 'run', global_flags=['NOT_HERE'])
 
 
 def test_parser_functions_raises_hook_kwarg_missing(chdir):
     chdir('exceptions')
     with pytest.raises(exceptions.UnknownInputArgumentException):
```

### Comparing `tackle-0.4.9/tests/parser/functions/test_functions_field_hooks.py` & `tackle-0.5.0/tests/functions/test_functions_field_hooks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/method-fixtures/method-else.yaml` & `tackle-0.5.0/tests/parser/base-method-fixtures/method-else.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/method-fixtures/method-except.yaml` & `tackle-0.5.0/tests/parser/base-method-fixtures/method-except.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/test_parser_args_handler.py` & `tackle-0.5.0/tests/parser/test_parser_args_handler.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/test_parser_exceptions.py` & `tackle-0.5.0/tests/parser/test_parser_exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Test the input source part of the parser."""
 import pytest
 
-from tackle.exceptions import (
-    EmptyTackleFileException,
-    UnknownArgumentException,
-    UnknownSourceException,
-    HookParseException,
-)
+from tackle import exceptions
 
 # from tackle import tackle
 from tackle.cli import main
 
 INPUT_SOURCES = [
     # TODO: empty should now be running help screen
-    # ("empty-with-functions.yaml", EmptyTackleFileException),
-    ("empty.yaml", EmptyTackleFileException),
-    ("out-of-range-arg.yaml", UnknownArgumentException),
-    ("non-existent.yaml", UnknownSourceException),
-    ("hook-input-validation-error.yaml", HookParseException),
-    ("function-input-validation-error.yaml", HookParseException),
+    # ("empty-with-functions.yaml", exceptions.EmptyTackleFileException),
+    ("empty-hook-call.yaml", exceptions.HookCallException),
+    ("empty.yaml", exceptions.EmptyTackleFileException),
+    ("out-of-range-arg.yaml", exceptions.UnknownArgumentException),
+    ("non-existent.yaml", exceptions.UnknownSourceException),
+    ("hook-input-validation-error.yaml", exceptions.HookParseException),
+    ("function-input-validation-error.yaml", exceptions.HookParseException),
 ]
 
 
 @pytest.mark.parametrize("input_file,exception", INPUT_SOURCES)
 def test_parser_raises_exceptions(chdir, input_file, exception):
     """Test raising exceptions."""
-    chdir('exceptions')
+    chdir('exceptions-fixtures')
     with pytest.raises(exception):
         main([input_file])
```

### Comparing `tackle-0.4.9/tests/parser/test_parser_hook_arguments.py` & `tackle-0.5.0/tests/parser/test_parser_hook_arguments.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/test_parser_macros.py` & `tackle-0.5.0/tests/parser/test_parser_macros.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/parser/test_parser_methods.py` & `tackle-0.5.0/tests/parser/test_parser_base_methods.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,94 +10,118 @@
     with open('petstore.yaml') as f:
         expected_output = yaml.load(f)
 
     output = tackle('merge-petstore-compact.yaml')
     assert output == expected_output
 
 
-def test_parser_methods_merge_list_value(change_curdir_fixtures):
+@pytest.fixture()
+def fixture_dir(chdir):
+    chdir("base-method-fixtures")
+
+
+def test_parser_methods_merge_dict(fixture_dir):
+    """Validate merging a dict into a dict."""
+    output = tackle('merge-dict.yaml')
+    assert output['resources']['name'] == 'operator'
+    assert output['resources']['foo'] == 'foo'
+
+
+def test_parser_methods_merge_list_value(fixture_dir):
     """Validate that when in a list, running a hook with a merge overwrites the list."""
     # Note: this is kind of strong... But what else is it supposed to mean? Don't use
     # merge for values...
     output = tackle('merge-list-value.yaml')
     assert output['resources'] == 'foo'
 
 
-def test_parser_methods_merge_list_loop(change_curdir_fixtures):
+def test_parser_methods_merge_list_loop_value(fixture_dir):
     """
     Validate that when in a list, running a hook in a for loop with a merge appends to
      the list.
     """
-    output = tackle('merge-list-loop.yaml')
+    output = tackle('merge-list-loop-value.yaml')
     assert len(output['resources']) == 5
+    assert output['resources'][2] == 'foo-0'
 
 
-def test_parser_methods_merge_dict_loop_dict(change_curdir_fixtures):
+def test_parser_methods_merge_list_loop_dict(fixture_dir):
+    """Same as above but with a dict."""
+    output = tackle('merge-list-loop-dict.yaml')
+    assert len(output['resources']) == 5
+    assert output['resources'][2]['foo-0'] == 'foo-0'
+    assert output['resources'][3]['foo-1'] == 'foo-1'
+
+
+def test_parser_methods_merge_dict_loop_dict(fixture_dir):
     """
     Validate that when in a dict, running a hook in a for loop with a merge adds new
      keys to the output.
     """
-    # TODO: Associated with https://github.com/robcxyz/tackle/issues/107
     output = tackle('merge-dict-loop-dict.yaml')
-    assert output['resources']['foo-2']
+    assert output['resources']['foo-2'] == 'foo-2'
+    assert output['resources']['name'] == 'operator'
+    assert output['resources']['foo-1'] == 'foo-1'
 
 
-def test_parser_methods_merge_dict_loop_exception(change_curdir_fixtures):
+def test_parser_methods_merge_dict_loop_exception(fixture_dir):
     """
     Validate exception that when in a dict, running a hook in a for loop with a merge
      with the hook output being a value.
     """
     with pytest.raises(exceptions.AppendMergeException):
         tackle('merge-dict-loop-exception.yaml')
 
 
-def test_parser_methods_try(chdir):
+# def test_parser_methods_merge_list_dict(fixture_dir):
+#     """Validate when we merge a list into a dict that it overwrites the contents."""
+#     output = tackle('merge-list-dict.yaml')
+#     # TODO: Determine how to merge twice into a list
+#     #  https://github.com/sudoblockio/tackle/issues/163
+#     assert output
+
+
+def test_parser_methods_try(fixture_dir):
     """Use try which should not have any output"""
-    chdir("method-fixtures")
     output = tackle('method-try.yaml')
     assert output == {}
 
 
-def test_parser_methods_except(chdir):
+def test_parser_methods_except(fixture_dir):
     """Use try which should not have any output"""
-    chdir("method-fixtures")
     output = tackle('method-except.yaml')
     assert output['compact'] == 'foo'
     assert output['str'] == 'foo'
     assert output['dic']['stuff'] == '{{stuff}}'
     assert output['dict_render_block'] == {'stuff': '{{stuff}}'}
     assert output['stuff'] == 'things'
     assert output['listed']['hook_call'][1]['stuff'] == 'things'
 
 
-def test_parser_methods_when(chdir):
+def test_parser_methods_when(fixture_dir):
     """Use try which should not have any output"""
-    chdir("method-fixtures")
     output = tackle('method-when.yaml')
     assert 'expanded' not in output
 
 
-def test_parser_methods_else_hooks(chdir):
+def test_parser_methods_else_hooks(fixture_dir):
     """Use try which should not have any output"""
-    chdir("method-fixtures")
     output = tackle('method-else.yaml')
     assert output['compact'] == 'foo'
     assert output['str'] == 'foo'
     assert output['dict_render']['stuff'] == '{{stuff}}'
     assert output['str_render_block'] == 'things'
     assert output['dict_render_block'] == {'stuff': '{{stuff}}'}
     assert output['stuff'] == 'things'
     assert output['listed']['hook_call'][1]['stuff'] == 'things'
 
 
-def test_parser_list_comprehension(chdir):
+def test_parser_list_comprehension(fixture_dir):
     """Test that we can do list comprehensions."""
-    chdir("method-fixtures")
     output = tackle('list-comprehension.yaml')
     assert len(output['nodes']) == 1
 
 
-def test_parser_validation_with_try_except(chdir):
+def test_parser_validation_with_try_except(fixture_dir):
     """Test that we can do list comprehensions."""
-    chdir("method-fixtures")
     output = tackle('try-validation-except.yaml')
     assert 'p' in output['call']
```

### Comparing `tackle-0.4.9/tests/parser/test_source.py` & `tackle-0.5.0/tests/parser/test_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # """Test the input source part of the parser."""
 # # import pytest
 # # import shutil
 #
 # from tackle import tackle
 # # from tackle.cli import main
 #
-# from tackle.parser import update_source
+# from tackle.parser import parse_source
 # from tackle.models import Context
 #
 # # INPUT_SOURCES = [
 # #     ("github.com/robcxyz/tackle-demo", 'my')
 # #     # ("robcxyz/full-stack-fastapi-postgresql", 'base-project')
 # # ]
 # #
 # #
 # # @pytest.mark.parametrize("input_string,output_dir", INPUT_SOURCES)
-# # def test_parser_update_source(change_curdir_fixtures, input_string, output_dir):
+# # def test_parser_parse_source(change_curdir_fixtures, input_string, output_dir):
 # #     """Test various inputs."""
 # #     context = Context(input_string=input_string, no_input=True)
-# #     update_source(context)
+# #     parse_source(context)
 # #     shutil.rmtree(output_dir)
 #
 #
 # def test_parser_find_in_parent(chdir):
 #     chdir('fixtures/input-key/child')
 #     output = tackle('calling.yaml', find_in_parent=True)
 #     assert output
 #
 #
-# def test_parser_update_source_key_to_parent(chdir, mocker):
+# def test_parser_parse_source_key_to_parent(chdir, mocker):
 #     """
 #     Test that when an input string is not a file/provider source that we correctly
 #     traverse to the nearest tackle file and run a key within it.
 #     """
 #     chdir('fixtures/input-key/child')
 #     context = Context(input_string="do_things", no_input=True)
-#     update_source(context)
+#     parse_source(context)
 #     print()
```

### Comparing `tackle-0.4.9/tests/render/fixtures/globals.yaml` & `tackle-0.5.0/tests/render/fixtures/globals.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/render/fixtures/special-variables.yaml` & `tackle-0.5.0/tests/render/fixtures/special-variables.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/render/test_environment.py` & `tackle-0.5.0/tests/render/test_environment.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/render/test_extensions.py` & `tackle-0.5.0/tests/render/test_extensions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/render/test_render.py` & `tackle-0.5.0/tests/render/test_render.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/render/test_render_exceptions.py` & `tackle-0.5.0/tests/render/test_render_exceptions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/files/test_utils_files.py` & `tackle-0.5.0/tests/utils/files/test_utils_files.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/fixtures/fake-repo-tmpl.zip` & `tackle-0.5.0/tests/utils/fixtures/fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/fixtures/protected-fake-repo-tmpl.zip` & `tackle-0.5.0/tests/utils/fixtures/protected-fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/test_log.py` & `tackle-0.5.0/tests/utils/test_log.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/test_paths.py` & `tackle-0.5.0/tests/utils/test_paths.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/test_unzip.py` & `tackle-0.5.0/tests/utils/test_unzip.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/test_utils.py` & `tackle-0.5.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/test_utils_command.py` & `tackle-0.5.0/tests/utils/test_utils_command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/test_utils_dicts.py` & `tackle-0.5.0/tests/utils/test_utils_dicts.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/vcs/test_vcs.py` & `tackle-0.5.0/tests/utils/vcs/test_vcs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.4.9/tests/utils/vcs/test_vcs_provider.py` & `tackle-0.5.0/tests/utils/vcs/test_vcs_provider.py`

 * *Files identical despite different names*

