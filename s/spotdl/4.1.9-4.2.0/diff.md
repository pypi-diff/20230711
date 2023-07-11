# Comparing `tmp/spotdl-4.1.9.tar.gz` & `tmp/spotdl-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl-4.1.9.tar", max compression
+gzip compressed data, was "spotdl-4.2.0.tar", max compression
```

## Comparing `spotdl-4.1.9.tar` & `spotdl-4.2.0.tar`

### file list

```diff
@@ -1,56 +1,59 @@
--rw-r--r--   0        0        0     1074 2023-05-01 11:50:54.916794 spotdl-4.1.9/LICENSE
--rw-r--r--   0        0        0     5977 2023-05-01 11:50:54.916794 spotdl-4.1.9/README.md
--rw-r--r--   0        0        0     2745 2023-05-01 11:50:54.920794 spotdl-4.1.9/pyproject.toml
--rw-r--r--   0        0        0     4668 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/__init__.py
--rw-r--r--   0        0        0      209 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/__main__.py
--rw-r--r--   0        0        0       58 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/_version.py
--rw-r--r--   0        0        0      186 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/__init__.py
--rw-r--r--   0        0        0      598 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/download.py
--rw-r--r--   0        0        0     4120 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/entry_point.py
--rw-r--r--   0        0        0     5995 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/meta.py
--rw-r--r--   0        0        0     2759 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/save.py
--rw-r--r--   0        0        0     5067 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/sync.py
--rw-r--r--   0        0        0     1702 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/url.py
--rw-r--r--   0        0        0     3041 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/web.py
--rw-r--r--   0        0        0       80 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/download/__init__.py
--rw-r--r--   0        0        0    27263 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/download/downloader.py
--rw-r--r--   0        0        0    13137 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/download/progress_handler.py
--rw-r--r--   0        0        0       54 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/__init__.py
--rw-r--r--   0        0        0      465 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/__init__.py
--rw-r--r--   0        0        0    11137 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/base.py
--rw-r--r--   0        0        0     2665 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/sliderkz.py
--rw-r--r--   0        0        0     1840 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/youtube.py
--rw-r--r--   0        0        0     2789 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      382 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3304 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3529 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/base.py
--rw-r--r--   0        0        0     3091 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/genius.py
--rw-r--r--   0        0        0     2765 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     1689 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/__init__.py
--rw-r--r--   0        0        0     3451 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/album.py
--rw-r--r--   0        0        0     3101 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/artist.py
--rw-r--r--   0        0        0     3871 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/options.py
--rw-r--r--   0        0        0     4199 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/playlist.py
--rw-r--r--   0        0        0     2186 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/result.py
--rw-r--r--   0        0        0     3230 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/saved.py
--rw-r--r--   0        0        0     9758 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/song.py
--rw-r--r--   0        0        0      103 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/utils/__init__.py
--rw-r--r--   0        0        0     1001 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/utils/archive.py
--rw-r--r--   0        0        0    19690 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/arguments.py
--rw-r--r--   0        0        0     6994 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/config.py
--rw-r--r--   0        0        0     3109 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/console.py
--rw-r--r--   0        0        0      571 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/downloader.py
--rw-r--r--   0        0        0    11688 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/ffmpeg.py
--rw-r--r--   0        0        0    14271 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/formatter.py
--rw-r--r--   0        0        0     7018 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/github.py
--rw-r--r--   0        0        0     5364 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/logging.py
--rw-r--r--   0        0        0      940 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/lrc.py
--rw-r--r--   0        0        0     4144 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/m3u.py
--rw-r--r--   0        0        0    23312 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/matching.py
--rw-r--r--   0        0        0    15621 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/metadata.py
--rw-r--r--   0        0        0    15570 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/search.py
--rw-r--r--   0        0        0     6870 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/spotify.py
--rw-r--r--   0        0        0    28221 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/static.py
--rw-r--r--   0        0        0    15281 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/web.py
--rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 spotdl-4.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-11 12:45:08.422942 spotdl-4.2.0/LICENSE
+-rw-r--r--   0        0        0     6045 2023-07-11 12:45:08.422942 spotdl-4.2.0/README.md
+-rw-r--r--   0        0        0     2986 2023-07-11 12:45:08.426942 spotdl-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4667 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/__init__.py
+-rw-r--r--   0        0        0      209 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/__main__.py
+-rw-r--r--   0        0        0       58 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/_version.py
+-rw-r--r--   0        0        0      186 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/__init__.py
+-rw-r--r--   0        0        0      598 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/download.py
+-rw-r--r--   0        0        0     4120 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/entry_point.py
+-rw-r--r--   0        0        0     5995 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/meta.py
+-rw-r--r--   0        0        0     2759 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/save.py
+-rw-r--r--   0        0        0     5102 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/sync.py
+-rw-r--r--   0        0        0     1702 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/url.py
+-rw-r--r--   0        0        0     3041 2023-07-11 12:45:08.426942 spotdl-4.2.0/spotdl/console/web.py
+-rw-r--r--   0        0        0       80 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/download/__init__.py
+-rw-r--r--   0        0        0    29131 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/download/downloader.py
+-rw-r--r--   0        0        0    13137 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/__init__.py
+-rw-r--r--   0        0        0      669 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/__init__.py
+-rw-r--r--   0        0        0     4239 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/bandcamp.py
+-rw-r--r--   0        0        0    11988 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/base.py
+-rw-r--r--   0        0        0     5166 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/piped.py
+-rw-r--r--   0        0        0     2665 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     2832 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/soundcloud.py
+-rw-r--r--   0        0        0     1840 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2789 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      382 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3304 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3529 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3091 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     2765 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     1689 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/__init__.py
+-rw-r--r--   0        0        0     3451 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/album.py
+-rw-r--r--   0        0        0     3101 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/artist.py
+-rw-r--r--   0        0        0     4019 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/options.py
+-rw-r--r--   0        0        0     4199 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/playlist.py
+-rw-r--r--   0        0        0     2186 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/result.py
+-rw-r--r--   0        0        0     3230 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/saved.py
+-rw-r--r--   0        0        0     9848 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/types/song.py
+-rw-r--r--   0        0        0      103 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/archive.py
+-rw-r--r--   0        0        0    20402 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/arguments.py
+-rw-r--r--   0        0        0     7586 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/config.py
+-rw-r--r--   0        0        0     3109 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/console.py
+-rw-r--r--   0        0        0      571 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/downloader.py
+-rw-r--r--   0        0        0    11726 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/ffmpeg.py
+-rw-r--r--   0        0        0    17842 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/formatter.py
+-rw-r--r--   0        0        0     7018 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/github.py
+-rw-r--r--   0        0        0     5494 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/logging.py
+-rw-r--r--   0        0        0      940 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/lrc.py
+-rw-r--r--   0        0        0     4183 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/m3u.py
+-rw-r--r--   0        0        0    22510 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/matching.py
+-rw-r--r--   0        0        0    19177 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/metadata.py
+-rw-r--r--   0        0        0    17301 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/search.py
+-rw-r--r--   0        0        0     6870 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/static.py
+-rw-r--r--   0        0        0    15249 2023-07-11 12:45:08.430942 spotdl-4.2.0/spotdl/utils/web.py
+-rw-r--r--   0        0        0     8168 1970-01-01 00:00:00.000000 spotdl-4.2.0/PKG-INFO
```

### Comparing `spotdl-4.1.9/LICENSE` & `spotdl-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/README.md` & `spotdl-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 ## Installation
 
 Refer to our [Installation Guide](https://spotdl.rtfd.io/en/latest/installation/) for more details.
 
 ### Python (Recommended Method)
   - _spotDL_ can be installed by running `pip install spotdl`.
+  - To update spotDL run `pip install --upgrade spotdl`
+
   > On some systems you might have to change `pip` to `pip3`.
 
 <details>
     <summary style="font-size:1.25em"><strong>Other options</strong></summary>
 
 - Prebuilt executable
   - You can download the latest version from the
@@ -60,15 +62,15 @@
     ```
 
  - Build from source
 	```bash
 	git clone https://github.com/spotDL/spotify-downloader && cd spotify-downloader
 	pip install poetry
 	poetry install
-	python3 scripts/build.py
+	poetry run python3 scripts/build.py
 	```
 	An executable is created in `spotify-downloader/dist/`.
 
 </details>
 
 
 ### Installing FFmpeg
@@ -111,15 +113,15 @@
     - Usage:
         `spotdl save [query] --save-file {filename}.spotdl`
 
 - `web`: Starts a web interface instead of using the command line. However, it has limited features and only supports downloading single songs.
 
 - `url`: Get direct download link for each song from the query.
     - Usage:
-        `spotdl web [query]`
+        `spotdl url [query]`
 
 - `sync`: Updates directories. Compares the directory with the current state of the playlist. Newly added songs will be downloaded and removed songs will be deleted. No other songs will be downloaded and no other files will be deleted.
 
     - Usage:
         `spotdl sync [query] --save-file {filename}.spotdl`
 
         This create a new **sync** file, to update the directory in the future, use:
```

### Comparing `spotdl-4.1.9/pyproject.toml` & `spotdl-4.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl"
-version = "4.1.9"
+version = "4.2.0"
 description = "Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/spotDL/spotify-downloader.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
@@ -29,62 +29,71 @@
 python = ">=3.7.2,<3.12"
 
 spotipy = "^2.23.0"
 ytmusicapi = [
     {version = "^0.22.0", python = "<3.8"},
     {version = "^0.24.0", python = ">=3.8"},
 ]
-pytube = "^12.1.3"
-yt-dlp = "^2023.3.4"
+pytube = "^15.0.0"
+yt-dlp = "^2023.7.6"
 mutagen = "^1.46.0"
-rich = "^13.3.5"
+rich = "^13.4.2"
 beautifulsoup4 = "^4.12.2"
-requests = "^2.29.0"
+requests = "^2.31.0"
 rapidfuzz = "==2.15.1"
 python-slugify = {extras = ["unidecode"], version = "^8.0.1"}
 uvicorn = "^0.22.0"
-pydantic = "^1.10.7"
-fastapi = "^0.95.1"
-platformdirs = "^3.5.0"
+pydantic = "^2.0.2"
+fastapi = "^0.100.0"
+platformdirs = "^3.8.1"
 pykakasi = "^2.2.1"
 syncedlyrics = "^0.5.0"
-typing-extensions = "^4.5.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.3.1"
-pytest-mock = "^3.10.0"
+typing-extensions = "^4.7.1"
+soundcloud-v2 = "^1.3.1"
+bandcamp-api = "^0.1.15"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+pytest-mock = "^3.11.1"
 pytest-vcr = "^1.0.2"
-pyfakefs = "^5.2.2"
-pytest-cov = "^4.0.0"
+pyfakefs = "^5.2.3"
+pytest-cov = "^4.1.0"
 pytest-subprocess = "^1.5.0"
 pytest-asyncio = "^0.21.0"
-mypy = "^1.2.0"
-pylint = "^2.17.3"
-black = "^23.3.0"
+mypy = "^1.4.1"
+pylint = "^2.17.4"
+black = [
+    {version = "^23.3.0", python = "<3.8"},
+    {version = "^23.7.0", python = ">=3.8"},
+]
 mdformat-gfm = "^0.3.5"
 types-orjson = "^3.6.2"
 types-python-slugify = "^8.0.0.2"
-types-requests = "^2.29.0.0"
-types-setuptools = "^67.7.0.0"
+types-requests = "^2.31.0.1"
+types-setuptools = "^68.0.0.1"
 types-toml = "^0.10.8.6"
-types-ujson = "^5.7.0.4"
-pyinstaller = "^5.10.1"
-mkdocs = "^1.4.2"
+types-ujson = "^5.8.0.0"
+pyinstaller = "^5.13.0"
+mkdocs = "^1.4.3"
 isort = [
     {version = "^5.11.4", python = "<3.8"},
     {version = "^5.12.0", python = ">=3.8"},
 ]
 dill = "^0.3.6"
-mkdocs-material = "^9.1.8"
-mkdocstrings = "^0.21.2"
-mkdocstrings-python = "^0.9.0"
-pymdown-extensions = "^9.11"
+mkdocs-material = "^9.1.18"
+mkdocstrings = "^0.22.0"
+mkdocstrings-python = "^1.1.2"
+pymdown-extensions = "^10.0.1"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
+vcrpy = [
+    {version = "^4.3.1", python = "<3.8"},
+    {version = "^5.0.0", python = ">=3.8"},
+]
 
 [tool.poetry.scripts]
 spotdl = "spotdl:console_entry_point"
 
 [tool.isort]
 profile = "black"
```

### Comparing `spotdl-4.1.9/spotdl/__init__.py` & `spotdl-4.2.0/spotdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     spotdl = Spotdl(client_id='your-client-id', client_secret='your-client-secret')
 
     songs = spotdl.search(['joji - test drive',
         'https://open.spotify.com/track/4cOdK2wGLETKBW3PvgPWqT'])
 
     results = spotdl.download_songs(songs)
-    song, path = spotdl. download(songs[0])
+    song, path = spotdl.download(songs[0])
     ```
     """
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
```

### Comparing `spotdl-4.1.9/spotdl/console/download.py` & `spotdl-4.2.0/spotdl/console/download.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/console/entry_point.py` & `spotdl-4.2.0/spotdl/console/entry_point.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/console/meta.py` & `spotdl-4.2.0/spotdl/console/meta.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/console/save.py` & `spotdl-4.2.0/spotdl/console/save.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/console/sync.py` & `spotdl-4.2.0/spotdl/console/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     # If the query is a single file, download it
     if len(query) == 1 and query[0].endswith(".spotdl") and not save_path:
         # Load the sync file
         with open(query[0], "r", encoding="utf-8") as sync_file:
             sync_data = json.load(sync_file)
 
         # Verify the sync file
-        if sync_data.get("type") != "sync":
+        if not isinstance(sync_data, dict) or sync_data.get("type") != "sync":
             raise ValueError("Sync file is not a valid sync file.")
 
         # Parse the query
         songs_playlist = parse_query(sync_data["query"], downloader.settings["threads"])
 
         # Get the names and URLs of previously downloaded songs from the sync file
         old_files = []
```

### Comparing `spotdl-4.1.9/spotdl/console/url.py` & `spotdl-4.2.0/spotdl/console/url.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/console/web.py` & `spotdl-4.2.0/spotdl/console/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/download/downloader.py` & `spotdl-4.2.0/spotdl/download/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,33 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from yt_dlp.postprocessor.modify_chapters import ModifyChaptersPP
 from yt_dlp.postprocessor.sponsorblock import SponsorBlockPP
 
 from spotdl.download.progress_handler import ProgressHandler
-from spotdl.providers.audio import AudioProvider, YouTube, YouTubeMusic
-from spotdl.providers.audio.sliderkz import SliderKZ
+from spotdl.providers.audio import (
+    AudioProvider,
+    BandCamp,
+    Piped,
+    SliderKZ,
+    SoundCloud,
+    YouTube,
+    YouTubeMusic,
+)
 from spotdl.providers.lyrics import AzLyrics, Genius, LyricsProvider, MusixMatch, Synced
 from spotdl.types.options import DownloaderOptionalOptions, DownloaderOptions
 from spotdl.types.song import Song
 from spotdl.utils.archive import Archive
 from spotdl.utils.config import (
     DOWNLOADER_OPTIONS,
     create_settings_type,
     get_errors_path,
     get_temp_path,
+    modernize_settings,
 )
 from spotdl.utils.ffmpeg import FFmpegError, convert, get_ffmpeg_path
 from spotdl.utils.formatter import create_file_name
 from spotdl.utils.lrc import generate_lrc
 from spotdl.utils.m3u import gen_m3u_files
 from spotdl.utils.metadata import MetadataError, embed_metadata
 from spotdl.utils.search import gather_known_songs, reinit_song, songs_from_albums
@@ -44,14 +52,17 @@
     "SPONSOR_BLOCK_CATEGORIES",
 ]
 
 AUDIO_PROVIDERS: Dict[str, Type[AudioProvider]] = {
     "youtube": YouTube,
     "youtube-music": YouTubeMusic,
     "slider-kz": SliderKZ,
+    "soundcloud": SoundCloud,
+    "bandcamp": BandCamp,
+    "piped": Piped,
 }
 
 LYRICS_PROVIDERS: Dict[str, Type[LyricsProvider]] = {
     "genius": Genius,
     "musixmatch": MusixMatch,
     "azlyrics": AzLyrics,
     "synced": Synced,
@@ -108,14 +119,16 @@
         # from spotdl.types.options.DOWNLOADER_OPTIONS
         self.settings: DownloaderOptions = DownloaderOptions(
             **create_settings_type(
                 Namespace(config=False), dict(settings), DOWNLOADER_OPTIONS
             )  # type: ignore
         )
 
+        # Handle deprecated values in config file
+        modernize_settings(self.settings)
         logger.debug("Downloader settings: %s", self.settings)
 
         # If no audio providers specified, raise an error
         if len(self.settings["audio_providers"]) == 0:
             raise DownloaderError(
                 "No audio providers specified. Please specify at least one."
             )
@@ -143,21 +156,29 @@
 
         # semaphore is required to limit concurrent asyncio executions
         self.semaphore = asyncio.Semaphore(self.settings["threads"])
 
         self.progress_handler = ProgressHandler(self.settings["simple_tui"])
 
         # Gather already present songs
+        self.scan_formats = self.settings["detect_formats"] or [self.settings["format"]]
         self.known_songs: Dict[str, List[Path]] = {}
         if self.settings["scan_for_songs"]:
             logger.info("Scanning for known songs, this might take a while...")
+            for scan_format in self.scan_formats:
+                logger.debug("Scanning for %s files", scan_format)
 
-            self.known_songs = gather_known_songs(
-                self.settings["output"], self.settings["format"]
-            )
+                found_files = gather_known_songs(self.settings["output"], scan_format)
+
+                for song_url, song_paths in found_files.items():
+                    known_paths = self.known_songs.get(song_url)
+                    if known_paths is None:
+                        self.known_songs[song_url] = song_paths
+                    else:
+                        self.known_songs[song_url].extend(song_paths)
 
         logger.debug("Found %s known songs", len(self.known_songs))
 
         # Initialize lyrics providers
         self.lyrics_providers: List[LyricsProvider] = []
         for lyrics_provider in self.settings["lyrics_providers"]:
             lyrics_class = LYRICS_PROVIDERS.get(lyrics_provider)
@@ -175,14 +196,15 @@
 
             self.audio_providers.append(
                 audio_class(
                     output_format=self.settings["format"],
                     cookie_file=self.settings["cookie_file"],
                     search_query=self.settings["search_query"],
                     filter_results=self.settings["filter_results"],
+                    yt_dlp_args=self.settings["yt_dlp_args"],
                 )
             )
 
         # Initialize list of errors
         self.errors: List[str] = []
 
         # Initialize archive
@@ -425,14 +447,20 @@
                 dup_song_path
                 for dup_song_path in dup_song_paths
                 if (dup_song_path.absolute() != output_file.absolute())
                 and dup_song_path.exists()
             ]
 
             file_exists = output_file.exists() or dup_song_paths
+            if not self.settings["scan_for_songs"]:
+                for file_extension in self.scan_formats:
+                    ext_path = output_file.with_suffix(f".{file_extension}")
+                    if ext_path.exists():
+                        dup_song_paths.append(ext_path)
+
             if dup_song_paths:
                 logger.debug(
                     "Found duplicate songs for %s at %s",
                     song.display_name,
                     dup_song_paths,
                 )
 
@@ -557,29 +585,39 @@
             output_file.parent.mkdir(parents=True, exist_ok=True)
             if song.download_url is None:
                 download_url = self.search(song)
             else:
                 download_url = song.download_url
 
             # Initialize audio downloader
-            audio_downloader = AudioProvider(
-                output_format=self.settings["format"],
-                cookie_file=self.settings["cookie_file"],
-                search_query=self.settings["search_query"],
-                filter_results=self.settings["filter_results"],
-            )
+            audio_downloader: Union[AudioProvider, Piped]
+            if self.settings["audio_providers"][0] == "piped":
+                audio_downloader = Piped(
+                    output_format=self.settings["format"],
+                    cookie_file=self.settings["cookie_file"],
+                    search_query=self.settings["search_query"],
+                    filter_results=self.settings["filter_results"],
+                    yt_dlp_args=self.settings["yt_dlp_args"],
+                )
+            else:
+                audio_downloader = AudioProvider(
+                    output_format=self.settings["format"],
+                    cookie_file=self.settings["cookie_file"],
+                    search_query=self.settings["search_query"],
+                    filter_results=self.settings["filter_results"],
+                    yt_dlp_args=self.settings["yt_dlp_args"],
+                )
 
             logger.debug("Downloading %s using %s", song.display_name, download_url)
 
             # Add progress hook to the audio provider
             audio_downloader.audio_handler.add_progress_hook(
                 display_progress_tracker.yt_dlp_progress_hook
             )
 
-            # Download the song using yt-dlp
             download_info = audio_downloader.get_download_metadata(
                 download_url, download=True
             )
 
             temp_file = Path(
                 temp_folder / f"{download_info['id']}.{download_info['ext']}"
             )
@@ -596,19 +634,24 @@
                 )
 
             display_progress_tracker.notify_download_complete()
 
             # Copy the downloaded file to the output file
             # if the temp file and output file have the same extension
             # and the bitrate is set to auto or disable
+            # Don't copy if the audio provider is piped
+            # unless the bitrate is set to disable
             if (
                 self.settings["bitrate"] in ["auto", "disable", None]
                 and temp_file.suffix == output_file.suffix
+            ) and not (
+                self.settings["audio_providers"][0] == "piped"
+                and self.settings["bitrate"] != "disable"
             ):
-                shutil.move(temp_file, output_file)
+                shutil.move(str(temp_file), output_file)
                 success = True
                 result = None
             else:
                 if self.settings["bitrate"] in ["auto", None]:
                     # Use the bitrate from the download info if it exists
                     # otherwise use `copy`
                     bitrate = (
```

### Comparing `spotdl-4.1.9/spotdl/download/progress_handler.py` & `spotdl-4.2.0/spotdl/download/progress_handler.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/audio/base.py` & `spotdl-4.2.0/spotdl/providers/audio/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 Base audio provider module.
 """
 
 import logging
 import re
+import shlex
 from typing import Any, Dict, List, Optional, Tuple
 
 from yt_dlp import YoutubeDL
 
 from spotdl.types.result import Result
 from spotdl.types.song import Song
 from spotdl.utils.config import get_temp_path
-from spotdl.utils.formatter import create_search_query, create_song_title
+from spotdl.utils.formatter import (
+    args_to_ytdlp_options,
+    create_search_query,
+    create_song_title,
+)
 from spotdl.utils.matching import get_best_matches, order_results
 
 __all__ = ["AudioProviderError", "AudioProvider", "ISRC_REGEX", "YTDLLogger"]
 
 logger = logging.getLogger(__name__)
 
 
@@ -66,14 +71,15 @@
 
     def __init__(
         self,
         output_format: str = "mp3",
         cookie_file: Optional[str] = None,
         search_query: Optional[str] = None,
         filter_results: bool = True,
+        yt_dlp_args: Optional[str] = None,
     ) -> None:
         """
         Base class for audio providers.
 
         ### Arguments
         - output_directory: The directory to save the downloaded songs to.
         - output_format: The format to save the downloaded songs in.
@@ -90,26 +96,30 @@
         if self.output_format == "m4a":
             ytdl_format = "bestaudio[ext=m4a]/bestaudio/best"
         elif self.output_format == "opus":
             ytdl_format = "bestaudio[ext=webm]/bestaudio/best"
         else:
             ytdl_format = "bestaudio"
 
-        self.audio_handler = YoutubeDL(
-            {
-                "format": ytdl_format,
-                "quiet": True,
-                "no_warnings": True,
-                "encoding": "UTF-8",
-                "logger": YTDLLogger(),
-                "cookiefile": self.cookie_file,
-                "outtmpl": f"{get_temp_path()}/%(id)s.%(ext)s",
-                "retries": 5,
-            }
-        )
+        yt_dlp_options = {
+            "format": ytdl_format,
+            "quiet": True,
+            "no_warnings": True,
+            "encoding": "UTF-8",
+            "logger": YTDLLogger(),
+            "cookiefile": self.cookie_file,
+            "outtmpl": f"{get_temp_path()}/%(id)s.%(ext)s",
+            "retries": 5,
+        }
+
+        if yt_dlp_args:
+            user_options = args_to_ytdlp_options(shlex.split(yt_dlp_args))
+            yt_dlp_options.update(user_options)
+
+        self.audio_handler = YoutubeDL(yt_dlp_options)
 
     def get_results(self, search_term: str, **kwargs) -> List[Result]:
         """
         Get results from audio provider.
 
         ### Arguments
         - search_term: The search term to use.
@@ -156,17 +166,15 @@
 
         logger.debug("[%s] Searching for %s", song.song_id, search_query)
 
         isrc_urls: List[str] = []
 
         # search for song using isrc if it's available
         if song.isrc and self.SUPPORTS_ISRC and not self.search_query:
-            isrc_results = self.get_results(
-                song.isrc, filter="songs", ignore_spelling=True
-            )
+            isrc_results = self.get_results(song.isrc, **self.GET_RESULTS_OPTS[0])
 
             if only_verified:
                 isrc_results = [result for result in isrc_results if result.verified]
 
             isrc_urls = [result.url for result in isrc_results]
             sorted_isrc_results = order_results(isrc_results, song, self.search_query)
             logger.debug(
@@ -318,17 +326,31 @@
             views = []
             for best_result in best_results:
                 if best_result[0].views:
                     views.append(best_result[0].views)
                 else:
                     views.append(self.get_views(best_result[0].url))
 
-            best_result = best_results[views.index(max(views))]
+            highest_views = max(views)
+            lowest_views = min(views)
 
-            return best_result[0], best_result[1]
+            if highest_views in (0, lowest_views):
+                return best_result[0], best_result[1]
+
+            weighted_results: List[Tuple[Result, float]] = []
+            for index, best_result in enumerate(best_results):
+                result_views = views[index]
+                views_score = (
+                    (result_views - lowest_views) / (highest_views - lowest_views)
+                ) * 15
+                score = min(best_result[1] + views_score, 100)
+                weighted_results.append((best_result[0], score))
+
+            # Now we return the result with the highest score
+            return max(weighted_results, key=lambda x: x[1])
 
         return best_result[0], best_result[1]
 
     def get_download_metadata(self, url: str, download: bool = False) -> Dict:
         """
         Get metadata for a download using yt-dlp.
 
@@ -341,14 +363,15 @@
 
         try:
             data = self.audio_handler.extract_info(url, download=download)
 
             if data:
                 return data
         except Exception as exception:
+            logger.debug(exception)
             raise AudioProviderError(f"YT-DLP download error - {url}") from exception
 
         raise AudioProviderError(f"No metadata found for the provided url {url}")
 
     @property
     def name(self) -> str:
         """
```

### Comparing `spotdl-4.1.9/spotdl/providers/audio/sliderkz.py` & `spotdl-4.2.0/spotdl/providers/audio/sliderkz.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/audio/youtube.py` & `spotdl-4.2.0/spotdl/providers/audio/youtube.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/audio/ytmusic.py` & `spotdl-4.2.0/spotdl/providers/audio/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/lyrics/azlyrics.py` & `spotdl-4.2.0/spotdl/providers/lyrics/azlyrics.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/lyrics/base.py` & `spotdl-4.2.0/spotdl/providers/lyrics/base.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/lyrics/genius.py` & `spotdl-4.2.0/spotdl/providers/lyrics/genius.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/lyrics/musixmatch.py` & `spotdl-4.2.0/spotdl/providers/lyrics/musixmatch.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/providers/lyrics/synced.py` & `spotdl-4.2.0/spotdl/providers/lyrics/synced.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/types/album.py` & `spotdl-4.2.0/spotdl/types/album.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/types/artist.py` & `spotdl-4.2.0/spotdl/types/artist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/types/options.py` & `spotdl-4.2.0/spotdl/types/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     bitrate: Optional[Union[str, int]]
     ffmpeg_args: Optional[str]
     format: str
     save_file: Optional[str]
     filter_results: bool
     threads: int
     cookie_file: Optional[str]
-    restrict: bool
+    restrict: Optional[str]
     print_errors: bool
     sponsor_block: bool
     preload: bool
     archive: Optional[str]
     load_config: bool
     log_level: str
     simple_tui: bool
@@ -70,14 +70,16 @@
     ytm_data: bool
     add_unavailable: bool
     generate_lrc: bool
     force_update_metadata: bool
     only_verified_results: bool
     sync_without_deleting: bool
     max_filename_length: Optional[int]
+    yt_dlp_args: Optional[str]
+    detect_formats: Optional[str]
 
 
 class WebOptions(TypedDict):
     """
     Options used for initializing the Web server.
     """
 
@@ -128,15 +130,15 @@
     bitrate: Optional[Union[str, int]]
     ffmpeg_args: Optional[str]
     format: str
     save_file: Optional[str]
     filter_results: bool
     threads: int
     cookie_file: Optional[str]
-    restrict: bool
+    restrict: Optional[str]
     print_errors: bool
     sponsor_block: bool
     preload: bool
     archive: Optional[str]
     load_config: bool
     log_level: str
     simple_tui: bool
@@ -145,14 +147,16 @@
     ytm_data: bool
     add_unavailable: bool
     generate_lrc: bool
     force_update_metadata: bool
     only_verified_results: bool
     sync_without_deleting: bool
     max_filename_length: Optional[int]
+    yt_dlp_args: Optional[str]
+    detect_formats: Optional[str]
 
 
 class WebOptionalOptions(TypedDict, total=False):
     """
     Options used for initializing the Web server.
     """
```

### Comparing `spotdl-4.1.9/spotdl/types/playlist.py` & `spotdl-4.2.0/spotdl/types/playlist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/types/result.py` & `spotdl-4.2.0/spotdl/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/types/saved.py` & `spotdl-4.2.0/spotdl/types/saved.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/types/song.py` & `spotdl-4.2.0/spotdl/types/song.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     publisher: str
     url: str
     isrc: Optional[str]
     cover_url: Optional[str]
     copyright_text: Optional[str]
     download_url: Optional[str] = None
     lyrics: Optional[str] = None
+    popularity: Optional[int] = None
     album_id: Optional[str] = None
     list_name: Optional[str] = None
     list_url: Optional[str] = None
     list_position: Optional[int] = None
     list_length: Optional[int] = None
 
     @classmethod
@@ -114,14 +115,15 @@
             track_number=raw_track_meta["track_number"],
             tracks_count=raw_album_meta["total_tracks"],
             isrc=raw_track_meta.get("external_ids", {}).get("isrc"),
             song_id=raw_track_meta["id"],
             explicit=raw_track_meta["explicit"],
             publisher=raw_album_meta["label"],
             url=raw_track_meta["external_urls"]["spotify"],
+            popularity=raw_track_meta["popularity"],
             cover_url=max(
                 raw_album_meta["images"], key=lambda i: i["width"] * i["height"]
             )["url"]
             if raw_album_meta["images"]
             else None,
         )
```

### Comparing `spotdl-4.1.9/spotdl/utils/archive.py` & `spotdl-4.2.0/spotdl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/arguments.py` & `spotdl-4.2.0/spotdl/utils/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,20 @@
 
     # Add query argument
     query = parser.add_argument(
         "query",
         nargs="+",
         type=str,
         help=(
-            "N|Spotify/YouTube URL for a song/playlist/album/artist/etc. to download.\n"
-            "For album searching, include 'album:' and optional 'artist:' tags\n"
-            "(ie. 'album:the album name' or 'artist:the artist album: the album').\n"
+            "N|Spotify/YouTube URL for a song/playlist/album/artist/etc. to download.\n\n"
+            "For album/playlist/artist searching, include 'album:', 'playlist:', 'artist:' \n"
+            "(ie. 'album:the album name' you can mix these options to get more accurate results)"
+            ".\n\n"
+            "To download liked songs use 'saved' as the query, or to download all user playlists\n"
+            "use 'all-user-playlists'.\n\n"
             "For manual audio matching, you can use the format 'YouTubeURL|SpotifyURL'\n"
             "You can only use album/playlist/tracks urls when "
             "downloading/matching youtube urls.\n"
             "When using youtube url without spotify url, "
             "you won't be able to use `--fetch-albums` option.\n\n"
         ),
     )
@@ -381,20 +384,22 @@
             "(When combined with --scan-for-songs force will remove "
             "all duplicates, and metadata will only apply metadata to the "
             "latest song and will remove the rest. )"
         ),
         type=str,
     )
 
-    # Option to restrict filenames for easier handling in the shell
+    # Option to increase compatibility of filenames and easier handling in the shell
     parser.add_argument(
         "--restrict",
-        action="store_const",
-        const=True,
-        help="Restrict filenames to ASCII only",
+        choices={"strict", "ascii", "none"},
+        const="strict",
+        nargs="?",
+        help="Restrict filenames to a sanitized set of characters for better compatibility",
+        type=str,
     )
 
     # Option to print errors on exit, useful for long playlist
     parser.add_argument(
         "--print-errors",
         action="store_const",
         const=True,
@@ -505,14 +510,30 @@
         type=int,
         help=(
             "Max file name length. "
             "(This won't override the max file name length enforced by the OS)"
         ),
     )
 
+    # YT-DlP options
+    parser.add_argument(
+        "--yt-dlp-args",
+        type=str,
+        help="Arguments to pass to yt-dlp",
+    )
+
+    # Detect formats option
+    parser.add_argument(
+        "--detect-formats",
+        type=str,
+        nargs="*",
+        help="Detect already downloaded songs with file format different from the --format option",
+        choices=FFMPEG_FORMATS.keys(),
+    )
+
 
 def parse_web_options(parser: _ArgumentGroup):
     """
     Parse web options from the command line.
 
     ### Arguments
     - parser: The argument parser to add the options to.
```

### Comparing `spotdl-4.1.9/spotdl/utils/config.py` & `spotdl-4.2.0/spotdl/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Module related to managing reading and writing to the config file.
 
 Default config - spotdl.utils.config.DEFAULT_CONFIG
 """
 
 import json
+import logging
 import os
 import platform
 from argparse import Namespace
 from pathlib import Path
 from typing import Any, Dict, Tuple, Union
 
 import platformdirs
@@ -32,14 +33,16 @@
     "create_settings",
     "SPOTIFY_OPTIONS",
     "DOWNLOADER_OPTIONS",
     "WEB_OPTIONS",
     "DEFAULT_CONFIG",
 ]
 
+logger = logging.getLogger(__name__)
+
 
 class ConfigError(Exception):
     """
     Base class for all exceptions related to config.
     """
 
 
@@ -226,14 +229,29 @@
         **create_settings_type(arguments, config, DOWNLOADER_OPTIONS)  # type: ignore
     )
     web_options = WebOptions(**create_settings_type(arguments, config, WEB_OPTIONS))  # type: ignore
 
     return spotify_options, downloader_options, web_options
 
 
+def modernize_settings(options: DownloaderOptions):
+    """Handle deprecated values in config file.
+
+    ### Arguments
+    - options: DownloaderOptions to modernize
+    """
+
+    warning_msg = "Deprecated '%s' value found for '%s' setting in config file. Using '%s' instead."
+
+    # Respect backward compatibility with old boolean --restrict flag
+    if options["restrict"] is True:
+        logger.warning(warning_msg, True, "restrict", "strict")
+        options["restrict"] = "strict"
+
+
 SPOTIFY_OPTIONS: SpotifyOptions = {
     "client_id": "5f573c9620494bae87890c0f08a60293",
     "client_secret": "212476d9b0f3472eaa762d90b19b0ba8",
     "auth_token": None,
     "user_auth": False,
     "headless": False,
     "cache_path": str(get_cache_path()),
@@ -255,15 +273,15 @@
     "bitrate": None,
     "ffmpeg_args": None,
     "format": "mp3",
     "save_file": None,
     "filter_results": True,
     "threads": 4,
     "cookie_file": None,
-    "restrict": False,
+    "restrict": None,
     "print_errors": False,
     "sponsor_block": False,
     "preload": False,
     "archive": None,
     "load_config": True,
     "log_level": "INFO",
     "simple_tui": False,
@@ -272,14 +290,16 @@
     "ytm_data": False,
     "add_unavailable": False,
     "generate_lrc": False,
     "force_update_metadata": False,
     "only_verified_results": False,
     "sync_without_deleting": False,
     "max_filename_length": None,
+    "yt_dlp_args": None,
+    "detect_formats": None,
 }
 
 WEB_OPTIONS: WebOptions = {
     "web_use_output_dir": False,
     "port": 8800,
     "host": "localhost",
     "keep_alive": False,
```

### Comparing `spotdl-4.1.9/spotdl/utils/console.py` & `spotdl-4.2.0/spotdl/utils/console.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/downloader.py` & `spotdl-4.2.0/spotdl/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/ffmpeg.py` & `spotdl-4.2.0/spotdl/utils/ffmpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 FFMPEG_FORMATS = {
     "mp3": ["-codec:a", "libmp3lame"],
     "flac": ["-codec:a", "flac", "-sample_fmt", "s16"],
     "ogg": ["-codec:a", "libvorbis"],
     "opus": ["-codec:a", "libopus"],
     "m4a": ["-codec:a", "aac"],
+    "wav": ["-codec:a", "pcm_s16le"],
 }
 
 DUR_REGEX = re.compile(
     r"Duration: (?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
 )
 TIME_REGEX = re.compile(
     r"out_time=(?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
```

### Comparing `spotdl-4.1.9/spotdl/utils/formatter.py` & `spotdl-4.2.0/spotdl/utils/formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 """
 
 import copy
 import logging
 import re
 from functools import lru_cache
 from pathlib import Path
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
+from unicodedata import normalize
 
 import pykakasi
 from rapidfuzz import fuzz
 from slugify import slugify as py_slugify
+from yt_dlp.options import create_parser
 from yt_dlp.utils import sanitize_filename
 
 from spotdl.types.song import Song
 
 __all__ = [
     "VARS",
     "JAP_REGEX",
@@ -28,14 +30,17 @@
     "format_query",
     "create_search_query",
     "create_file_name",
     "parse_duration",
     "to_ms",
     "restrict_filename",
     "ratio",
+    "smart_split",
+    "create_path_object",
+    "args_to_ytdlp_options",
 ]
 
 VARS = [
     "{title}",
     "{artists}",
     "{artist}",
     "{album}",
@@ -60,14 +65,15 @@
 KKS = pykakasi.kakasi()
 
 JAP_REGEX = re.compile(
     "[\u3000-\u303f\u3040-\u309f\u30a0-\u30ff\uff00-\uff9f\u4e00-\u9faf\u3400-\u4dbf]"
 )
 
 DISALLOWED_REGEX = re.compile(r"[^-a-zA-Z0-9\!\@\$]+")
+YT_DLP_PARSER = create_parser()
 
 logger = logging.getLogger(__name__)
 
 
 def create_song_title(song_name: str, song_artists: List[str]) -> str:
     """
     Create the song title.
@@ -281,26 +287,26 @@
     return format_query(song, template, santitize, file_extension, short=short)
 
 
 def create_file_name(
     song: Song,
     template: str,
     file_extension: str,
-    restrict: bool = False,
+    restrict: Optional[str] = None,
     short: bool = False,
     file_name_length: Optional[int] = None,
 ) -> Path:
     """
     Create the file name for the song, by replacing template variables with the actual values.
 
     ### Arguments
     - song: the song object
     - template: the template string
     - file_extension: the file extension to use
-    - restrict: whether to sanitize the filename
+    - restrict: sanitization to apply to the filename
     - short: whether to use the short version of the template
     - file_name_length: the maximum length of the file name
 
     ### Returns
     - the formatted string as a Path object
     """
 
@@ -327,101 +333,103 @@
         song=song,
         template=template,
         santitize=True,
         file_extension=file_extension,
         short=short,
     )
 
-    # Parse template as Path object
-    file = Path(formatted_string)
-
-    santitized_parts = []
-    for part in file.parts:
-        match = re.search(r"[^\.*](.*)[^\.*$]", part)
-        if match and part != ".spotdl":
-            santitized_parts.append(match.group(0))
-        else:
-            santitized_parts.append(part)
-
-    # Join the parts of the path
-    file = Path(*santitized_parts)
+    file = create_path_object(formatted_string)
 
     length_limit = file_name_length or 255
 
     # Check if the file name length is greater than the limit
     if len(file.name) < length_limit:
         # Restrict the filename if needed
-        if restrict:
-            return restrict_filename(file)
+        if restrict and restrict != "none":
+            return restrict_filename(file, restrict == "strict")
 
         return file
 
     if short is False:
         return create_file_name(
             song,
             template,
             file_extension,
             restrict=restrict,
             short=True,
             file_name_length=length_limit,
         )
 
+    non_template_chars = re.findall(r"(?<!{)[^{}]+(?![^{}]*})", template)
+    half_length = int((length_limit * 0.50) - (len("".join(non_template_chars)) / 2))
+
     # Path template is already short, but we still can't create a file
     # so we reduce it even further
-    long_artist = len(song.artist) > (length_limit * 0.50)
-    long_title = len(song.name) > (length_limit * 0.50)
+    is_long_artist = len(temp_song.artist) > half_length
+    is_long_title = len(temp_song.name) > half_length
 
     path_separator = "/" if "/" in template else "\\"
-    name_template = template.rsplit(path_separator, 1)[1]
+    name_template_parts = template.rsplit(path_separator, 1)
+    name_template = (
+        name_template_parts[1]
+        if len(name_template_parts) > 1
+        else name_template_parts[0]
+    )
 
-    if long_artist:
+    if is_long_artist:
         logger.warning(
-            "%s: File name is too long. Using only part of song artist.",
+            "%s: Song artist is too long. Using only part of song artist.",
             temp_song.display_name,
         )
 
-        short_artist = temp_song.artist.split(",")[0]
-        temp_song.artist = short_artist
-        if len(temp_song.artist) > (length_limit * 0.50):
-            temp_song.artist = temp_song.artist.split(" ")[0]
+        temp_song.artist = smart_split(temp_song.artist, half_length, None)
+        temp_song.artists = [temp_song.artist]
 
-    if long_title:
+    if is_long_title:
         logger.warning(
             "%s: File name is too long. Using only part of the song title.",
             temp_song.display_name,
         )
 
-        name_parts = temp_song.name.split(" ")
+        temp_song.name = smart_split(temp_song.name, half_length, None)
+
+    new_file = create_path_object(
+        format_query(
+            song=temp_song,
+            template=name_template,
+            santitize=True,
+            file_extension=file_extension,
+            short=short,
+        )
+    )
+
+    if len(new_file.name) > length_limit:
+        logger.warning(
+            "File name is still too long. "
+            "Using default file name with shortened artist and title."
+        )
 
-        old_name = temp_song.name
-        temp_song.name = ""
-        for part in name_parts:
-            old_name = temp_song.name
-            temp_song.name += part + " "
-
-            formatted_name = format_query(
-                song=temp_song,
-                template=name_template,
-                santitize=True,
-                file_extension=file_extension,
-                short=True,
+        if template == "{artist} - {title}.{output-ext}":
+            raise ValueError(
+                "File name is still too long, "
+                "but the template is already short. "
+                "Please try other template, "
+                "increase the file name length limit."
             )
 
-            if len(formatted_name.strip()) > length_limit:
-                temp_song.name = old_name.strip()
-                break
+        return create_file_name(
+            temp_song,
+            "{artist} - {title}.{output-ext}",
+            file_extension,
+            restrict=restrict,
+            short=True,
+            file_name_length=length_limit,
+        )
 
-    return create_file_name(
-        song=temp_song,
-        template=template,
-        file_extension=file_extension,
-        restrict=restrict,
-        short=short,
-        file_name_length=length_limit,
-    )
+    return new_file
 
 
 def parse_duration(duration: Optional[str]) -> float:
     """
     Convert string value of time (duration: "25:36:59") to a float value of seconds (92219.0)
 
     ### Arguments
@@ -483,30 +491,35 @@
 
     if precision and isinstance(precision, int):
         return round(result, precision)
 
     return result
 
 
-def restrict_filename(pathobj: Path) -> Path:
+def restrict_filename(pathobj: Path, strict: bool = True) -> Path:
     """
     Sanitizes the filename part of a Path object. Returns modified object.
 
     ### Arguments
     - pathobj: the Path object to sanitize
+    - strict: whether sanitization should be strict
 
     ### Returns
     - the modified Path object
 
     ### Notes
     - Based on the `sanitize_filename` function from yt-dlp
     """
-
-    result = sanitize_filename(pathobj.name, True, False)
-    result = result.replace("_-_", "-")
+    if strict:
+        result = sanitize_filename(pathobj.name, True, False)
+        result = result.replace("_-_", "-")
+    else:
+        result = (
+            normalize("NFKD", pathobj.name).encode("ascii", "ignore").decode("utf-8")
+        )
 
     if not result:
         result = "_"
 
     return pathobj.with_name(result)
 
 
@@ -521,7 +534,111 @@
     - string2: the second string
 
     ### Returns
     - the ratio
     """
 
     return fuzz.ratio(string1, string2)
+
+
+def smart_split(
+    string: str, max_length: int, separators: Optional[List[str]] = None
+) -> str:
+    """
+    Split a string into a list of strings
+    with a maximum length of max_length.
+    Stops at the first separator that produces a string
+    with a length less than max_length.
+
+    ### Arguments
+    - string: the string to split
+    - max_length: the maximum length of string
+    - separators: the separators to split the string with
+
+    ### Returns
+    - the new string
+    """
+
+    if separators is None:
+        separators = ["-", ",", " ", ""]
+
+    for separator in separators:
+        parts = string.split(separator if separator != "" else None)
+        new_string = separator.join(parts[:1])
+        for part in parts[1:]:
+            if len(new_string) + len(separator) + len(part) > max_length:
+                break
+            new_string += separator + part
+
+        if len(new_string) <= max_length:
+            return new_string
+
+    return string[:max_length]
+
+
+def create_path_object(string: str) -> Path:
+    """
+    Create a Path object from a string.
+    Sanitizes the filename part of the Path object.
+
+    ### Arguments
+    - string: the string to convert
+
+    ### Returns
+    - the Path object
+    """
+
+    # Parse template as Path object
+    file = Path(string)
+
+    santitized_parts = []
+    for part in file.parts:
+        match = re.search(r"[^\.*](.*)[^\.*$]", part)
+        if match and part != ".spotdl":
+            santitized_parts.append(match.group(0))
+        else:
+            santitized_parts.append(part)
+
+    # Join the parts of the path
+    return Path(*santitized_parts)
+
+
+def args_to_ytdlp_options(argument_list: List[str]) -> Dict[str, Any]:
+    """
+    Convert a list of arguments to a dictionary of options.
+
+    ### Arguments
+    - argument_list: the list of arguments
+
+    ### Returns
+    - the dictionary of options
+    """
+
+    options_dict: Dict[str, Any] = {}
+    for option_group in YT_DLP_PARSER.option_groups:
+        for option in option_group.option_list:
+            for opts in option._long_opts:  # pylint: disable=protected-access
+                try:
+                    index = argument_list.index(opts)
+                except ValueError:
+                    continue
+
+                if option.action == "store_true":
+                    options_dict[option.dest] = True
+                    continue
+
+                if option.action == "store_false":
+                    options_dict[option.dest] = False
+                    continue
+
+                if option.action == "store":
+                    values = []
+                    val_index = index
+                    while val_index + 1 < len(argument_list) and not argument_list[
+                        val_index + 1
+                    ].startswith("--"):
+                        values.append(argument_list[val_index + 1])
+                        val_index += 1
+
+                    options_dict[option.dest] = values
+
+    return options_dict
```

### Comparing `spotdl-4.1.9/spotdl/utils/github.py` & `spotdl-4.2.0/spotdl/utils/github.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/logging.py` & `spotdl-4.2.0/spotdl/utils/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,14 +172,16 @@
 
     # Don't log too much
     logging.getLogger("requests").setLevel(logging.WARNING)
     logging.getLogger("urllib3").setLevel(logging.WARNING)
     logging.getLogger("spotipy").setLevel(logging.WARNING)
     logging.getLogger("asyncio").setLevel(logging.WARNING)
     logging.getLogger("syncedlyrics").setLevel(logging.WARNING)
+    logging.getLogger("bandcamp_api").setLevel(logging.WARNING)
+    logging.getLogger("beautifulsoup4").setLevel(logging.WARNING)
 
     # Create console
     console = get_console()
     console.push_theme(THEME)
 
     # Add matching level loggers
     logging.addLevelName(MATCH, "MATCH")
```

### Comparing `spotdl-4.1.9/spotdl/utils/lrc.py` & `spotdl-4.2.0/spotdl/utils/lrc.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/m3u.py` & `spotdl-4.2.0/spotdl/utils/m3u.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 ]
 
 
 def create_m3u_content(
     song_list: List[Song],
     template: str,
     file_extension: str,
-    restrict: bool = False,
+    restrict: Optional[str] = None,
     short: bool = False,
 ) -> str:
     """
     Create m3u content and return it as a string.
 
     ### Arguments
     - song_list: the list of songs
     - template: the template to use
     - file_extension: the file extension to use
-    - restrict: whether to sanitize the filename
+    - restrict: sanitization to apply to the filename
     - short: whether to use the short version of the template
 
     ### Returns
     - the m3u content as a string
     """
 
     text = ""
@@ -46,27 +46,27 @@
 
 
 def gen_m3u_files(
     songs: List[Song],
     file_name: Optional[str],
     template: str,
     file_extension: str,
-    restrict: bool = False,
+    restrict: Optional[str] = None,
     short: bool = False,
 ):
     """
     Create an m3u8 filename from the query.
 
     ### Arguments
     - query: the query
     - file_name: the file name to use
     - song_list: the list of songs
     - template: the output file template to use
     - file_extension: the file extension to use
-    - restrict: whether to sanitize the filename
+    - restrict: sanitization to apply to the filename
     - short: whether to use the short version of the template
     """
 
     # If no file name is provided, use the first list's name
     if not file_name:
         file_name = "{list[0]}.m3u8"
 
@@ -129,26 +129,26 @@
 
 
 def create_m3u_file(
     file_name: str,
     song_list: List[Song],
     template: str,
     file_extension: str,
-    restrict: bool = False,
+    restrict: Optional[str] = None,
     short: bool = False,
 ) -> str:
     """
     Create the m3u file.
 
     ### Arguments
     - file_name: the file name to use
     - song_list: the list of songs
     - template: the template to use
     - file_extension: the file extension to use
-    - restrict: whether to sanitize the filename
+    - restrict: sanitization to apply to the filename
     - short: whether to use the short version of the template
 
     ### Returns
     - the m3u content as a string
     """
 
     m3u_content = create_m3u_content(
```

### Comparing `spotdl-4.1.9/spotdl/utils/matching.py` & `spotdl-4.2.0/spotdl/utils/matching.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,22 @@
     "remastered",
     "remaster",
     "reverb",
     "bassboost",
     "live",
     "acoustic",
     "8daudio",
+    "concert",
+    "live",
+    "acapella",
+    "slowed",
+    "instrumental",
+    "remix",
+    "cover",
+    "reverb",
 ]
 
 
 def debug(song_id: str, result_id: str, message: str) -> None:
     """
     Log a message with MATCH level
 
@@ -367,23 +375,24 @@
     if len(song.artists) == 1 or not result.artists:
         return artist_match_number
 
     artist1_list, artist2_list = based_sort(
         list(map(slugify, song.artists)), list(map(slugify, result.artists))
     )
 
+    # Remove main artist from the lists
+    artist1_list, artist2_list = artist1_list[1:], artist2_list[1:]
+
     artists_match = 0.0
     for artist1, artist2 in zip_longest(artist1_list, artist2_list):
         artist12_match = ratio(artist1, artist2)
         artists_match += artist12_match
 
     artist_match_number = artists_match / len(artist1_list)
 
-    debug(song.song_id, result.result_id, f"Artists match: {artist_match_number}")
-
     return artist_match_number
 
 
 def artists_match_fixup1(song: Song, result: Result, score: float) -> float:
     """
     Multiple fixes to the artists score for
     not verified results to improve the accuracy
@@ -449,54 +458,21 @@
     if score > 70 or not result.verified:
         # Don't fixup the score
         # if the artist match is already high
         # or if the result is not verified
         return score
 
     # Slugify some variables
-    slug_song_artist = slugify(song.artists[0])
     slug_song_name = slugify(song.name)
     slug_result_name = slugify(result.name)
-    slug_result_artists = slugify(", ".join(result.artists)) if result.artists else ""
 
-    # Check if the main artist is simlar
+    # # Check if the main artist is simlar
     has_main_artist = (score / (2 if len(song.artists) > 1 else 1)) > 50
 
-    match_str1, match_str2 = create_match_strings(song, result, search_query)
-
-    # Add 10 points to the score
-    # if the name match is greater than 75%
-    if ratio(match_str1, match_str2) >= 75:
-        score += 10
-
-    # If the result doesn't have the same number of artists but has
-    # the same main artist and similar name
-    # we add 25% to the artist match
-    if (
-        result.artists
-        and len(result.artists) < len(song.artists)
-        and slug_song_artist.replace("-", "")
-        in [
-            slug_result_artists.replace("-", ""),
-            slug_result_name.replace("-", ""),
-        ]
-    ):
-        score += 25
-
-    # Check if the song album name is very similar to the result album name
-    # if it is, we increase the artist match
-    if result.album:
-        if (
-            ratio(
-                slugify(result.album),
-                slugify(song.album_name),
-            )
-            >= 85
-        ):
-            score += 10
+    _, match_str2 = create_match_strings(song, result, search_query)
 
     # Check if other song artists are in the result name
     # if they are, we increase the artist match
     # (main artist is already checked, so we skip it)
     artists_to_check = song.artists[int(has_main_artist) :]
     for artist in artists_to_check:
         artist = slugify(artist).replace("-", "")
@@ -696,21 +672,23 @@
         # Calculate match value for all artists
         other_artists_match = calc_artists_match(song, result)
         debug(
             song.song_id,
             result.result_id,
             f"Other artists match: {other_artists_match}",
         )
+
         artists_match += other_artists_match
 
         # Calculate initial artist match value
-        artists_match = artists_match / (2 if len(song.artists) > 1 else 1)
         debug(song.song_id, result.result_id, f"Initial artists match: {artists_match}")
+        artists_match = artists_match / (2 if len(song.artists) > 1 else 1)
+        debug(song.song_id, result.result_id, f"First artists match: {artists_match}")
 
-        # First attempt to fix artist match
+        # # First attempt to fix artist match
         artists_match = artists_match_fixup1(song, result, artists_match)
         debug(
             song.song_id,
             result.result_id,
             f"Artists match after fixup1: {artists_match}",
         )
 
@@ -753,20 +731,20 @@
         album_match = calc_album_match(song, result)
         debug(song.song_id, result.result_id, f"Final album match: {album_match}")
 
         # Calculate time match
         time_match = calc_time_match(song, result)
         debug(song.song_id, result.result_id, f"Final time match: {time_match}")
 
-        # Ignore results with name match lower than 50%
-        if name_match <= 50:
+        # Ignore results with name match lower than 60%
+        if name_match <= 60:
             debug(
                 song.song_id,
                 result.result_id,
-                "Skipping result due to name match lower than 50%",
+                "Skipping result due to name match lower than 60%",
             )
             continue
 
         # Ignore results with artists match lower than 70%
         if artists_match < 70 and result.source != "slider.kz":
             debug(
                 song.song_id,
```

### Comparing `spotdl-4.1.9/spotdl/utils/metadata.py` & `spotdl-4.2.0/spotdl/utils/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,48 @@
     song=song_object,
     file_format="mp3",
 )
 ```
 """
 
 import base64
+import logging
 import re
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import requests
 from mutagen._file import File
 from mutagen.flac import Picture
 from mutagen.id3 import ID3
-from mutagen.id3._frames import APIC, COMM, SYLT, USLT, WOAS
+from mutagen.id3._frames import (
+    APIC,
+    COMM,
+    POPM,
+    SYLT,
+    TALB,
+    TCOM,
+    TCON,
+    TCOP,
+    TDRC,
+    TIT2,
+    TPE1,
+    TRCK,
+    USLT,
+    WOAS,
+)
 from mutagen.id3._specs import Encoding
 from mutagen.mp4 import MP4Cover
+from mutagen.wave import WAVE
 
 from spotdl.types.song import Song
 from spotdl.utils.formatter import to_ms
 
+logger = logging.getLogger(__name__)
+
 __all__ = [
     "MetadataError",
     "M4A_TAG_PRESET",
     "MP3_TAG_PRESET",
     "TAG_PRESET",
     "TAG_TO_SONG",
     "M4A_TO_SONG",
@@ -52,15 +71,14 @@
 # http://mutagen.readthedocs.io/en/latest/api/mp4.html
 M4A_TAG_PRESET = {
     "album": "\xa9alb",
     "artist": "\xa9ART",
     "date": "\xa9day",
     "title": "\xa9nam",
     "year": "\xa9day",
-    "originaldate": "purd",
     "comment": "\xa9cmt",
     "group": "\xa9grp",
     "writer": "\xa9wrt",
     "genre": "\xa9gen",
     "tracknumber": "trkn",
     "albumartist": "aART",
     "discnumber": "disk",
@@ -68,37 +86,38 @@
     "albumart": "covr",
     "encodedby": "\xa9too",
     "copyright": "cprt",
     "tempo": "tmpo",
     "lyrics": "\xa9lyr",
     "explicit": "rtng",
     "woas": "----:spotdl:WOAS",
+    "isrc": "----:spotdl:ISRC",
 }
 
 MP3_TAG_PRESET = {
     "album": "TALB",
     "artist": "TPE1",
     "date": "TDRC",
     "title": "TIT2",
     "year": "TDRC",
-    "originaldate": "TDOR",
     "comment": "COMM::XXX",
     "group": "TIT1",
     "writer": "TEXT",
     "genre": "TCON",
     "tracknumber": "TRCK",
     "albumartist": "TPE2",
     "discnumber": "TPOS",
     "cpil": "TCMP",
     "albumart": "APIC",
     "encodedby": "TENC",
     "copyright": "TCOP",
     "tempo": "TBPM",
     "lyrics": "USLT::XXX",
     "woas": "WOAS",
+    "isrc": "ISRC",
     "explicit": "NULL",
 }
 
 TAG_PRESET = {key: key for key in M4A_TAG_PRESET}
 
 TAG_TO_SONG = {
     "title": "name",
@@ -108,14 +127,15 @@
     "genre": "genres",
     "discnumber": "disc_number",
     "year": "year",
     "date": "date",
     "tracknumber": "track_number",
     "encodedby": "publisher",
     "woas": "url",
+    "isrc": "isrc",
     "copyright": "copyright_text",
     "lyrics": "lyrics",
     "albumart": "album_art",
 }
 
 M4A_TO_SONG = {
     value: TAG_TO_SONG.get(key)
@@ -139,14 +159,18 @@
     - output_file: Path to the output file.
     - song: Song object.
     """
 
     # Get the file extension for the output file
     encoding = output_file.suffix[1:]
 
+    if encoding == "wav":
+        embed_wav_file(output_file, song)
+        return
+
     # Get the tag preset for the file extension
     tag_preset = TAG_PRESET if encoding != "m4a" else M4A_TAG_PRESET
 
     try:
         audio_file = File(str(output_file.resolve()), easy=encoding == "mp3")
 
         if audio_file is None:
@@ -159,15 +183,14 @@
     # Embed basic metadata
     audio_file[tag_preset["artist"]] = song.artists
     audio_file[tag_preset["albumartist"]] = (
         song.album_artist if song.album_artist else song.artist
     )
     audio_file[tag_preset["title"]] = song.name
     audio_file[tag_preset["date"]] = song.date
-    audio_file[tag_preset["originaldate"]] = song.date
     audio_file[tag_preset["encodedby"]] = song.publisher
 
     # Embed metadata that isn't always present
     album_name = song.album_name
     if album_name:
         audio_file[tag_preset["album"]] = album_name
 
@@ -185,14 +208,15 @@
         # Zero fill the disc and track numbers
         zfilled_disc_number = str(song.disc_number).zfill(len(str(song.disc_count)))
         zfilled_track_number = str(song.track_number).zfill(len(str(song.tracks_count)))
 
         audio_file[tag_preset["discnumber"]] = zfilled_disc_number
         audio_file[tag_preset["tracknumber"]] = zfilled_track_number
         audio_file[tag_preset["woas"]] = song.url
+        audio_file[tag_preset["isrc"]] = song.isrc
     elif encoding == "m4a":
         audio_file[tag_preset["discnumber"]] = [(song.disc_number, song.disc_count)]
         audio_file[tag_preset["tracknumber"]] = [(song.track_number, song.tracks_count)]
         audio_file[tag_preset["explicit"]] = (4 if song.explicit is True else 2,)
         audio_file[tag_preset["woas"]] = song.url.encode("utf-8")
     elif encoding == "mp3":
         audio_file["tracknumber"] = f"{str(song.track_number)}/{str(song.tracks_count)}"
@@ -208,14 +232,21 @@
         audio_file = ID3(str(output_file.resolve()))
 
         audio_file.add(WOAS(encoding=3, url=song.url))
 
         if song.download_url:
             audio_file.add(COMM(encoding=3, text=song.download_url))
 
+        if song.popularity:
+            audio_file.add(
+                POPM(
+                    rating=int(song.popularity * 255 / 100),
+                )
+            )
+
     # Embed album art
     audio_file = embed_cover(audio_file, song, encoding)
 
     # Embed lyrics
     audio_file = embed_lyrics(audio_file, song, encoding)
 
     # Mp3 specific encoding
@@ -324,17 +355,15 @@
                     continue
 
                 minute, sec, millisecond = time_tag_vals
                 time = to_ms(min=minute, sec=sec, ms=millisecond)
                 lrc_data.append((text, time))
 
             audio_file.add(USLT(encoding=3, text=song.lyrics))
-            audio_file.add(
-                SYLT(encoding=Encoding.UTF8, text=lrc_data, format=2, type=1)
-            )
+            audio_file.add(SYLT(encoding=3, text=lrc_data, format=2, type=1))
         else:
             audio_file[tag_preset["lyrics"]] = song.lyrics
 
     return audio_file
 
 
 def get_file_metadata(path: Path, id3_separator: str = "/") -> Optional[Dict[str, Any]]:
@@ -465,16 +494,14 @@
                         val[0] if isinstance(val, list) and len(val) == 1 else val
                     )
 
         # FLAC, OGG, OPUS specific decoding
         else:
             if key == "artist":
                 song_meta["artists"] = val
-            if key == "originaldate":
-                song_meta["year"] = int(str(val[0])[:4])
             elif key == "tracknumber":
                 song_meta["track_number"] = int(val[0])
             elif key == "discnumber":
                 song_meta["disc_count"] = int(val[0])
                 song_meta["disc_number"] = int(val[0])
             else:
                 meta_key = TAG_TO_SONG.get(key)
@@ -498,7 +525,96 @@
     # Add main artist to the song meta object
     if song_meta["artists"]:
         song_meta["artist"] = song_meta["artists"][0]
     else:
         song_meta["artist"] = None
 
     return song_meta
+
+
+def embed_wav_file(output_file: Path, song: Song):
+    """
+    Embeds the song metadata into the wav file
+
+    ### Arguments
+    - output_file: The output file path
+    - song: The song object
+    - id3_separator: The separator used for the id3 tags
+    """
+    audio = WAVE(output_file)
+    if audio is None:
+        raise ValueError("Invalid audio file")
+
+    if audio.tags:
+        audio.tags.clear()
+
+    audio.add_tags()
+
+    audio.tags.add(TIT2(encoding=3, text=song.name))  # type: ignore
+    audio.tags.add(TPE1(encoding=3, text=song.artists))  # type: ignore
+    audio.tags.add(TALB(encoding=3, text=song.album_name))  # type: ignore
+    audio.tags.add(TCOM(encoding=3, text=song.publisher))  # type: ignore
+    audio.tags.add(TCON(encoding=3, text=song.genres))  # type: ignore
+    audio.tags.add(TDRC(encoding=3, text=song.date))  # type: ignore
+    audio.tags.add(  # type: ignore
+        TRCK(encoding=3, text=f"{song.track_number}/{song.tracks_count}")  # type: ignore
+    )
+    audio.tags.add(TDRC(encoding=3, text=song.date))  # type: ignore
+    audio.tags.add(WOAS(encoding=3, text=song.url))  # type: ignore
+
+    if song.download_url:
+        audio.tags.add(COMM(encoding=3, text=song.download_url))  # type: ignore
+
+    if song.copyright_text:
+        audio.tags.add(TCOP(encoding=3, text=song.copyright_text))  # type: ignore
+
+    if song.popularity:
+        audio.tags.add(  # type: ignore
+            COMM(
+                encoding=3,
+                lang="eng",
+                text="Spotify Popularity: " + str(song.popularity),
+            )
+        )
+
+    if song.cover_url:
+        try:
+            cover_data = requests.get(song.cover_url, timeout=10).content
+            audio.tags.add(  # type: ignore
+                APIC(
+                    encoding=3, mime="image/jpeg", type=3, desc="Cover", data=cover_data
+                )
+            )
+        except Exception:
+            pass
+
+    if song.lyrics:
+        # Check if the lyrics are in lrc format
+        # using regex on the first 5 lines
+        lrc_lines = song.lyrics.splitlines()[:5]
+        lrc_lines = [line for line in lrc_lines if line and LRC_REGEX.match(line)]
+
+        if len(lrc_lines) == 0:
+            audio.tags.add(USLT(encoding=Encoding.UTF8, text=song.lyrics))  # type: ignore
+        else:
+            lrc_data = []
+            for line in song.lyrics.splitlines():
+                time_tag = line.split("]", 1)[0] + "]"
+                text = line.replace(time_tag, "")
+
+                time_tag = time_tag.replace("[", "")
+                time_tag = time_tag.replace("]", "")
+                time_tag = time_tag.replace(".", ":")
+                time_tag_vals = time_tag.split(":")
+                if len(time_tag_vals) != 3 or any(
+                    not isinstance(tag, int) for tag in time_tag_vals
+                ):
+                    continue
+
+                minute, sec, millisecond = time_tag_vals
+                time = to_ms(min=minute, sec=sec, ms=millisecond)
+                lrc_data.append((text, time))
+
+            audio.tags.add(USLT(encoding=3, text=song.lyrics))  # type: ignore
+            audio.tags.add(SYLT(encoding=3, text=lrc_data, format=2, type=1))  # type: ignore
+
+    audio.save()
```

### Comparing `spotdl-4.1.9/spotdl/utils/search.py` & `spotdl-4.2.0/spotdl/utils/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,37 +4,40 @@
 
 To use this module you must first initialize the SpotifyClient.
 """
 
 import concurrent.futures
 import json
 import logging
+import re
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import requests
 from ytmusicapi import YTMusic
 
 from spotdl.types.album import Album
 from spotdl.types.artist import Artist
 from spotdl.types.playlist import Playlist
 from spotdl.types.saved import Saved
 from spotdl.types.song import Song, SongList
 from spotdl.utils.metadata import get_file_metadata
+from spotdl.utils.spotify import SpotifyClient, SpotifyError
 
 __all__ = [
     "QueryError",
     "get_search_results",
     "parse_query",
     "get_simple_songs",
     "reinit_song",
     "get_song_from_file_metadata",
     "gather_known_songs",
     "create_ytm_album",
     "create_ytm_playlist",
+    "get_all_user_playlists",
 ]
 
 logger = logging.getLogger(__name__)
 client = None  # pylint: disable=invalid-name
 
 
 def get_ytm_client() -> YTMusic:
@@ -119,33 +122,51 @@
     """
 
     songs: List[Song] = []
     lists: List[SongList] = []
     for request in query:
         logger.info("Processing query: %s", request)
 
+        # Remove /intl-xxx/ from Spotify URLs with regex
+        request = re.sub(r"\/intl-\w+\/", "/", request)
+
         if (
-            ("youtube.com/watch?v=" in request or "youtu.be/" in request)
+            ("watch?v=" in request or "youtu.be/" in request)
             and "open.spotify.com" in request
             and "track" in request
             and "|" in request
         ):
             split_urls = request.split("|")
             if (
                 len(split_urls) <= 1
-                or not ("youtube" in split_urls[0] or "youtu.be" in split_urls[0])
+                or not ("watch?v=" in split_urls[0] or "youtu.be" in split_urls[0])
                 or "spotify" not in split_urls[1]
             ):
                 raise QueryError(
                     'Incorrect format used, please use "YouTubeURL|SpotifyURL"'
                 )
 
             songs.append(
                 Song.from_missing_data(url=split_urls[1], download_url=split_urls[0])
             )
+        elif "music.youtube.com/watch?v" in request:
+            track_data = get_ytm_client().get_song(request.split("?v=", 1)[1])
+
+            yt_song = Song.from_search_term(
+                f"{track_data['videoDetails']['author']} - {track_data['videoDetails']['title']}"
+            )
+
+            if use_ytm_data:
+                yt_song.name = track_data["title"]
+                yt_song.artist = track_data["author"]
+                yt_song.artists = [track_data["author"]]
+                yt_song.duration = track_data["lengthSeconds"]
+
+            yt_song.download_url = request
+            songs.append(yt_song)
         elif (
             "https://music.youtube.com/playlist?list=" in request
             or "https://music.youtube.com/browse/VLPL" in request
         ):
             split_urls = request.split("|")
             if len(split_urls) == 1:
                 if "?list=OLAK5uy_" in request:
@@ -192,17 +213,14 @@
 
                     lists.append(ytm_list)
                 else:
                     for index, song in enumerate(spot_list.songs):
                         song.download_url = ytm_list.songs[index].download_url
 
                     lists.append(spot_list)
-        elif "open.spotify.com/intl-" in request and "track" in request:
-            request = request.split("/intl-")[0] + "/track" + request.split("/track")[1]
-            songs.append(Song.from_url(url=request))
         elif "open.spotify.com" in request and "track" in request:
             songs.append(Song.from_url(url=request))
         elif "https://spotify.link/" in request:
             resp = requests.head(request, allow_redirects=True, timeout=10)
             songs.append(Song.from_url(url=resp.url))
         elif "open.spotify.com" in request and "playlist" in request:
             lists.append(Playlist.from_url(request, fetch_songs=False))
@@ -214,14 +232,16 @@
             lists.append(Album.from_search_term(request, fetch_songs=False))
         elif "playlist:" in request:
             lists.append(Playlist.from_search_term(request, fetch_songs=False))
         elif "artist:" in request:
             lists.append(Artist.from_search_term(request, fetch_songs=False))
         elif request == "saved":
             lists.append(Saved.from_url(request, fetch_songs=False))
+        elif request == "all-user-playlists":
+            lists.extend(get_all_user_playlists())
         elif request.endswith(".spotdl"):
             with open(request, "r", encoding="utf-8") as save_file:
                 for track in json.load(save_file):
                     # Append to songs
                     songs.append(Song.from_dict(track))
         else:
             songs.append(Song.from_search_term(request))
@@ -274,14 +294,47 @@
         album = Album.from_url(album_id, fetch_songs=False)
 
         songs.extend([Song.from_missing_data(**song.json) for song in album.songs])
 
     return songs
 
 
+def get_all_user_playlists() -> List[Playlist]:
+    """
+    Get all user playlists
+
+    ### Returns
+    - List of all user playlists
+    """
+
+    spotify_client = SpotifyClient()
+    if spotify_client.user_auth is False:  # type: ignore
+        raise SpotifyError("You must be logged in to use this function")
+
+    user_playlists_response = spotify_client.current_user_playlists()
+    if user_playlists_response is None:
+        raise SpotifyError("Couldn't get user playlists")
+
+    user_playlists = user_playlists_response["items"]
+
+    # Fetch all saved tracks
+    while user_playlists_response and user_playlists_response["next"]:
+        response = spotify_client.next(user_playlists_response)
+        if response is None:
+            break
+
+        user_playlists_response = response
+        user_playlists.extend(user_playlists_response["items"])
+
+    return [
+        Playlist.from_url(playlist["external_urls"]["spotify"], fetch_songs=False)
+        for playlist in user_playlists
+    ]
+
+
 def reinit_song(song: Song) -> Song:
     """
     Update song object with new data
     from Spotify
 
     ### Arguments
     - song: Song object
@@ -294,15 +347,15 @@
     if data.get("url"):
         new_data = Song.from_url(data["url"]).json
     elif data.get("song_id"):
         new_data = Song.from_url(
             "https://open.spotify.com/track/" + data["song_id"]
         ).json
     elif data.get("name") and data.get("artist"):
-        new_data = Song.from_search_term(data["name"]).json
+        new_data = Song.from_search_term(f"{data['artist']} - {data['name']}").json
     else:
         raise QueryError("Song object is missing required data to be reinitialized")
 
     for key in Song.__dataclass_fields__:  # type: ignore # pylint: disable=E1101
         val = data.get(key)
         new_val = new_data.get(key)
         if new_val is not None and val is None:
```

### Comparing `spotdl-4.1.9/spotdl/utils/spotify.py` & `spotdl-4.2.0/spotdl/utils/spotify.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/static.py` & `spotdl-4.2.0/spotdl/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.9/spotdl/utils/web.py` & `spotdl-4.2.0/spotdl/utils/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         """
         Called when a new client connects to the websocket.
         """
 
         await self.websocket.accept()
 
         # Add the connection to the list of connections
-        app_state.clients.append(self)
+        app_state.clients[self.client_id] = self
         app_state.logger.info("Client %s connected", self.client_id)
 
     async def send_update(self, update: Dict[str, Any]):
         """
         Send an update to the client.
 
         ### Arguments
@@ -179,17 +179,17 @@
         ### Arguments
         - client_id: The client's ID.
 
         ### Returns
         - returns the WebSocket instance.
         """
 
-        for instance in app_state.clients:
-            if instance.client_id == client_id:
-                return instance
+        instance = app_state.clients.get(client_id)
+        if instance:
+            return instance
 
         app_state.logger.error("Client %s not found", client_id)
 
         return None
 
 
 class ApplicationState:
@@ -198,15 +198,15 @@
     """
 
     api: FastAPI
     server: Server
     loop: asyncio.AbstractEventLoop
     web_settings: WebOptions
     downloader_settings: DownloaderOptions
-    clients: List[Client] = []
+    clients: Dict[str, Client] = {}
     logger: logging.Logger
 
 
 router = APIRouter()
 app_state: ApplicationState = ApplicationState()
 
 
@@ -253,17 +253,15 @@
 
     await Client(websocket, client_id).connect()
 
     try:
         while True:
             await websocket.receive_json()
     except WebSocketDisconnect:
-        instance = Client.get_instance(client_id)
-        if instance:
-            app_state.clients.remove(instance)
+        app_state.clients.pop(client_id, None)
 
         if (
             len(app_state.clients) == 0
             and app_state.web_settings["keep_alive"] is False
         ):
             app_state.logger.debug(
                 "No active connections, waiting 1s before shutting down"
@@ -456,14 +454,15 @@
     settings_cpy.update({k: v for k, v in settings.items() if v is not None})  # type: ignore
 
     state.logger.info(f"Applying settings: {settings_cpy}")
 
     new_settings = DownloaderOptions(**settings_cpy)  # type: ignore
 
     # Re-initialize downloader
+    client.downloader_settings = new_settings
     client.downloader = Downloader(
         new_settings,
         loop=state.loop,
     )
 
     return new_settings
```

### Comparing `spotdl-4.1.9/PKG-INFO` & `spotdl-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl
-Version: 4.1.9
+Version: 4.2.0
 Summary: Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
@@ -14,39 +14,37 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Utilities
+Requires-Dist: bandcamp-api (>=0.1.15,<0.2.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: mutagen (>=1.46.0,<2.0.0)
-Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: platformdirs (>=3.8.1,<4.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pykakasi (>=2.2.1,<3.0.0)
 Requires-Dist: python-slugify[unidecode] (>=8.0.1,<9.0.0)
-Requires-Dist: pytube (>=12.1.3,<13.0.0)
+Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: rapidfuzz (==2.15.1)
-Requires-Dist: requests (>=2.29.0,<3.0.0)
-Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: soundcloud-v2 (>=1.3.1,<2.0.0)
 Requires-Dist: spotipy (>=2.23.0,<3.0.0)
 Requires-Dist: syncedlyrics (>=0.5.0,<0.6.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
-Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
+Requires-Dist: yt-dlp (>=2023.7.6,<2024.0.0)
 Requires-Dist: ytmusicapi (>=0.22.0,<0.23.0) ; python_version < "3.8"
 Requires-Dist: ytmusicapi (>=0.24.0,<0.25.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://spotdl.rtfd.io/en/latest/
 Project-URL: Repository, https://github.com/spotDL/spotify-downloader.git
 Description-Content-Type: text/markdown
 
 
@@ -79,14 +77,16 @@
 
 ## Installation
 
 Refer to our [Installation Guide](https://spotdl.rtfd.io/en/latest/installation/) for more details.
 
 ### Python (Recommended Method)
   - _spotDL_ can be installed by running `pip install spotdl`.
+  - To update spotDL run `pip install --upgrade spotdl`
+
   > On some systems you might have to change `pip` to `pip3`.
 
 <details>
     <summary style="font-size:1.25em"><strong>Other options</strong></summary>
 
 - Prebuilt executable
   - You can download the latest version from the
@@ -111,15 +111,15 @@
     ```
 
  - Build from source
 	```bash
 	git clone https://github.com/spotDL/spotify-downloader && cd spotify-downloader
 	pip install poetry
 	poetry install
-	python3 scripts/build.py
+	poetry run python3 scripts/build.py
 	```
 	An executable is created in `spotify-downloader/dist/`.
 
 </details>
 
 
 ### Installing FFmpeg
@@ -162,15 +162,15 @@
     - Usage:
         `spotdl save [query] --save-file {filename}.spotdl`
 
 - `web`: Starts a web interface instead of using the command line. However, it has limited features and only supports downloading single songs.
 
 - `url`: Get direct download link for each song from the query.
     - Usage:
-        `spotdl web [query]`
+        `spotdl url [query]`
 
 - `sync`: Updates directories. Compares the directory with the current state of the playlist. Newly added songs will be downloaded and removed songs will be deleted. No other songs will be downloaded and no other files will be deleted.
 
     - Usage:
         `spotdl sync [query] --save-file {filename}.spotdl`
 
         This create a new **sync** file, to update the directory in the future, use:
```

