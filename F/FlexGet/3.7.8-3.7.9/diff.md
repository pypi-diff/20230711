# Comparing `tmp/FlexGet-3.7.8.tar.gz` & `tmp/FlexGet-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-kxhtegp_/FlexGet-3.7.8.tar", last modified: Wed Jun 21 15:12:36 2023, max compression
+gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-exxe270e/FlexGet-3.7.9.tar", last modified: Tue Jul 11 15:14:55 2023, max compression
```

## Comparing `FlexGet-3.7.8.tar` & `FlexGet-3.7.9.tar`

### file list

```diff
@@ -1,982 +1,982 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 15:12:35.000000 FlexGet-3.7.8/FlexGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-21 15:12:19.000000 FlexGet-3.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 15:12:19.000000 FlexGet-3.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-21 15:12:36.000000 FlexGet-3.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-21 15:12:19.000000 FlexGet-3.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-21 15:12:19.000000 FlexGet-3.7.8/dev-requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-21 15:12:19.000000 FlexGet-3.7.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 15:12:27.000000 FlexGet-3.7.8/flexget/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/templates/api_response.html
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/api/templates/swagger-ui.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archive/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/archives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archives/archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archives/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/backlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/backlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/backlog/backlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/backlog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/backlog/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/bittorrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/convert_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/magnet_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/private_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/torrent_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/torrent_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/torrent_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/torrent_scrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/torrent_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/bittorrent/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/emby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83806 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/api_emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/emby_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/emby_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/emby_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/emby_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/emby/from_emby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/estimate_release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/estimate_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/estimate_release/estimate_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/estimate_release/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/estimate_release/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/estimate_release/estimators/est_movies_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/estimate_release/estimators/est_released_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/estimate_release/estimators/est_series_tvmaze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/failed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/failed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/failed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/failed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/failed/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/failed/retry_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/ftp/ftp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/ftp/ftp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/ftp/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23176 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/ftp/sftp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/history/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/history/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/history/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/imdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/from_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/imdb_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/imdb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/imdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/irc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/irc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/irc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/irc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/irc/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/managed_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/list_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/list_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/list_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/list_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/couchpotato_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/entry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/imdb_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/movie_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/pending_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/plex_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/radarr_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/sonarr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/subtitle_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/thetvdb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/managed_lists/lists/yaml_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notification_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/cronitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/gotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/ifttt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/microsoftteams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/notifymyandroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/ntfysh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/prowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/pushalot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/pushsafer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/rapidpush.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/sms_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notifiers/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/notify/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/parsing/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/parsing/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/parsing/parsers/parser_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/parsing/parsers/parser_guessit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/parsing/parsers/parser_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/parsing/plugin_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/pending_approval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/pending_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/pending_approval/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/pending_approval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/pending_approval/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/pending_approval/pending_approval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/rejected/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/rejected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/rejected/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/rejected/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/rejected/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/rejected/remember_rejected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/scheduler/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/seen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/seen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/seen_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/seen/seen_movies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/all_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    47041 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/configure_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    57306 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/gen_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/internal_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/metainfo_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/next_series_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/next_series_seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    53392 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/series_begin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/series_premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/series_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/sites/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/allyoulike.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/alpharatio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/animeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/anirena.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/archetorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/argenteam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/awesomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/bakabt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/btn.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/cinemageddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/cpasbien.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/deadfrog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/descargas2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/ettv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/eztv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/filelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/filelist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/frenchtorrentdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/fuzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/google_cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/hebits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/hliang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/horriblesubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/koreus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/limetorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/lostfilm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/magnetdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/morethantv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/ncore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/newtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/newznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/nnmclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/passthepopcorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/ptn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/rarbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/rlsbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/rmz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/serienjunkies.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/shortened.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/site_1337x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/site_rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/solidtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/torrent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/torrentday.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/torrentz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/wordpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/sites/yts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/urlrewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/urlrewrite_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/urlrewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/sites/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/status/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/status/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/status/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/thetvdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/thetvdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/thetvdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/thetvdb/api_tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/thetvdb/thetvdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/tmdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tmdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tmdb/api_tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tmdb/tmdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/api_trakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/next_trakt_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/trakt_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/trakt_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/trakt/trakt_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/tvmaze/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tvmaze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tvmaze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tvmaze/api_tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/tvmaze/tvmaze_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/components/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/variables/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/components/variables/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/db_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/explain_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/perf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/try_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/wiki_qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/cli/win32_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/pyload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40357 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/clients/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/daemon/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/abort_if_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/accept_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/best_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/content_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/crossmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/exists_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/exists_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/if_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/limit_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/magnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/only_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/proper_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/require_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/thetvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/filter/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/cron_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/db_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/db_vacuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/log_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/generic/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/input/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/anidb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/apple_trailers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/betaseries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/filmweb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/from_piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/from_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/from_telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/input_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/kitsu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/letterboxd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/medusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/my_anime_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/myepisodes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/next_sonarr_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/npo_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/plex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/pogcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/regexp_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/rlslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/rottentomatoes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/sceper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/sickbeard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/torznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/input/twitterfeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/internal/api_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/internal/api_rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/internal/change_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/metainfo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/assume_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/bluray_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/media_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/metainfo_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/nfo_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/nzb_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/rottentomatoes_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/subtitles_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/metainfo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/modify/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/path_by_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/path_by_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/plugin_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/reorder_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/set_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/modify/sort_by_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/operate/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/abort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/cfscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/debug_db_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/debug_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/disable_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/domain_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/entry_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/formlogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/free_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/max_reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/spy_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/verbose_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/verify_ssl_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/operate/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/output/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22421 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/download_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/dump_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/mock_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/rtorrent_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/subtitles_periscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/subtitles_subliminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/output/utorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/services/kodi_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/services/myepisodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/plugins/services/pogcal_acquired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/resources/flexget.png
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/templates/entry/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/templates/entry/default.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/templates/task/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/templates/task/default.template
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/templates/task/html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/templates/task/rss.template
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/app.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/app/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/app/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.eot
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/app/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/scripts/splash.js
--rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/scripts/vendor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/styles/splash.css
--rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-06-21 15:12:28.000000 FlexGet-3.7.8/flexget/ui/v1/app/styles/vendor.css
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/build.js
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/inject.js
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/lint.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/scripts.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/server.js
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/test.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulp/watch.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/load.failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/specs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/app.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/app.loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/app.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/app.scss
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/app.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/assets/images/header.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/_error-dialog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/exception/exception.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/exception/exception.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/pagination.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/pagination.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/router/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/router/router-helper.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/router/router-helper.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/_login.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.config.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/components.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.route.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/_database.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/_sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/components/user/user.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/construction.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/directives/directives.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/directives/palette-background/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/layout.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.route.js
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.scss
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/plugins.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-field/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:35.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.service.js
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/server.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/server.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/server.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/scss/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/scss/_loading-bar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/scss/flexget.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/src/services/schema.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/execute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/history.js
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/movie_list.js
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/registerPlugin.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/schedules.js
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/seen.js
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/series.js
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/states.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
--rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
--rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
--rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
--rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
--rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
--rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
--rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
--rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
--rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
--rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
--rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
--rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-21 15:12:29.000000 FlexGet-3.7.8/flexget/ui/v2/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/ui/v2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/bittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/cached_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/lazy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:12:36.000000 FlexGet-3.7.8/flexget/utils/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/parsers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/parsers/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/parsers/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/simple_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/soup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-21 15:12:19.000000 FlexGet-3.7.8/flexget/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-21 15:12:19.000000 FlexGet-3.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-21 15:12:19.000000 FlexGet-3.7.8/requirements-docker.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-21 15:12:19.000000 FlexGet-3.7.8/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-21 15:12:19.000000 FlexGet-3.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:12:36.000000 FlexGet-3.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 15:14:55.000000 FlexGet-3.7.9/FlexGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-11 15:14:30.000000 FlexGet-3.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 15:14:30.000000 FlexGet-3.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-11 15:14:55.000000 FlexGet-3.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-11 15:14:30.000000 FlexGet-3.7.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-11 15:14:30.000000 FlexGet-3.7.9/dev-requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-11 15:14:30.000000 FlexGet-3.7.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-11 15:14:43.000000 FlexGet-3.7.9/flexget/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/templates/api_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/api/templates/swagger-ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archive/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/backlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/backlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/backlog/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/bittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/convert_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/magnet_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/private_torrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/torrent_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/bittorrent/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/emby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83806 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/api_emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/emby_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/emby/from_emby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/estimate_release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimate_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_movies_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_released_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_series_tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/failed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/failed/retry_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/ftp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/ftp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23176 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/ftp/sftp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/history/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/imdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/from_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/imdb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/imdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/irc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/irc/irc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/list_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/couchpotato_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/entry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/imdb_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/movie_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/pending_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/plex_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/radarr_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/sonarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/subtitle_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/thetvdb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/managed_lists/lists/yaml_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notification_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/cronitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/ifttt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/microsoftteams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/notifymyandroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/ntfysh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/pushsafer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/rapidpush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/sms_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notifiers/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/parser_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/parser_guessit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/parsers/parser_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/parsing/plugin_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/pending_approval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/pending_approval/pending_approval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/rejected/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/rejected/remember_rejected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/scheduler/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/seen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/seen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/seen_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/seen/seen_movies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/all_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47041 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/configure_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57516 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/gen_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/internal_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/metainfo_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/next_series_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/next_series_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53392 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series_premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/series_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/sites/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/allyoulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/alpharatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/animeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/anirena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/archetorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/argenteam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/awesomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/bakabt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/cinemageddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/cpasbien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/deadfrog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/descargas2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/ettv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/eztv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/filelist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/frenchtorrentdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/fuzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/google_cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/hebits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/hliang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/horriblesubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/koreus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/limetorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/lostfilm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/magnetdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/morethantv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/ncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/newtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/nnmclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/passthepopcorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/ptn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rarbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rlsbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rmz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/serienjunkies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/shortened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/site_1337x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/site_rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/solidtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrentday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/torrentz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/wordpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/sites/yts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/urlrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/urlrewrite_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/urlrewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/sites/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/thetvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/api_tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/thetvdb/thetvdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/api_tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tmdb/tmdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/api_trakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/next_trakt_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/trakt_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/trakt_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/trakt/trakt_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/tvmaze/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/api_tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/tvmaze/tvmaze_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/components/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/variables/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/components/variables/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/explain_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/perf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/try_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/wiki_qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/cli/win32_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/pyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40357 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/clients/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/daemon/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/abort_if_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/accept_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/best_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/content_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/crossmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/exists_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/exists_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/if_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/limit_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/magnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/only_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/proper_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/require_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/thetvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/filter/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/cron_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/db_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/db_vacuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/log_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/generic/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/anidb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/apple_trailers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/betaseries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/filmweb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/from_piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/from_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/from_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/input_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/kitsu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/letterboxd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/medusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/my_anime_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/myepisodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/next_sonarr_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/npo_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/plex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/pogcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/regexp_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/rlslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/rottentomatoes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/sceper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/sickbeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/torznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/input/twitterfeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/api_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/api_rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/internal/change_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/metainfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/assume_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/bluray_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/media_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/metainfo_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/nfo_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/nzb_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/rottentomatoes_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/subtitles_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/metainfo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/modify/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/path_by_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/path_by_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/plugin_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/reorder_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/set_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/modify/sort_by_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/abort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/cfscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/debug_db_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/debug_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/disable_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/domain_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/entry_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/formlogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/free_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/max_reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/spy_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/verbose_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/verify_ssl_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/operate/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/download_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/dump_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/mock_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/rtorrent_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/subtitles_periscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/subtitles_subliminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/output/utorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/kodi_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/myepisodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/plugins/services/pogcal_acquired.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/resources/flexget.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/templates/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/entry/default.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/templates/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/task/default.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/task/html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/templates/task/rss.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/app.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/splash.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/scripts/vendor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/splash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-07-11 15:14:44.000000 FlexGet-3.7.9/flexget/ui/v1/app/styles/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/build.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/inject.js
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/lint.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulp/watch.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/load.failure.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/specs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/app.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/assets/images/header.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/_error-dialog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/_login.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/components.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.route.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/_database.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/_sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/components/user/user.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/construction.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/directives.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/palette-background/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/layout.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/plugins.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-field/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/_loading-bar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/scss/flexget.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/src/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/src/services/schema.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/execute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/movie_list.js
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/registerPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/schedules.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/seen.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/series.js
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/states.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
+-rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
+-rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-11 15:14:46.000000 FlexGet-3.7.9/flexget/ui/v2/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/ui/v2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/bittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/cached_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:14:55.000000 FlexGet-3.7.9/flexget/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/parsers/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/simple_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/soup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-11 15:14:30.000000 FlexGet-3.7.9/flexget/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-11 15:14:30.000000 FlexGet-3.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-11 15:14:30.000000 FlexGet-3.7.9/requirements-docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-11 15:14:30.000000 FlexGet-3.7.9/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-11 15:14:30.000000 FlexGet-3.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:14:55.000000 FlexGet-3.7.9/setup.cfg
```

### Comparing `FlexGet-3.7.8/FlexGet.egg-info/PKG-INFO` & `FlexGet-3.7.9/FlexGet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.7.8
+Version: 3.7.9
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.7.8/FlexGet.egg-info/SOURCES.txt` & `FlexGet-3.7.9/FlexGet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/FlexGet.egg-info/requires.txt` & `FlexGet-3.7.9/FlexGet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/LICENSE` & `FlexGet-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/PKG-INFO` & `FlexGet-3.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.7.8
+Version: 3.7.9
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.7.8/README.rst` & `FlexGet-3.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/dev-requirements-extras.txt` & `FlexGet-3.7.9/dev-requirements-extras.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/dev-requirements.txt` & `FlexGet-3.7.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/__init__.py` & `FlexGet-3.7.9/flexget/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/python
 import os
 import sys
-from typing import Sequence
+from typing import Optional, Sequence
 
 # __version__ import need to be first in order to avoid circular import within logger
 from ._version import __version__  # noqa
 
 # isort: split
 from flexget import log
 from flexget.manager import Manager
 
 
-def main(args: Sequence[str] = None):
+def main(args: Optional[Sequence[str]] = None):
     """Main entry point for Command Line Interface"""
 
     if args is None:
         args = sys.argv[1:]
     try:
         log.initialize()
```

### Comparing `FlexGet-3.7.8/flexget/api/app.py` & `FlexGet-3.7.9/flexget/api/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import re
 from collections import deque
 from contextlib import suppress
 from functools import partial, wraps
-from typing import TYPE_CHECKING, Callable, Dict, List, Mapping, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Mapping, Optional, Tuple, Union
 
 from flask import Flask, Request, Response, jsonify, make_response, request
 from flask_compress import Compress
 from flask_cors import CORS
 from flask_restx import Api as RestxAPI
 from flask_restx import Model, Resource
 from flask_restx.reqparse import RequestParser
@@ -53,15 +53,15 @@
 
     def __init__(self) -> None:
         self.app = api_app.test_client()
 
     def __getattr__(self, item: str) -> 'APIEndpoint':
         return APIEndpoint('/api/' + item, self.get_endpoint)
 
-    def get_endpoint(self, url: str, data=None, method: str = None):
+    def get_endpoint(self, url: str, data=None, method: Optional[str] = None):
         if method is None:
             method = 'POST' if data is not None else 'GET'
         auth_header = {'Authorization': 'Token %s' % api_key()}
         response = self.app.open(
             url, data=data, follow_redirects=True, method=method, headers=auth_header
         )
         result = json.loads(response.get_data(as_text=True))
@@ -77,15 +77,15 @@
         self.caller = caller
 
     def __getattr__(self, item):
         return self.__class__(self.endpoint + '/' + item, self.caller)
 
     __getitem__ = __getattr__
 
-    def __call__(self, data=None, method: str = None):
+    def __call__(self, data=None, method: Optional[str] = None):
         return self.caller(self.endpoint, data=data, method=method)
 
 
 def api_version(f: Callable[..., Response]):
     """Add the 'API-Version' header to all responses"""
 
     @wraps(f)
@@ -113,15 +113,15 @@
       - methods to make using json schemas easier
       - methods to auto document and handle :class:`ApiError` responses
     """
 
     def validate(
         self,
         model: Model,
-        schema_override: Dict[str, List[Dict[str, str]]] = None,
+        schema_override: Optional[Dict[str, List[Dict[str, str]]]] = None,
         description=None,
     ):
         """
         When a method is decorated with this, json data submitted to the endpoint will be validated with the given
         `model`. This also auto-documents the expected model, as well as the possible :class:`ValidationError` response.
         """
 
@@ -164,17 +164,17 @@
                     **kwargs,
                 )
         return self.doc(responses={code_or_apierror: (description, model)}, **kwargs)
 
     def pagination_parser(
         self,
         parser: RequestParser = None,
-        sort_choices: List[str] = None,
-        default: str = None,
-        add_sort: bool = None,
+        sort_choices: Optional[List[str]] = None,
+        default: Optional[str] = None,
+        add_sort: Optional[bool] = None,
     ) -> RequestParser:
         """
         Return a standardized pagination parser, to be used for any endpoint that has pagination.
 
         :param RequestParser parser: Can extend a given parser or create a new one
         :param tuple sort_choices: A tuple of strings, to be used as server side attribute searches
         :param str default: The default sort string, used `sort_choices[0]` if not given
@@ -233,15 +233,15 @@
 
 class APIError(Exception):
     description = 'Server error'
     status_code = 500
     status = 'Error'
     response_model = base_message_schema
 
-    def __init__(self, message: str = None, payload=None) -> None:
+    def __init__(self, message: Optional[str] = None, payload=None) -> None:
         self.message = message
         self.payload = payload
 
     def to_dict(self):
         rv = self.payload or {}
         rv.update(status_code=self.status_code, message=self.message, status=self.status)
         return rv
@@ -369,15 +369,15 @@
 
 @with_session
 def api_key(session: Session = None) -> str:
     logger.debug('fetching token for internal lookup')
     return session.query(User).first().token  # type: ignore
 
 
-def etag(method: Callable = None, cache_age: int = 0):
+def etag(method: Optional[Callable] = None, cache_age: int = 0):
     """
     A decorator that add an ETag header to the response and checks for the "If-Match" and "If-Not-Match" headers to
      return an appropriate response.
 
     :param method: A GET or HEAD flask method to wrap
     :param cache_age: max-age cache age for the content
     :return: The method's response with the ETag and Cache-Control headers, raises a 412 error or returns a 304 response
```

### Comparing `FlexGet-3.7.8/flexget/api/core/authentication.py` & `FlexGet-3.7.9/flexget/api/core/authentication.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/cached.py` & `FlexGet-3.7.9/flexget/api/core/cached.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/database.py` & `FlexGet-3.7.9/flexget/api/core/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/format_checker.py` & `FlexGet-3.7.9/flexget/api/core/format_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/plugins.py` & `FlexGet-3.7.9/flexget/api/core/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/schema.py` & `FlexGet-3.7.9/flexget/api/core/schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/server.py` & `FlexGet-3.7.9/flexget/api/core/server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/tasks.py` & `FlexGet-3.7.9/flexget/api/core/tasks.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/core/user.py` & `FlexGet-3.7.9/flexget/api/core/user.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/templates/api_response.html` & `FlexGet-3.7.9/flexget/api/templates/api_response.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/api/templates/swagger-ui.html` & `FlexGet-3.7.9/flexget/api/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/archive/archive.py` & `FlexGet-3.7.9/flexget/components/archive/archive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/archive/cli.py` & `FlexGet-3.7.9/flexget/components/archive/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/archive/db.py` & `FlexGet-3.7.9/flexget/components/archive/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/archives/archives.py` & `FlexGet-3.7.9/flexget/components/archives/archives.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/archives/decompress.py` & `FlexGet-3.7.9/flexget/components/archives/decompress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/archives/utils.py` & `FlexGet-3.7.9/flexget/components/archives/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/backlog/backlog.py` & `FlexGet-3.7.9/flexget/components/backlog/backlog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/backlog/cli.py` & `FlexGet-3.7.9/flexget/components/backlog/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/backlog/db.py` & `FlexGet-3.7.9/flexget/components/backlog/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/convert_magnet.py` & `FlexGet-3.7.9/flexget/components/bittorrent/convert_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/magnet_info_hash.py` & `FlexGet-3.7.9/flexget/components/bittorrent/magnet_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/private_torrents.py` & `FlexGet-3.7.9/flexget/components/bittorrent/private_torrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/torrent.py` & `FlexGet-3.7.9/flexget/components/bittorrent/torrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/torrent_alive.py` & `FlexGet-3.7.9/flexget/components/bittorrent/torrent_alive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/torrent_files.py` & `FlexGet-3.7.9/flexget/components/bittorrent/torrent_files.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/torrent_match.py` & `FlexGet-3.7.9/flexget/components/bittorrent/torrent_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/torrent_scrub.py` & `FlexGet-3.7.9/flexget/components/bittorrent/torrent_scrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/torrent_size.py` & `FlexGet-3.7.9/flexget/components/bittorrent/torrent_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/bittorrent/trackers.py` & `FlexGet-3.7.9/flexget/components/bittorrent/trackers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/emby/api_emby.py` & `FlexGet-3.7.9/flexget/components/emby/api_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/emby/emby_list.py` & `FlexGet-3.7.9/flexget/components/emby/emby_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/emby/emby_lookup.py` & `FlexGet-3.7.9/flexget/components/emby/emby_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/emby/emby_refresh.py` & `FlexGet-3.7.9/flexget/components/emby/emby_refresh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/emby/emby_util.py` & `FlexGet-3.7.9/flexget/components/emby/emby_util.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/emby/from_emby.py` & `FlexGet-3.7.9/flexget/components/emby/from_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/estimate_release/estimate_release.py` & `FlexGet-3.7.9/flexget/components/estimate_release/estimate_release.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/estimate_release/estimators/est_movies_bluray.py` & `FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_movies_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/estimate_release/estimators/est_released_movies.py` & `FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_released_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/estimate_release/estimators/est_series_tvmaze.py` & `FlexGet-3.7.9/flexget/components/estimate_release/estimators/est_series_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/failed/api.py` & `FlexGet-3.7.9/flexget/components/failed/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/failed/cli.py` & `FlexGet-3.7.9/flexget/components/failed/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/failed/db.py` & `FlexGet-3.7.9/flexget/components/failed/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/failed/retry_failed.py` & `FlexGet-3.7.9/flexget/components/failed/retry_failed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/ftp/ftp_download.py` & `FlexGet-3.7.9/flexget/components/ftp/ftp_download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/ftp/ftp_list.py` & `FlexGet-3.7.9/flexget/components/ftp/ftp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/ftp/sftp.py` & `FlexGet-3.7.9/flexget/components/ftp/sftp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/ftp/sftp_client.py` & `FlexGet-3.7.9/flexget/components/ftp/sftp_client.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/history/api.py` & `FlexGet-3.7.9/flexget/components/history/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/history/cli.py` & `FlexGet-3.7.9/flexget/components/history/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/history/db.py` & `FlexGet-3.7.9/flexget/components/history/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/history/history.py` & `FlexGet-3.7.9/flexget/components/history/history.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/api.py` & `FlexGet-3.7.9/flexget/components/imdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/db.py` & `FlexGet-3.7.9/flexget/components/imdb/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/from_imdb.py` & `FlexGet-3.7.9/flexget/components/imdb/from_imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/imdb.py` & `FlexGet-3.7.9/flexget/components/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/imdb_lookup.py` & `FlexGet-3.7.9/flexget/components/imdb/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/imdb_url.py` & `FlexGet-3.7.9/flexget/components/imdb/imdb_url.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/imdb_watchlist.py` & `FlexGet-3.7.9/flexget/components/imdb/imdb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/imdb/utils.py` & `FlexGet-3.7.9/flexget/components/imdb/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/irc/api.py` & `FlexGet-3.7.9/flexget/components/irc/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/irc/cli.py` & `FlexGet-3.7.9/flexget/components/irc/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/irc/irc.py` & `FlexGet-3.7.9/flexget/components/irc/irc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/list_add.py` & `FlexGet-3.7.9/flexget/components/managed_lists/list_add.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/list_clear.py` & `FlexGet-3.7.9/flexget/components/managed_lists/list_clear.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/list_match.py` & `FlexGet-3.7.9/flexget/components/managed_lists/list_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/list_remove.py` & `FlexGet-3.7.9/flexget/components/managed_lists/list_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/couchpotato_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/couchpotato_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/api.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/cli.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/db.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/entry_list/entry_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/entry_list/entry_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/imdb_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/imdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/api.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/cli.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/db.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/movie_list/movie_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/movie_list/movie_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/api.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/cli.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/db.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/pending_list/pending_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/pending_list/pending_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/plex_watchlist.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/plex_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/radarr_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/radarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/cli.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/db.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/regexp_list/regexp_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/regexp_list/regexp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/sonarr_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/sonarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/subtitle_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/subtitle_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/thetvdb_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/thetvdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/managed_lists/lists/yaml_list.py` & `FlexGet-3.7.9/flexget/components/managed_lists/lists/yaml_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notification_framework.py` & `FlexGet-3.7.9/flexget/components/notify/notification_framework.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/bark.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/bark.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/cronitor.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/cronitor.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/discord.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/email.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/gotify.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/gotify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/ifttt.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/ifttt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/join.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/join.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/matrix.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/matrix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/microsoftteams.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/microsoftteams.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/mqtt.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/mqtt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/notifymyandroid.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/notifymyandroid.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/ntfysh.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/ntfysh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/prowl.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/prowl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/pushalot.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/pushalot.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/pushbullet.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/pushbullet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/pushover.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/pushover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/pushsafer.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/pushsafer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/rapidpush.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/rapidpush.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/slack.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/sms_ru.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/sms_ru.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/telegram.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/toast.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/toast.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notifiers/xmpp.py` & `FlexGet-3.7.9/flexget/components/notify/notifiers/xmpp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/notify/notify.py` & `FlexGet-3.7.9/flexget/components/notify/notify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/parsing/parsers/parser_common.py` & `FlexGet-3.7.9/flexget/components/parsing/parsers/parser_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     name = capwords(name)
     return name
 
 
 class MovieParseResult:
     def __init__(
         self,
-        data: str = None,
-        name: str = None,
+        data: Optional[str] = None,
+        name: Optional[str] = None,
         year: Optional[int] = None,
         quality: Quality = None,
         proper_count: int = 0,
         release_group: Optional[str] = None,
         valid: bool = True,
     ) -> None:
         self.name: str = name
@@ -109,19 +109,19 @@
             valid,
         )
 
 
 class SeriesParseResult:
     def __init__(
         self,
-        data: str = None,
-        name: str = None,
-        identified_by: str = None,
-        id_type: str = None,
-        id: Union[Tuple[int, int], str, int, datetime.date] = None,
+        data: Optional[str] = None,
+        name: Optional[str] = None,
+        identified_by: Optional[str] = None,
+        id_type: Optional[str] = None,
+        id: Optional[Union[Tuple[int, int], str, int, datetime.date]] = None,
         episodes: int = 1,
         season_pack: bool = False,
         strict_name: bool = False,
         quality: Quality = None,
         proper_count: int = 0,
         special: bool = False,
         group: Optional[str] = None,
```

### Comparing `FlexGet-3.7.8/flexget/components/parsing/parsers/parser_guessit.py` & `FlexGet-3.7.9/flexget/components/parsing/parsers/parser_guessit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/parsing/parsers/parser_internal.py` & `FlexGet-3.7.9/flexget/components/parsing/parsers/parser_internal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/parsing/plugin_parsing.py` & `FlexGet-3.7.9/flexget/components/parsing/plugin_parsing.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/pending_approval/api.py` & `FlexGet-3.7.9/flexget/components/pending_approval/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/pending_approval/cli.py` & `FlexGet-3.7.9/flexget/components/pending_approval/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/pending_approval/db.py` & `FlexGet-3.7.9/flexget/components/pending_approval/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/pending_approval/pending_approval.py` & `FlexGet-3.7.9/flexget/components/pending_approval/pending_approval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/rejected/api.py` & `FlexGet-3.7.9/flexget/components/rejected/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/rejected/cli.py` & `FlexGet-3.7.9/flexget/components/rejected/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/rejected/db.py` & `FlexGet-3.7.9/flexget/components/rejected/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/rejected/remember_rejected.py` & `FlexGet-3.7.9/flexget/components/rejected/remember_rejected.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/scheduler/api.py` & `FlexGet-3.7.9/flexget/components/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/scheduler/scheduler.py` & `FlexGet-3.7.9/flexget/components/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/seen/api.py` & `FlexGet-3.7.9/flexget/components/seen/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/seen/cli.py` & `FlexGet-3.7.9/flexget/components/seen/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/seen/db.py` & `FlexGet-3.7.9/flexget/components/seen/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/seen/seen.py` & `FlexGet-3.7.9/flexget/components/seen/seen.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/seen/seen_info_hash.py` & `FlexGet-3.7.9/flexget/components/seen/seen_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/seen/seen_movies.py` & `FlexGet-3.7.9/flexget/components/seen/seen_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/all_series.py` & `FlexGet-3.7.9/flexget/components/series/all_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/api.py` & `FlexGet-3.7.9/flexget/components/series/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/cli.py` & `FlexGet-3.7.9/flexget/components/series/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/configure_series.py` & `FlexGet-3.7.9/flexget/components/series/configure_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/db.py` & `FlexGet-3.7.9/flexget/components/series/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -801,16 +801,16 @@
             db_alt_names.append(AlternateNames(alt_name))
             logger.debug('adding alternate name `{}` to series `{}`', alt_name, db_series.name)
     db_series.alternate_names[:] = db_alt_names
 
 
 def show_seasons(
     series: Series,
-    start: int = None,
-    stop: int = None,
+    start: Optional[int] = None,
+    stop: Optional[int] = None,
     count: bool = False,
     descending: bool = False,
     session: Session = None,
 ) -> Union[int, List[Season]]:
     """Return all seasons of a given series"""
     seasons = session.query(Season).filter(Season.series_id == series.id)
     if count:
@@ -837,20 +837,20 @@
             return e.first_seen or datetime.min, e.identifier
 
     return sorted(episodes + seasons, key=key, reverse=reverse)
 
 
 def get_episode_releases(
     episode: Episode,
-    downloaded: bool = None,
-    start: int = None,
-    stop: int = None,
+    downloaded: Optional[bool] = None,
+    start: Optional[int] = None,
+    stop: Optional[int] = None,
     count: bool = False,
     descending: bool = False,
-    sort_by: str = None,
+    sort_by: Optional[str] = None,
     session: Session = None,
 ) -> List[EpisodeRelease]:
     """Return all releases for a given episode"""
     releases = session.query(EpisodeRelease).filter(EpisodeRelease.episode_id == episode.id)
     if downloaded is not None:
         releases = releases.filter(EpisodeRelease.downloaded == downloaded)
     if count:
@@ -861,20 +861,20 @@
     else:
         releases = releases.order_by(getattr(EpisodeRelease, sort_by))
     return releases.slice(start, stop).all()
 
 
 def get_season_releases(
     season: Season,
-    downloaded: bool = None,
-    start: int = None,
-    stop: int = None,
+    downloaded: Optional[bool] = None,
+    start: Optional[int] = None,
+    stop: Optional[int] = None,
     count: bool = False,
     descending: bool = False,
-    sort_by: str = None,
+    sort_by: Optional[str] = None,
     session: Session = None,
 ) -> Union[int, List[SeasonRelease]]:
     """Return all releases for a given season"""
     releases = session.query(SeasonRelease).filter(SeasonRelease.season_id == season.id)
     if downloaded is not None:
         releases = releases.filter(SeasonRelease.downloaded == downloaded)
     if count:
@@ -942,23 +942,23 @@
         db_series_alt = AlternateNames(alt)
         db_series.alternate_names.append(db_series_alt)
         logger.debug('-> added {}', db_series_alt)
 
 
 @with_session
 def get_series_summary(
-    configured: str = None,
-    premieres: bool = None,
-    start: int = None,
-    stop: int = None,
+    configured: Optional[str] = None,
+    premieres: Optional[bool] = None,
+    start: Optional[int] = None,
+    stop: Optional[int] = None,
     count: bool = False,
     sort_by: str = 'show_name',
-    descending: bool = None,
+    descending: Optional[bool] = None,
     session: Session = None,
-    name: str = None,
+    name: Optional[str] = None,
 ) -> Union[int, Iterable[Series]]:
     """
     Return a query with results for all series.
 
     :param configured: 'configured' for shows in config, 'unconfigured' for shows not in config, 'all' for both.
         Default is 'all'
     :param premieres: Return only shows with 1 season and less than 3 episodes
@@ -1044,15 +1044,15 @@
         'Multiple id types may be accepted until it locks in on the appropriate type.',
         series.name,
     )
     return 'auto'
 
 
 def get_latest_season_pack_release(
-    series: Series, downloaded: bool = True, season: int = None
+    series: Series, downloaded: bool = True, season: Optional[int] = None
 ) -> Optional[Season]:
     """
     Return the latest season pack release for a series
 
     :param Series series: Series object
     :param bool downloaded: Flag to return only downloaded season packs
     :param season: Filter by season number
@@ -1087,15 +1087,15 @@
         downloaded,
         season,
     )
     return latest_season_pack_release
 
 
 def get_latest_episode_release(
-    series: Series, downloaded: bool = True, season: int = None
+    series: Series, downloaded: bool = True, season: Optional[int] = None
 ) -> Optional[Episode]:
     """
     :param series series: SQLAlchemy session
     :param downloaded: find only downloaded releases
     :param season: season to find newest release for
     :return: Instance of Episode or None if not found.
     """
@@ -1142,15 +1142,15 @@
         downloaded,
         season,
     )
     return latest_episode_release
 
 
 def get_latest_release(
-    series: Series, downloaded: bool = True, season: int = None
+    series: Series, downloaded: bool = True, season: Optional[int] = None
 ) -> Union[EpisodeRelease, SeasonRelease, None]:
     """
     Return the latest downloaded entity of a series, either season pack or episode
 
     :param Series series: Series object
     :param bool downloaded: Downloaded flag
     :param int season: Filter by season
@@ -1407,16 +1407,16 @@
 def season_release_by_id(release_id: int, session: Session = None) -> SeasonRelease:
     """Return an instance of an episode release by querying its ID"""
     return session.query(SeasonRelease).filter(SeasonRelease.id == release_id).one()
 
 
 def show_episodes(
     series: Series,
-    start: int = None,
-    stop: int = None,
+    start: Optional[int] = None,
+    stop: Optional[int] = None,
     count: bool = False,
     descending: bool = False,
     session: Session = None,
 ) -> Union[int, List[Episode]]:
     """Return all episodes of a given series"""
     episodes = session.query(Episode).filter(Episode.series_id == series.id)
     if count:
```

### Comparing `FlexGet-3.7.8/flexget/components/series/gen_series.py` & `FlexGet-3.7.9/flexget/components/series/gen_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/internal_estimator.py` & `FlexGet-3.7.9/flexget/components/series/internal_estimator.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/metainfo_series.py` & `FlexGet-3.7.9/flexget/components/series/metainfo_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/next_series_episodes.py` & `FlexGet-3.7.9/flexget/components/series/next_series_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/next_series_seasons.py` & `FlexGet-3.7.9/flexget/components/series/next_series_seasons.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/series.py` & `FlexGet-3.7.9/flexget/components/series/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/series_begin.py` & `FlexGet-3.7.9/flexget/components/series/series_begin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/series_premiere.py` & `FlexGet-3.7.9/flexget/components/series/series_premiere.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/series/series_remove.py` & `FlexGet-3.7.9/flexget/components/series/series_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/allyoulike.py` & `FlexGet-3.7.9/flexget/components/sites/sites/allyoulike.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/alpharatio.py` & `FlexGet-3.7.9/flexget/components/sites/sites/alpharatio.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/animeindex.py` & `FlexGet-3.7.9/flexget/components/sites/sites/animeindex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/anirena.py` & `FlexGet-3.7.9/flexget/components/sites/sites/anirena.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/archetorrent.py` & `FlexGet-3.7.9/flexget/components/sites/sites/archetorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/argenteam.py` & `FlexGet-3.7.9/flexget/components/sites/sites/argenteam.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/awesomehd.py` & `FlexGet-3.7.9/flexget/components/sites/sites/awesomehd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/bakabt.py` & `FlexGet-3.7.9/flexget/components/sites/sites/bakabt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/btn.py` & `FlexGet-3.7.9/flexget/components/sites/sites/btn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/cinemageddon.py` & `FlexGet-3.7.9/flexget/components/sites/sites/cinemageddon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/cpasbien.py` & `FlexGet-3.7.9/flexget/components/sites/sites/cpasbien.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/deadfrog.py` & `FlexGet-3.7.9/flexget/components/sites/sites/deadfrog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/descargas2020.py` & `FlexGet-3.7.9/flexget/components/sites/sites/descargas2020.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/ettv.py` & `FlexGet-3.7.9/flexget/components/sites/sites/ettv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/eztv.py` & `FlexGet-3.7.9/flexget/components/sites/sites/eztv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/filelist.py` & `FlexGet-3.7.9/flexget/components/sites/sites/filelist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/filelist_api.py` & `FlexGet-3.7.9/flexget/components/sites/sites/filelist_api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/frenchtorrentdb.py` & `FlexGet-3.7.9/flexget/components/sites/sites/frenchtorrentdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/fuzer.py` & `FlexGet-3.7.9/flexget/components/sites/sites/fuzer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/google_cse.py` & `FlexGet-3.7.9/flexget/components/sites/sites/google_cse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/hebits.py` & `FlexGet-3.7.9/flexget/components/sites/sites/hebits.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/hliang.py` & `FlexGet-3.7.9/flexget/components/sites/sites/hliang.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/horriblesubs.py` & `FlexGet-3.7.9/flexget/components/sites/sites/horriblesubs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/iptorrents.py` & `FlexGet-3.7.9/flexget/components/sites/sites/iptorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/koreus.py` & `FlexGet-3.7.9/flexget/components/sites/sites/koreus.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/limetorrents.py` & `FlexGet-3.7.9/flexget/components/sites/sites/limetorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/lostfilm.py` & `FlexGet-3.7.9/flexget/components/sites/sites/lostfilm.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/magnetdl.py` & `FlexGet-3.7.9/flexget/components/sites/sites/magnetdl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/morethantv.py` & `FlexGet-3.7.9/flexget/components/sites/sites/morethantv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/ncore.py` & `FlexGet-3.7.9/flexget/components/sites/sites/ncore.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/newtorrents.py` & `FlexGet-3.7.9/flexget/components/sites/sites/newtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/newznab.py` & `FlexGet-3.7.9/flexget/components/sites/sites/newznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/nnmclub.py` & `FlexGet-3.7.9/flexget/components/sites/sites/nnmclub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/nyaa.py` & `FlexGet-3.7.9/flexget/components/sites/sites/nyaa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/passthepopcorn.py` & `FlexGet-3.7.9/flexget/components/sites/sites/passthepopcorn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/piratebay.py` & `FlexGet-3.7.9/flexget/components/sites/sites/piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/ptn.py` & `FlexGet-3.7.9/flexget/components/sites/sites/ptn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/rarbg.py` & `FlexGet-3.7.9/flexget/components/sites/sites/rarbg.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/redirect.py` & `FlexGet-3.7.9/flexget/components/sites/sites/redirect.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/rlsbb.py` & `FlexGet-3.7.9/flexget/components/sites/sites/rlsbb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/rmz.py` & `FlexGet-3.7.9/flexget/components/sites/sites/rmz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/rss.py` & `FlexGet-3.7.9/flexget/components/sites/sites/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/rutracker.py` & `FlexGet-3.7.9/flexget/components/sites/sites/rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/serienjunkies.py` & `FlexGet-3.7.9/flexget/components/sites/sites/serienjunkies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/shortened.py` & `FlexGet-3.7.9/flexget/components/sites/sites/shortened.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/site_1337x.py` & `FlexGet-3.7.9/flexget/components/sites/sites/site_1337x.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/site_rutracker.py` & `FlexGet-3.7.9/flexget/components/sites/sites/site_rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/solidtorrents.py` & `FlexGet-3.7.9/flexget/components/sites/sites/solidtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/torrent_cache.py` & `FlexGet-3.7.9/flexget/components/sites/sites/torrent_cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/torrentday.py` & `FlexGet-3.7.9/flexget/components/sites/sites/torrentday.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/torrentleech.py` & `FlexGet-3.7.9/flexget/components/sites/sites/torrentleech.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/torrentz.py` & `FlexGet-3.7.9/flexget/components/sites/sites/torrentz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/wordpress.py` & `FlexGet-3.7.9/flexget/components/sites/sites/wordpress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/sites/yts.py` & `FlexGet-3.7.9/flexget/components/sites/sites/yts.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/urlrewrite.py` & `FlexGet-3.7.9/flexget/components/sites/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/urlrewrite_search.py` & `FlexGet-3.7.9/flexget/components/sites/urlrewrite_search.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/urlrewriting.py` & `FlexGet-3.7.9/flexget/components/sites/urlrewriting.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/sites/utils.py` & `FlexGet-3.7.9/flexget/components/sites/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/status/api.py` & `FlexGet-3.7.9/flexget/components/status/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/status/cli.py` & `FlexGet-3.7.9/flexget/components/status/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/status/db.py` & `FlexGet-3.7.9/flexget/components/status/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/status/status.py` & `FlexGet-3.7.9/flexget/components/status/status.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/thetvdb/api.py` & `FlexGet-3.7.9/flexget/components/thetvdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/thetvdb/api_tvdb.py` & `FlexGet-3.7.9/flexget/components/thetvdb/api_tvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/thetvdb/thetvdb_lookup.py` & `FlexGet-3.7.9/flexget/components/thetvdb/thetvdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/tmdb/api.py` & `FlexGet-3.7.9/flexget/components/tmdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/tmdb/api_tmdb.py` & `FlexGet-3.7.9/flexget/components/tmdb/api_tmdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/tmdb/tmdb_lookup.py` & `FlexGet-3.7.9/flexget/components/tmdb/tmdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/api.py` & `FlexGet-3.7.9/flexget/components/trakt/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/api_trakt.py` & `FlexGet-3.7.9/flexget/components/trakt/api_trakt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/cli.py` & `FlexGet-3.7.9/flexget/components/trakt/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/db.py` & `FlexGet-3.7.9/flexget/components/trakt/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/next_trakt_episodes.py` & `FlexGet-3.7.9/flexget/components/trakt/next_trakt_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/trakt_calendar.py` & `FlexGet-3.7.9/flexget/components/trakt/trakt_calendar.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/trakt_list.py` & `FlexGet-3.7.9/flexget/components/trakt/trakt_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/trakt/trakt_lookup.py` & `FlexGet-3.7.9/flexget/components/trakt/trakt_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/tvmaze/api.py` & `FlexGet-3.7.9/flexget/components/tvmaze/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/tvmaze/api_tvmaze.py` & `FlexGet-3.7.9/flexget/components/tvmaze/api_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/tvmaze/tvmaze_lookup.py` & `FlexGet-3.7.9/flexget/components/tvmaze/tvmaze_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/variables/api.py` & `FlexGet-3.7.9/flexget/components/variables/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/components/variables/variables.py` & `FlexGet-3.7.9/flexget/components/variables/variables.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/config_schema.py` & `FlexGet-3.7.9/flexget/config_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/db_schema.py` & `FlexGet-3.7.9/flexget/db_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         _plugin = plugin
         _version = version
 
     return VersionedBase
 
 
 @sqlalchemy.event.listens_for(Base.metadata, "after_create")
-def after_table_create(target, connection, tables: List[Table] = None, **kw) -> None:
+def after_table_create(target, connection, tables: Optional[List[Table]] = None, **kw) -> None:
     """Sets the schema version to most recent for a plugin when it's tables are freshly created."""
     if tables:
         # TODO: Detect if any database upgrading is needed and acquire the lock only in one place
         with flexget.manager.manager.acquire_lock(event=False):
             tables = [table.name for table in tables]
             for plugin, info in plugin_schemas.items():
                 # Only set the version if all tables for a given plugin are being created
```

### Comparing `FlexGet-3.7.8/flexget/entry.py` & `FlexGet-3.7.9/flexget/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 
         # Make sure constructor does not escape our __setitem__ enforcement
         self.update(*args, **kwargs)
 
     def trace(
         self,
         message: Optional[str],
-        operation: str = None,
-        plugin: str = None,
+        operation: Optional[str] = None,
+        plugin: Optional[str] = None,
     ) -> None:
         """
         Adds trace message to the entry which should contain useful information about why
         plugin did not operate on entry. Accept and Reject messages are added to trace automatically.
 
         :param string message: Message to add into entry trace.
         :param string operation: None, reject, accept or fail
@@ -163,24 +163,24 @@
         Register a function to be called when a :class:`Task` has finished processing this entry.
 
         :param func: The function to call
         :param kwargs: Keyword arguments that should be passed to the registered function
         """
         self.add_hook('complete', func, **kwargs)
 
-    def accept(self, reason: str = None, **kwargs) -> None:
+    def accept(self, reason: Optional[str] = None, **kwargs) -> None:
         if self.rejected:
             logger.debug('tried to accept rejected {!r}', self)
         elif not self.accepted:
             self._state = EntryState.ACCEPTED
             self.trace(reason, operation='accept')
             # Run entry on_accept hooks
             self.run_hooks('accept', reason=reason, **kwargs)
 
-    def reject(self, reason: str = None, **kwargs) -> None:
+    def reject(self, reason: Optional[str] = None, **kwargs) -> None:
         # ignore rejections on immortal entries
         if self.get('immortal'):
             reason_str = '(%s)' % reason if reason else ''
             logger.info('Tried to reject immortal {} {}', self['title'], reason_str)
             self.trace(f'Tried to reject immortal {reason_str}')
             return
         if not self.rejected:
@@ -348,16 +348,16 @@
             result.add_lazy_fields(*lazy_lookup)
         return result
 
     def add_lazy_fields(
         self,
         lazy_func: Union[Callable[['Entry'], None], str],
         fields: Iterable[str],
-        args: Sequence = None,
-        kwargs: Mapping = None,
+        args: Optional[Sequence] = None,
+        kwargs: Optional[Mapping] = None,
     ):
         """
         Add lazy fields to an entry.
         :param lazy_func: should be a funciton previously registered with the `register_lazy_func` decorator,
             or the name it was registered under.
         :param fields: list of fields this function will fill
         :param args: Arguments that will be passed to the lazy lookup function when called.
```

### Comparing `FlexGet-3.7.8/flexget/event.py` & `FlexGet-3.7.9/flexget/event.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ipc.py` & `FlexGet-3.7.9/flexget/ipc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/log.py` & `FlexGet-3.7.9/flexget/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,18 @@
     )
 
     std_logger = logging.getLogger()
     std_logger.addHandler(InterceptHandler())
 
 
 def start(
-    filename: str = None, level: str = 'INFO', to_console: bool = True, to_file: bool = True
+    filename: Optional[str] = None,
+    level: str = 'INFO',
+    to_console: bool = True,
+    to_file: bool = True,
 ) -> None:
     """After initialization, start file logging."""
     global _logging_started, _startup_buffer, _startup_buffer_id
 
     assert _logging_configured
 
     if _logging_started:
```

### Comparing `FlexGet-3.7.8/flexget/manager.py` & `FlexGet-3.7.9/flexget/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,17 +250,17 @@
 
     @property
     def has_lock(self) -> bool:
         return self._has_lock
 
     def execute(
         self,
-        options: Union[dict, argparse.Namespace] = None,
+        options: Optional[Union[dict, argparse.Namespace]] = None,
         priority: int = 1,
-        suppress_warnings: Sequence[str] = None,
+        suppress_warnings: Optional[Sequence[str]] = None,
     ) -> List[Tuple[str, str, threading.Event]]:
         """
         Run all (can be limited with options) tasks from the config.
 
         :param options: Either an :class:`argparse.Namespace` instance, or a dict, containing options for execution
         :param priority: If there are other executions waiting to be run, they will be run in priority order,
             lowest first.
@@ -362,15 +362,15 @@
             self.db_filename = db_test_filename
         # No running process, we start our own to handle command
         with self.acquire_lock():
             self.initialize()
             self.handle_cli()
             self._shutdown()
 
-    def handle_cli(self, options: argparse.Namespace = None) -> None:
+    def handle_cli(self, options: Optional[argparse.Namespace] = None) -> None:
         """
         Dispatch a cli command to the appropriate function.
 
         * :meth:`.execute_command`
         * :meth:`.daemon_command`
         * CLI plugin callback function
 
@@ -613,15 +613,17 @@
             while True:
                 data = f.read(65536)
                 if not data:
                     break
                 sha1_hash.update(data)
         return sha1_hash.hexdigest()
 
-    def load_config(self, output_to_console: bool = True, config_file_hash: str = None) -> None:
+    def load_config(
+        self, output_to_console: bool = True, config_file_hash: Optional[str] = None
+    ) -> None:
         """
         Loads the config file from disk, validates and activates it.
 
         :raises: `ValueError` if there is a problem loading the config file
         """
         fire_event('manager.before_config_load', self)
         with open(self.config_path, encoding='utf-8') as f:
@@ -738,15 +740,15 @@
         """Makes sure that all tasks will have the config_modified flag come out true on the next run.
         Useful when changing the db and all tasks need to be completely reprocessed."""
         from flexget.task import config_changed
 
         config_changed()
         fire_event('manager.config_updated', self)
 
-    def validate_config(self, config: dict = None) -> dict:
+    def validate_config(self, config: Optional[dict] = None) -> dict:
         """
         Check all root level keywords are valid. Config may be modified by before_config_validate hooks. Modified
         config will be returned.
 
         :param config: Config to check. If not provided, current manager config will be checked.
         :raises: `ValueError` when config fails validation. There will be an `errors` attribute with the schema errors.
         :returns: Final validated config.
@@ -894,15 +896,15 @@
                     fire_event('manager.lock_acquired', self)
             yield
         finally:
             if acquired:
                 self.release_lock()
                 self._has_lock = False
 
-    def write_lock(self, ipc_info: dict = None) -> None:
+    def write_lock(self, ipc_info: Optional[dict] = None) -> None:
         assert self._has_lock
         with open(self.lockfile, 'w', encoding='utf-8') as f:
             f.write(f'PID: {os.getpid()}\n')
             if ipc_info:
                 for key in sorted(ipc_info):
                     f.write(f'{key}: {ipc_info[key]}\n')
```

### Comparing `FlexGet-3.7.8/flexget/options.py` & `FlexGet-3.7.9/flexget/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from flexget.utils.tools import get_current_flexget_version, get_latest_flexget_version_number
 
 _UNSET = object()
 
 core_parser: Optional['CoreArgumentParser'] = None
 
 
-def get_parser(command: str = None) -> 'ArgumentParser':
+def get_parser(command: Optional[str] = None) -> 'ArgumentParser':
     global core_parser
     if not core_parser:
         core_parser = CoreArgumentParser()
         # Add all plugin options to the parser
         fire_event('options.register')
     if command:
         return core_parser.get_subparser(command)
@@ -207,15 +207,15 @@
         self.nested_namespaces = kwargs.pop('nested_namespaces', False)
         self.parent_defaults = {}
         # Python < 3.7 doesn't support the 'required' argument for subparsers
         required = kwargs.pop('required', True)
         super().__init__(*args, **kwargs)
         self.required = required
 
-    def add_parser(self, name: str, parent_defaults: dict = None, **kwargs):
+    def add_parser(self, name: str, parent_defaults: Optional[dict] = None, **kwargs):
         if parent_defaults:
             self.parent_defaults[name] = parent_defaults
         return super().add_parser(name, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         parser_name = values[0]
         if parser_name in self.parent_defaults:
@@ -339,18 +339,18 @@
                 action.default = SUPPRESS
 
     def error(self, msg: str):
         raise ParserError(msg, self)
 
     def parse_args(
         self,
-        args: List[str] = None,
-        namespace: Namespace = None,
+        args: Optional[List[str]] = None,
+        namespace: Optional[Namespace] = None,
         raise_errors: bool = False,
-        file: TextIO = None,
+        file: Optional[TextIO] = None,
     ):  # pylint: disable=W0221
         """
         :param raise_errors: If this is true, errors will be raised as `ParserError`s instead of calling sys.exit
         """
         ArgumentParser.file = file
         try:
             return super().parse_args(args, namespace)
@@ -359,17 +359,17 @@
                 raise
             super(ArgumentParser, e.parser).error(e.message)
         finally:
             ArgumentParser.file = None
 
     def parse_known_args(
         self,
-        args: List[str] = None,
-        namespace: Namespace = None,
-        do_help: bool = None,
+        args: Optional[List[str]] = None,
+        namespace: Optional[Namespace] = None,
+        do_help: Optional[bool] = None,
     ):
         if args is None:
             args = sys.argv[1:]
         if namespace is None:
             namespace = ScopedNamespace()
         old_do_help = ArgumentParser.do_help
         if do_help is not None:
```

### Comparing `FlexGet-3.7.8/flexget/plugin.py` & `FlexGet-3.7.9/flexget/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 plugins_loaded = False
 
 _loaded_plugins = {}
 _plugin_options = []
 _new_phase_queue: Dict[str, List[Optional[str]]] = {}
 
 
-def register_task_phase(name: str, before: str = None, after: str = None):
+def register_task_phase(name: str, before: Optional[str] = None, after: Optional[str] = None):
     """Adds a new task phase to the available phases."""
     if before and after:
         raise RegisterException('You can only give either before or after for a phase.')
     if not before and not after:
         raise RegisterException('You must specify either a before or after phase.')
     if name in task_phases or name in _new_phase_queue:
         raise RegisterException(f'Phase {name} already exists.')
```

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/check.py` & `FlexGet-3.7.9/flexget/plugins/cli/check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/cli_config.py` & `FlexGet-3.7.9/flexget/plugins/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/database.py` & `FlexGet-3.7.9/flexget/plugins/cli/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/debug_info.py` & `FlexGet-3.7.9/flexget/plugins/cli/debug_info.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/doc.py` & `FlexGet-3.7.9/flexget/plugins/cli/doc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/explain_sql.py` & `FlexGet-3.7.9/flexget/plugins/cli/explain_sql.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/filters.py` & `FlexGet-3.7.9/flexget/plugins/cli/filters.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/inject.py` & `FlexGet-3.7.9/flexget/plugins/cli/inject.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/perf_tests.py` & `FlexGet-3.7.9/flexget/plugins/cli/perf_tests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/performance.py` & `FlexGet-3.7.9/flexget/plugins/cli/performance.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/plugins.py` & `FlexGet-3.7.9/flexget/plugins/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/templates.py` & `FlexGet-3.7.9/flexget/plugins/cli/templates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/try_regexp.py` & `FlexGet-3.7.9/flexget/plugins/cli/try_regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/web.py` & `FlexGet-3.7.9/flexget/plugins/cli/web.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/wiki_qualities.py` & `FlexGet-3.7.9/flexget/plugins/cli/wiki_qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/cli/win32_service.py` & `FlexGet-3.7.9/flexget/plugins/cli/win32_service.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/aria2.py` & `FlexGet-3.7.9/flexget/plugins/clients/aria2.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/deluge.py` & `FlexGet-3.7.9/flexget/plugins/clients/deluge.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/nzbget.py` & `FlexGet-3.7.9/flexget/plugins/clients/nzbget.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/pyload.py` & `FlexGet-3.7.9/flexget/plugins/clients/pyload.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/qbittorrent.py` & `FlexGet-3.7.9/flexget/plugins/clients/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/rtorrent.py` & `FlexGet-3.7.9/flexget/plugins/clients/rtorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/clients/transmission.py` & `FlexGet-3.7.9/flexget/plugins/clients/transmission.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/daemon/web_server.py` & `FlexGet-3.7.9/flexget/plugins/daemon/web_server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/abort_if_exists.py` & `FlexGet-3.7.9/flexget/plugins/filter/abort_if_exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/accept_all.py` & `FlexGet-3.7.9/flexget/plugins/filter/accept_all.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/age.py` & `FlexGet-3.7.9/flexget/plugins/filter/age.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/best_quality.py` & `FlexGet-3.7.9/flexget/plugins/filter/best_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/content_filter.py` & `FlexGet-3.7.9/flexget/plugins/filter/content_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/content_size.py` & `FlexGet-3.7.9/flexget/plugins/filter/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/crossmatch.py` & `FlexGet-3.7.9/flexget/plugins/filter/crossmatch.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/delay.py` & `FlexGet-3.7.9/flexget/plugins/filter/delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/duplicates.py` & `FlexGet-3.7.9/flexget/plugins/filter/duplicates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/exists.py` & `FlexGet-3.7.9/flexget/plugins/filter/exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/exists_movie.py` & `FlexGet-3.7.9/flexget/plugins/filter/exists_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/exists_series.py` & `FlexGet-3.7.9/flexget/plugins/filter/exists_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/if_condition.py` & `FlexGet-3.7.9/flexget/plugins/filter/if_condition.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/limit_new.py` & `FlexGet-3.7.9/flexget/plugins/filter/limit_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/magnets.py` & `FlexGet-3.7.9/flexget/plugins/filter/magnets.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/only_new.py` & `FlexGet-3.7.9/flexget/plugins/filter/only_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/proper_movies.py` & `FlexGet-3.7.9/flexget/plugins/filter/proper_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/quality.py` & `FlexGet-3.7.9/flexget/plugins/filter/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/regexp.py` & `FlexGet-3.7.9/flexget/plugins/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/require_field.py` & `FlexGet-3.7.9/flexget/plugins/filter/require_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/rottentomatoes.py` & `FlexGet-3.7.9/flexget/plugins/filter/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/thetvdb.py` & `FlexGet-3.7.9/flexget/plugins/filter/thetvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/timeframe.py` & `FlexGet-3.7.9/flexget/plugins/filter/timeframe.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/unique.py` & `FlexGet-3.7.9/flexget/plugins/filter/unique.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/filter/upgrade.py` & `FlexGet-3.7.9/flexget/plugins/filter/upgrade.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/generic/cron_env.py` & `FlexGet-3.7.9/flexget/plugins/generic/cron_env.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/generic/db_vacuum.py` & `FlexGet-3.7.9/flexget/plugins/generic/db_vacuum.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/generic/log_start.py` & `FlexGet-3.7.9/flexget/plugins/generic/log_start.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/generic/urlfix.py` & `FlexGet-3.7.9/flexget/plugins/generic/urlfix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/generic/welcome.py` & `FlexGet-3.7.9/flexget/plugins/generic/welcome.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/anidb_list.py` & `FlexGet-3.7.9/flexget/plugins/input/anidb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/anilist.py` & `FlexGet-3.7.9/flexget/plugins/input/anilist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/apple_trailers.py` & `FlexGet-3.7.9/flexget/plugins/input/apple_trailers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/betaseries_list.py` & `FlexGet-3.7.9/flexget/plugins/input/betaseries_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/discover.py` & `FlexGet-3.7.9/flexget/plugins/input/discover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/filesystem.py` & `FlexGet-3.7.9/flexget/plugins/input/filesystem.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/filmweb_watchlist.py` & `FlexGet-3.7.9/flexget/plugins/input/filmweb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/from_piratebay.py` & `FlexGet-3.7.9/flexget/plugins/input/from_piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/from_task.py` & `FlexGet-3.7.9/flexget/plugins/input/from_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/from_telegram.py` & `FlexGet-3.7.9/flexget/plugins/input/from_telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/gazelle.py` & `FlexGet-3.7.9/flexget/plugins/input/gazelle.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/generate.py` & `FlexGet-3.7.9/flexget/plugins/input/generate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/html.py` & `FlexGet-3.7.9/flexget/plugins/input/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/input_csv.py` & `FlexGet-3.7.9/flexget/plugins/input/input_csv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/inputs.py` & `FlexGet-3.7.9/flexget/plugins/input/inputs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/json.py` & `FlexGet-3.7.9/flexget/plugins/input/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/kitsu.py` & `FlexGet-3.7.9/flexget/plugins/input/kitsu.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/letterboxd.py` & `FlexGet-3.7.9/flexget/plugins/input/letterboxd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/limit.py` & `FlexGet-3.7.9/flexget/plugins/input/limit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/medusa.py` & `FlexGet-3.7.9/flexget/plugins/input/medusa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/mock.py` & `FlexGet-3.7.9/flexget/plugins/input/mock.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/my_anime_list.py` & `FlexGet-3.7.9/flexget/plugins/input/my_anime_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/myepisodes_list.py` & `FlexGet-3.7.9/flexget/plugins/input/myepisodes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/next_sonarr_episodes.py` & `FlexGet-3.7.9/flexget/plugins/input/next_sonarr_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/npo_watchlist.py` & `FlexGet-3.7.9/flexget/plugins/input/npo_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/parameterize.py` & `FlexGet-3.7.9/flexget/plugins/input/parameterize.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/plex.py` & `FlexGet-3.7.9/flexget/plugins/input/plex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/pogcal.py` & `FlexGet-3.7.9/flexget/plugins/input/pogcal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/regexp_parse.py` & `FlexGet-3.7.9/flexget/plugins/input/regexp_parse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/rlslog.py` & `FlexGet-3.7.9/flexget/plugins/input/rlslog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/rottentomatoes_list.py` & `FlexGet-3.7.9/flexget/plugins/input/rottentomatoes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/rss.py` & `FlexGet-3.7.9/flexget/plugins/input/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/sceper.py` & `FlexGet-3.7.9/flexget/plugins/input/sceper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/sickbeard.py` & `FlexGet-3.7.9/flexget/plugins/input/sickbeard.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/tail.py` & `FlexGet-3.7.9/flexget/plugins/input/tail.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/text.py` & `FlexGet-3.7.9/flexget/plugins/input/text.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/torznab.py` & `FlexGet-3.7.9/flexget/plugins/input/torznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/input/twitterfeed.py` & `FlexGet-3.7.9/flexget/plugins/input/twitterfeed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/internal/api_bluray.py` & `FlexGet-3.7.9/flexget/plugins/internal/api_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/internal/api_rottentomatoes.py` & `FlexGet-3.7.9/flexget/plugins/internal/api_rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/internal/change_warn.py` & `FlexGet-3.7.9/flexget/plugins/internal/change_warn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/assume_quality.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/assume_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/bluray_lookup.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/bluray_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/content_size.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/media_id.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/media_id.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/metainfo_movie.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/metainfo_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/nfo_lookup.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/nfo_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/nzb_size.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/nzb_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/quality.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/rottentomatoes_lookup.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/rottentomatoes_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/subtitles_check.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/subtitles_check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/metainfo/task.py` & `FlexGet-3.7.9/flexget/plugins/metainfo/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/extension.py` & `FlexGet-3.7.9/flexget/plugins/modify/extension.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/headers.py` & `FlexGet-3.7.9/flexget/plugins/modify/headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/manipulate.py` & `FlexGet-3.7.9/flexget/plugins/modify/manipulate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/path_by_ext.py` & `FlexGet-3.7.9/flexget/plugins/modify/path_by_ext.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/path_by_space.py` & `FlexGet-3.7.9/flexget/plugins/modify/path_by_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/plugin_priority.py` & `FlexGet-3.7.9/flexget/plugins/modify/plugin_priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/regex_extract.py` & `FlexGet-3.7.9/flexget/plugins/modify/regex_extract.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/reorder_quality.py` & `FlexGet-3.7.9/flexget/plugins/modify/reorder_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/set_field.py` & `FlexGet-3.7.9/flexget/plugins/modify/set_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/sort_by.py` & `FlexGet-3.7.9/flexget/plugins/modify/sort_by.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/modify/sort_by_weight.py` & `FlexGet-3.7.9/flexget/plugins/modify/sort_by_weight.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/cfscraper.py` & `FlexGet-3.7.9/flexget/plugins/operate/cfscraper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/cookies.py` & `FlexGet-3.7.9/flexget/plugins/operate/cookies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/debug_db_sessions.py` & `FlexGet-3.7.9/flexget/plugins/operate/debug_db_sessions.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/debug_warnings.py` & `FlexGet-3.7.9/flexget/plugins/operate/debug_warnings.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/digest.py` & `FlexGet-3.7.9/flexget/plugins/operate/digest.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/disable.py` & `FlexGet-3.7.9/flexget/plugins/operate/disable.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/disable_phases.py` & `FlexGet-3.7.9/flexget/plugins/operate/disable_phases.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/domain_delay.py` & `FlexGet-3.7.9/flexget/plugins/operate/domain_delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/entry_trace.py` & `FlexGet-3.7.9/flexget/plugins/operate/entry_trace.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/formlogin.py` & `FlexGet-3.7.9/flexget/plugins/operate/formlogin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/free_space.py` & `FlexGet-3.7.9/flexget/plugins/operate/free_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/include.py` & `FlexGet-3.7.9/flexget/plugins/operate/include.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/interval.py` & `FlexGet-3.7.9/flexget/plugins/operate/interval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/log_filter.py` & `FlexGet-3.7.9/flexget/plugins/operate/log_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/manual.py` & `FlexGet-3.7.9/flexget/plugins/operate/manual.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/max_reruns.py` & `FlexGet-3.7.9/flexget/plugins/operate/max_reruns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/pathscrub.py` & `FlexGet-3.7.9/flexget/plugins/operate/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/priority.py` & `FlexGet-3.7.9/flexget/plugins/operate/priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/proxy.py` & `FlexGet-3.7.9/flexget/plugins/operate/proxy.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/rerun.py` & `FlexGet-3.7.9/flexget/plugins/operate/rerun.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/run_task.py` & `FlexGet-3.7.9/flexget/plugins/operate/run_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/sequence.py` & `FlexGet-3.7.9/flexget/plugins/operate/sequence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/sleep.py` & `FlexGet-3.7.9/flexget/plugins/operate/sleep.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/spy_headers.py` & `FlexGet-3.7.9/flexget/plugins/operate/spy_headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/template.py` & `FlexGet-3.7.9/flexget/plugins/operate/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/verbose.py` & `FlexGet-3.7.9/flexget/plugins/operate/verbose.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/verbose_details.py` & `FlexGet-3.7.9/flexget/plugins/operate/verbose_details.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/verify_ssl_certificates.py` & `FlexGet-3.7.9/flexget/plugins/operate/verify_ssl_certificates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/operate/version_checker.py` & `FlexGet-3.7.9/flexget/plugins/operate/version_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/download.py` & `FlexGet-3.7.9/flexget/plugins/output/download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/download_auth.py` & `FlexGet-3.7.9/flexget/plugins/output/download_auth.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/dump.py` & `FlexGet-3.7.9/flexget/plugins/output/dump.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/dump_config.py` & `FlexGet-3.7.9/flexget/plugins/output/dump_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/exec.py` & `FlexGet-3.7.9/flexget/plugins/output/exec.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/file_operations.py` & `FlexGet-3.7.9/flexget/plugins/output/file_operations.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/html.py` & `FlexGet-3.7.9/flexget/plugins/output/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/memusage.py` & `FlexGet-3.7.9/flexget/plugins/output/memusage.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/mock_output.py` & `FlexGet-3.7.9/flexget/plugins/output/mock_output.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/rss.py` & `FlexGet-3.7.9/flexget/plugins/output/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/rtorrent_magnet.py` & `FlexGet-3.7.9/flexget/plugins/output/rtorrent_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/sabnzbd.py` & `FlexGet-3.7.9/flexget/plugins/output/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/sns.py` & `FlexGet-3.7.9/flexget/plugins/output/sns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/subtitles.py` & `FlexGet-3.7.9/flexget/plugins/output/subtitles.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/subtitles_periscope.py` & `FlexGet-3.7.9/flexget/plugins/output/subtitles_periscope.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/subtitles_subliminal.py` & `FlexGet-3.7.9/flexget/plugins/output/subtitles_subliminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/symlink.py` & `FlexGet-3.7.9/flexget/plugins/output/symlink.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/output/utorrent.py` & `FlexGet-3.7.9/flexget/plugins/output/utorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/services/kodi_library.py` & `FlexGet-3.7.9/flexget/plugins/services/kodi_library.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/services/myepisodes.py` & `FlexGet-3.7.9/flexget/plugins/services/myepisodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/plugins/services/pogcal_acquired.py` & `FlexGet-3.7.9/flexget/plugins/services/pogcal_acquired.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/resources/flexget.png` & `FlexGet-3.7.9/flexget/resources/flexget.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/task.py` & `FlexGet-3.7.9/flexget/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     hash = Column('hash', String)
 
     def __repr__(self) -> str:
         return f'<TaskConfigHash(task={self.task},hash={self.hash})>'
 
 
 @with_session
-def config_changed(task: str = None, session: ContextSession = None) -> None:
+def config_changed(task: Optional[str] = None, session: ContextSession = None) -> None:
     """
     Forces config_modified flag to come out true on next run of `task`. Used when the db changes, and all
     entries need to be reprocessed.
 
     .. WARNING: DO NOT (FURTHER) USE FROM PLUGINS
 
     :param task: Name of the task. If `None`, will be set for all tasks.
@@ -130,15 +130,15 @@
     def sort(self, *args, **kwargs):
         self.all_entries.sort(*args, **kwargs)
 
 
 class EntryContainer(list):
     """Container for a list of entries, also contains accepted, rejected failed iterators over them."""
 
-    def __init__(self, iterable: list = None):
+    def __init__(self, iterable: Optional[list] = None):
         list.__init__(self, iterable or [])
 
         self._entries = EntryIterator(self, [EntryState.UNDECIDED, EntryState.ACCEPTED])
         self._accepted = EntryIterator(
             self, EntryState.ACCEPTED
         )  # accepted entries, can still be rejected
         self._rejected = EntryIterator(
@@ -405,15 +405,15 @@
         :param string plugin: Name of ``plugin``
         :raises ValueError: *plugin* could not be found.
         """
         if plugin not in all_plugins:
             raise ValueError(f'`{plugin}` is not a valid plugin.')
         self.disabled_plugins.append(plugin)
 
-    def abort(self, reason='Unknown', silent=False, traceback: str = None):
+    def abort(self, reason='Unknown', silent=False, traceback: Optional[str] = None):
         """Abort this task execution, no more plugins will be executed except the abort handling ones."""
         self.aborted = True
         self.abort_reason = reason
         self.silent_abort = silent
         self.traceback = traceback
         if not self.silent_abort:
             logger.warning('Aborting task (plugin: {})', self.current_plugin)
```

### Comparing `FlexGet-3.7.8/flexget/task_queue.py` & `FlexGet-3.7.9/flexget/task_queue.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/templates/task/default.template` & `FlexGet-3.7.9/flexget/templates/task/default.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/templates/task/html.template` & `FlexGet-3.7.9/flexget/templates/task/html.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/templates/task/rss.template` & `FlexGet-3.7.9/flexget/templates/task/rss.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/terminal.py` & `FlexGet-3.7.9/flexget/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         },
         'single': {'box': rich.box.SQUARE},
         'double': {'box': rich.box.DOUBLE},
         'github': {'box': GITHUB_BOX},
         'heavy-head': {'box': rich.box.HEAVY_HEAD},
     }
 
-    def __init__(self, *args, table_type: str = None, **kwargs) -> None:
+    def __init__(self, *args, table_type: Optional[str] = None, **kwargs) -> None:
         self.table_type = table_type
         if table_type:
             kwargs = {**kwargs, **self.TABLE_TYPES[table_type]}
         super().__init__(*args, **kwargs)
 
     def __rich_console__(self, console, options):
         segments = super().__rich_console__(console, options)
```

### Comparing `FlexGet-3.7.8/flexget/tray_icon.py` & `FlexGet-3.7.9/flexget/tray_icon.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,18 +49,18 @@
         self.running: bool = False
 
         self.add_core_menu_items()
 
     @check_if_tray_is_active
     def add_menu_item(
         self,
-        text: str = None,
-        action: Callable = None,
+        text: Optional[str] = None,
+        action: Optional[Callable] = None,
         menu_item: 'MenuItem' = None,
-        index: int = None,
+        index: Optional[int] = None,
         **kwargs,
     ):
         """
         Add a menu item by passing its text and function, or pass a created MenuItem. Force position by sending index
         """
         if not any(v for v in (menu_item, text)):
             raise ValueError("Either 'text' or 'menu_item' are required")
@@ -68,15 +68,15 @@
         menu_item = menu_item or MenuItem(text=text, action=action, **kwargs)
         if index is not None:
             self.menu_items.insert(index, menu_item)
         else:
             self.menu_items.append(menu_item)
 
     @check_if_tray_is_active
-    def add_menu_separator(self, index: int = None):
+    def add_menu_separator(self, index: Optional[int] = None):
         self.add_menu_item(menu_item=Menu.SEPARATOR, index=index)
 
     def add_core_menu_items(self):
         open_web = partial(webbrowser.open)
         self.add_menu_item(text=f'Flexget {__version__}', enabled=False)
         self.add_menu_separator()
         self.add_menu_item(text='Homepage', action=partial(open_web, 'https://flexget.com/'))
```

### Comparing `FlexGet-3.7.8/flexget/ui/v1/__init__.py` & `FlexGet-3.7.9/flexget/ui/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/app.html` & `FlexGet-3.7.9/flexget/ui/v1/app/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/assets/images/header.png` & `FlexGet-3.7.9/flexget/ui/v1/app/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/favicon.ico` & `FlexGet-3.7.9/flexget/ui/v1/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/FontAwesome.otf` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.eot` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.svg` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.eot` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.svg` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.ttf` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/fonts/ui-grid.woff` & `FlexGet-3.7.9/flexget/ui/v1/app/fonts/ui-grid.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/scripts/app.js` & `FlexGet-3.7.9/flexget/ui/v1/app/scripts/app.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/scripts/splash.js` & `FlexGet-3.7.9/flexget/ui/v1/app/scripts/splash.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/scripts/vendor.js` & `FlexGet-3.7.9/flexget/ui/v1/app/scripts/vendor.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/styles/app.css` & `FlexGet-3.7.9/flexget/ui/v1/app/styles/app.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/styles/splash.css` & `FlexGet-3.7.9/flexget/ui/v1/app/styles/splash.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/app/styles/vendor.css` & `FlexGet-3.7.9/flexget/ui/v1/app/styles/vendor.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/bower.json` & `FlexGet-3.7.9/flexget/ui/v1/bower.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/build.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/build.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/inject.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/inject.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/lint.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/lint.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/proxy.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/proxy.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/server.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/server.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/styles.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/styles.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/test.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/test.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/gulp/watch.js` & `FlexGet-3.7.9/flexget/ui/v1/gulp/watch.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/karma.conf.js` & `FlexGet-3.7.9/flexget/ui/v1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/package.json` & `FlexGet-3.7.9/flexget/ui/v1/package.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/specs.html` & `FlexGet-3.7.9/flexget/ui/v1/specs.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/app.html` & `FlexGet-3.7.9/flexget/ui/v1/src/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/app.module.js` & `FlexGet-3.7.9/flexget/ui/v1/src/app.module.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/app.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/app.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/assets/images/header.png` & `FlexGet-3.7.9/flexget/ui/v1/src/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error-dialog.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/error/error.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/error/error.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/exception/exception.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/exception/exception.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/exception/exception.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/_pagination.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/pagination.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/router/router-helper.provider.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/router/router-helper.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/404/404.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/components/404/404.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.config.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.config.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.config.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/auth.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/auth.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/auth/login.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/components/auth/login.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.config.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/core/core.provider.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/core/core.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.config.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/database/database.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/components/database/database.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/home/home.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/components/home/home.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/_sidenav.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/_sidenav.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.semver.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.semver.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.provider.js` & `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/construction.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/construction.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js` & `FlexGet-3.7.9/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/favicon.ico` & `FlexGet-3.7.9/flexget/ui/v1/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/config/config.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/config/config.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.filter.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/execute/execute.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/execute/execute.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/history/history.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/history/history.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/log/log.tmpl.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/log/log.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/pending/pending.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/pending/pending.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/seen/seen.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/seen/seen.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.component.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.route.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.service.spec.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/series/series.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/series/series.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/loading-dialog.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/server.config.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/server/server.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/server/server.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.component.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.route.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/plugins/status/status.tmpl.html` & `FlexGet-3.7.9/flexget/ui/v1/src/plugins/status/status.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/scss/_header.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/scss/flexget.scss` & `FlexGet-3.7.9/flexget/ui/v1/src/scss/flexget.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/src/services/schema.service.js` & `FlexGet-3.7.9/flexget/ui/v1/src/services/schema.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/config.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/execute.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/execute.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/history.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/history.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/movie_list.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/movie_list.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/seen.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/seen.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/series.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/series.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v1/tests-mock-data/states.js` & `FlexGet-3.7.9/flexget/ui/v1/tests-mock-data/states.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/__init__.py` & `FlexGet-3.7.9/flexget/ui/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map` & `FlexGet-3.7.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/ui/v2/dist/index.html` & `FlexGet-3.7.9/flexget/ui/v2/dist/index.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/bittorrent.py` & `FlexGet-3.7.9/flexget/utils/bittorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Torrenting utils, mostly for handling bencoding and torrent files."""
 # Torrent decoding is a short fragment from effbot.org. Site copyright says:
 # Test scripts and other short code fragments can be considered as being in the public domain.
 import binascii
 import re
 from contextlib import suppress
-from typing import Any, Callable, Dict, Generator, Iterator, List, Union
+from typing import Any, Callable, Dict, Generator, Iterator, List, Optional, Union
 
 from loguru import logger
 
 logger = logger.bind(name='torrent')
 
 # Magic indicator used to quickly recognize torrent files
 TORRENT_RE = re.compile(br'^d\d{1,3}:')
@@ -34,15 +34,17 @@
         "info.files.length",
         "info.files.path",
     )
 ]
 
 
 def clean_meta(
-    meta: Dict[str, Any], including_info: bool = False, log_func: Callable[..., None] = None
+    meta: Dict[str, Any],
+    including_info: bool = False,
+    log_func: Optional[Callable[..., None]] = None,
 ):
     """Clean meta dict. Optionally log changes using the given logger.
 
     See also http://packages.python.org/pyrocore/apidocs/pyrocore.util.metafile-pysrc.html#clean_meta
 
     @param log_func: If given, a callable accepting a string message.
     @return: Set of keys removed from C{meta}.
```

### Comparing `FlexGet-3.7.8/flexget/utils/cache.py` & `FlexGet-3.7.9/flexget/utils/cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/cached_input.py` & `FlexGet-3.7.9/flexget/utils/cached_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
       If the key is not given or present in the configuration :name: is expected to be a cache name (ie. url)
 
     .. note:: Configuration assumptions may make this unusable in some (future) inputs
     """
 
     cache = TimedDict(cache_time='5 minutes')
 
-    def __init__(self, name: str, persist: str = None) -> None:
+    def __init__(self, name: str, persist: Optional[str] = None) -> None:
         # Cast name to unicode to prevent sqlalchemy warnings when filtering
         self.name = str(name)
         # Parse persist time
         self.persist: Optional[timedelta] = parse_timedelta(persist) if persist else None
         # Will be set when wrapped function is called
         self.config_hash = None
         self.cache_name = None
@@ -218,15 +218,15 @@
 
 class IterableCache:
     """
     Can cache any iterable (including generators) without immediately evaluating all entries.
     If `finished_hook` is supplied, it will be called the first time the iterable is run to the end.
     """
 
-    def __init__(self, iterable: Iterable, finished_hook: Callable[[List], None] = None):
+    def __init__(self, iterable: Iterable, finished_hook: Optional[Callable[[List], None]] = None):
         self.iterable = iter(iterable)
         self.cache: List = []
         self.finished_hook = finished_hook
 
     def __iter__(self):
         for item in self.cache:
             yield copy.deepcopy(item)
```

### Comparing `FlexGet-3.7.8/flexget/utils/database.py` & `FlexGet-3.7.9/flexget/utils/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/json.py` & `FlexGet-3.7.9/flexget/utils/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/lazy_dict.py` & `FlexGet-3.7.9/flexget/utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/log.py` & `FlexGet-3.7.9/flexget/utils/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/parsers/generic.py` & `FlexGet-3.7.9/flexget/utils/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/parsers/movie.py` & `FlexGet-3.7.9/flexget/utils/parsers/movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/parsers/parser.py` & `FlexGet-3.7.9/flexget/utils/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/parsers/series.py` & `FlexGet-3.7.9/flexget/utils/parsers/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/pathscrub.py` & `FlexGet-3.7.9/flexget/utils/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/qualities.py` & `FlexGet-3.7.9/flexget/utils/qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/requests.py` & `FlexGet-3.7.9/flexget/utils/requests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/serialization.py` & `FlexGet-3.7.9/flexget/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/simple_persistence.py` & `FlexGet-3.7.9/flexget/utils/simple_persistence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/sqlalchemy_utils.py` & `FlexGet-3.7.9/flexget/utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/utils/template.py` & `FlexGet-3.7.9/flexget/utils/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 def filter_pathdir(val: Optional[str]) -> str:
     """Directory containing the given path."""
     return os.path.dirname(val or '')
 
 
-def filter_pathscrub(val: str, os_mode: str = None) -> str:
+def filter_pathscrub(val: str, os_mode: Optional[str] = None) -> str:
     """Replace problematic characters in a path."""
     if not isinstance(val, str):
         return val
     return pathscrub(val, os_mode)
 
 
 def filter_re_replace(val: AnyStr, pattern: str, repl: str) -> str:
@@ -111,15 +111,15 @@
     if 4 <= day <= 20 or 24 <= day <= 30:
         suffix = "th"
     else:
         suffix = ["st", "nd", "rd"][day % 10 - 1]
     return date_str + suffix
 
 
-def filter_format_number(val, places: int = None, grouping: bool = True) -> str:
+def filter_format_number(val, places: Optional[int] = None, grouping: bool = True) -> str:
     """Formats a number according to the user's locale."""
     if not isinstance(val, (int, float)):
         return val
     if places is not None:
         format_str = f'%.{places}f'
     elif isinstance(val, int):
         format_str = '%d'
@@ -277,15 +277,15 @@
         if name.startswith('filter_'):
             environment.filters[name.split('_', 1)[1]] = filt
     for name, test in list(globals().items()):
         if name.startswith('is_'):
             environment.tests[name.split('_', 1)[1]] = test
 
 
-def list_templates(extensions: List[str] = None) -> List[str]:
+def list_templates(extensions: Optional[List[str]] = None) -> List[str]:
     """Returns all templates names that are configured under environment loader dirs"""
     if environment is None or not hasattr(environment, 'loader'):
         return []
     return environment.list_templates(extensions=extensions)
 
 
 def get_filters() -> dict:
```

### Comparing `FlexGet-3.7.8/flexget/utils/tools.py` & `FlexGet-3.7.9/flexget/utils/tools.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/flexget/webserver.py` & `FlexGet-3.7.9/flexget/webserver.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/pyproject.toml` & `FlexGet-3.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 select = ["C4", "E", "F", "I", "ISC", "PLE", "RUF", "UP"]
 
 ignore = [
     "E501",  # We leave line length up to black
     "E711", "E712",  # Comparisons to True/False/None are valid for sqlalchemy
     "PLE1205",  # Thinks we are using stdlib logging rather than loguru
     "RUF001",  # Some of these ambiguous unicode are in tests on purpose
+    "RUF012", # Maybe can re-enable after https://github.com/astral-sh/ruff/issues/5243
 ]
 
 [tool.ruff.isort]
 known-first-party = ['flexget']
 
 [tool.mypy]
 plugins = ["sqlmypy"]
```

### Comparing `FlexGet-3.7.8/requirements-docker.txt` & `FlexGet-3.7.9/requirements-docker.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/requirements-release.txt` & `FlexGet-3.7.9/requirements-release.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.8/requirements.txt` & `FlexGet-3.7.9/requirements.txt`

 * *Files identical despite different names*

