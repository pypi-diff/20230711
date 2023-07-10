# Comparing `tmp/seventeenlands-0.1.39.tar.gz` & `tmp/seventeenlands-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventeenlands-0.1.39.tar", last modified: Wed May 24 15:03:46 2023, max compression
+gzip compressed data, was "seventeenlands-0.1.40.tar", last modified: Mon Jul 10 22:10:12 2023, max compression
```

## Comparing `seventeenlands-0.1.39.tar` & `seventeenlands-0.1.40.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/
--rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2023-05-24 15:00:01.000000 seventeenlands-0.1.39/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      585 2023-05-24 15:00:01.000000 seventeenlands-0.1.39/README.md
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)      839 2023-05-24 15:03:39.000000 seventeenlands-0.1.39/setup.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/seventeenlands/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-24 15:00:01.000000 seventeenlands-0.1.39/seventeenlands/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    48442 2023-05-24 15:02:09.000000 seventeenlands-0.1.39/seventeenlands/mtga_follower.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/seventeenlands.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      315 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       70 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       15 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/top_level.txt
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2023-05-24 15:00:01.000000 seventeenlands-0.1.40/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      585 2023-05-24 15:00:01.000000 seventeenlands-0.1.40/README.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)      839 2023-07-10 22:10:05.000000 seventeenlands-0.1.40/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/seventeenlands/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-24 15:00:01.000000 seventeenlands-0.1.40/seventeenlands/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     4461 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/api_client.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1040 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/logging_utils.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    55087 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/mtga_follower.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2301 2023-07-10 22:09:48.000000 seventeenlands-0.1.40/seventeenlands/retry_utils.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-07-10 22:10:12.587261 seventeenlands-0.1.40/seventeenlands.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      406 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       70 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       15 2023-07-10 22:10:12.000000 seventeenlands-0.1.40/seventeenlands.egg-info/top_level.txt
```

### Comparing `seventeenlands-0.1.39/LICENSE` & `seventeenlands-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.39/PKG-INFO` & `seventeenlands-0.1.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventeenlands
-Version: 0.1.39
+Version: 0.1.40
 Summary: Utility to upload MTG Arena data to 17Lands.com
 Home-page: https://github.com/rconroy293/mtga-log-client
 Author: Robert Conroy
 Author-email: seventeenlands@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seventeenlands-0.1.39/README.md` & `seventeenlands-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.39/setup.py` & `seventeenlands-0.1.40/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seventeenlands",
-    version="0.1.39",
+    version="0.1.40",
     author="Robert Conroy",
     author_email="seventeenlands@gmail.com",
     description="Utility to upload MTG Arena data to 17Lands.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rconroy293/mtga-log-client",
     packages=setuptools.find_packages(),
```

### Comparing `seventeenlands-0.1.39/seventeenlands/mtga_follower.py` & `seventeenlands-0.1.40/seventeenlands/mtga_follower.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,81 +12,112 @@
 """
 
 import argparse
 import copy
 import datetime
 import json
 import getpass
-import gzip
 import itertools
-import logging
-import logging.handlers
 import os
 import os.path
 import pathlib
 import re
 import subprocess
 import sys
 import time
 import traceback
 import uuid
 
-from collections import defaultdict, namedtuple
+from collections import defaultdict
 
 import dateutil.parser
-import requests
 
-LOG_FOLDER = os.path.join(os.path.expanduser('~'), '.seventeenlands')
-if not os.path.exists(LOG_FOLDER):
-    os.makedirs(LOG_FOLDER)
-LOG_FILENAME = os.path.join(LOG_FOLDER, 'seventeenlands.log')
-
-log_formatter = logging.Formatter('%(asctime)s,%(levelname)s,%(message)s', datefmt='%Y%m%d %H%M%S')
-handlers = {
-    logging.handlers.TimedRotatingFileHandler(LOG_FILENAME, when='D', interval=1, backupCount=7, utc=True),
-    logging.StreamHandler(),
-}
-logger = logging.getLogger('17Lands')
-for handler in handlers:
-    handler.setFormatter(log_formatter)
-    logger.addHandler(handler)
-logger.setLevel(logging.INFO)
-logger.info(f'Saving logs to {LOG_FILENAME}')
+import seventeenlands.api_client
+import seventeenlands.logging_utils
 
-CLIENT_VERSION = '0.1.39.p'
+logger = seventeenlands.logging_utils.get_logger('17Lands')
+
+CLIENT_VERSION = '0.1.40.p'
 
 UPDATE_CHECK_INTERVAL = datetime.timedelta(hours=1)
 UPDATE_PROMPT_FREQUENCY = 24
 
 TOKEN_ENTRY_TITLE = 'MTGA Log Client Token'
 TOKEN_ENTRY_MESSAGE = 'Please enter your client token from 17lands.com/account: '
 TOKEN_MISSING_TITLE = 'Error: Client Token Needed'
 TOKEN_MISSING_MESSAGE = 'Error: The program cannot continue without specifying a client token. Exiting.'
 TOKEN_INVALID_MESSAGE = 'That token is invalid. Please specify a valid client token. See 17lands.com/getting_started for more details.'
 
 FILE_UPDATED_FORCE_REFRESH_SECONDS = 60
 
 OSX_LOG_ROOT = os.path.join('Library','Logs')
-WINDOWS_LOG_ROOT = os.path.join('users', getpass.getuser(), 'AppData', 'LocalLow')
+WINDOWS_LOG_ROOT = os.path.join(
+    'users',
+    getpass.getuser(),
+    'AppData',
+    'LocalLow',
+)
+STEAM_LOG_ROOT = os.path.join(
+    'steamapps',
+    'compatdata',
+    '2141910',
+    'pfx',
+    'drive_c',
+    'users',
+    'steamuser',
+    'AppData',
+    'LocalLow',
+)
 LOG_INTERMEDIATE = os.path.join('Wizards Of The Coast', 'MTGA')
 CURRENT_LOG = 'Player.log'
 PREVIOUS_LOG = 'Player-prev.log'
 CURRENT_LOG_PATH = os.path.join(LOG_INTERMEDIATE, CURRENT_LOG)
 PREVIOUS_LOG_PATH = os.path.join(LOG_INTERMEDIATE, PREVIOUS_LOG)
 
 POSSIBLE_ROOTS = (
+    # OSX
+    os.path.join(os.path.expanduser('~'), OSX_LOG_ROOT),
+
+    # Steam
+    os.path.join(
+        os.path.expanduser('~'),
+        '.steam',
+        'steam',
+        STEAM_LOG_ROOT,
+    ),
+    os.path.join(
+        os.path.expanduser('~'),
+        '.local',
+        'share',
+        'Steam',
+        STEAM_LOG_ROOT,
+    ),
+
     # Windows
     os.path.join('C:/', WINDOWS_LOG_ROOT),
     os.path.join('D:/', WINDOWS_LOG_ROOT),
+
     # Lutris
-    os.path.join(os.path.expanduser('~'), 'Games', 'magic-the-gathering-arena', 'drive_c', WINDOWS_LOG_ROOT),
+    os.path.join(
+        os.path.expanduser('~'),
+        'Games',
+        'magic-the-gathering-arena',
+        'drive_c',
+        WINDOWS_LOG_ROOT,
+    ),
+
     # Wine
-    os.path.join(os.environ.get('WINEPREFIX', os.path.join(os.path.expanduser('~'), '.wine')), 'drive_c', WINDOWS_LOG_ROOT),
-    # OSX
-    os.path.join(os.path.expanduser('~'), OSX_LOG_ROOT),
+    os.path.join(
+        os.environ.get(
+            'WINEPREFIX',
+            os.path.join(os.path.expanduser('~'), '.wine'),
+        ),
+        'drive_c',
+        WINDOWS_LOG_ROOT,
+    ),
 )
 
 POSSIBLE_CURRENT_FILEPATHS = list(map(lambda root_and_path: os.path.join(*root_and_path), itertools.product(POSSIBLE_ROOTS, (CURRENT_LOG_PATH, ))))
 POSSIBLE_PREVIOUS_FILEPATHS = list(map(lambda root_and_path: os.path.join(*root_and_path), itertools.product(POSSIBLE_ROOTS, (PREVIOUS_LOG_PATH, ))))
 
 CONFIG_FILE = os.path.join(os.path.expanduser('~'), '.mtga_follower.ini')
 
@@ -109,37 +140,17 @@
     '%Y/%m/%d %I:%M:%S %p',
     '%d/%m/%Y %H:%M:%S',
     '%d/%m/%Y %I:%M:%S %p',
     '%d.%m.%Y %H:%M:%S',
     '%d.%m.%Y %I:%M:%S %p'
 )
 OUTPUT_TIME_FORMAT = '%Y%m%d%H%M%S'
+MAX_MILLISECONDS_SINCE_EPOCH = int(1000 * datetime.datetime(3000, 1, 1).timestamp())
 
-API_ENDPOINT = 'https://www.17lands.com'
-ENDPOINT_USER = 'api/account'
-ENDPOINT_DECK_SUBMISSION = 'deck'
-ENDPOINT_EVENT_SUBMISSION = 'event'
-ENDPOINT_EVENT_COURSE_SUBMISSION = 'event_course'
-ENDPOINT_GAME_RESULT = 'game'
-ENDPOINT_DRAFT_PACK = 'pack'
-ENDPOINT_DRAFT_PICK = 'pick'
-ENDPOINT_HUMAN_DRAFT_PICK = 'human_draft_pick'
-ENDPOINT_HUMAN_DRAFT_PACK = 'human_draft_pack'
-ENDPOINT_COLLECTION = 'collection'
-ENDPOINT_INVENTORY = 'inventory'
-ENDPOINT_PLAYER_PROGRESS = 'player_progress'
-ENDPOINT_CLIENT_VERSION = 'api/version_validation'
-ENDPOINT_RANK = 'api/rank'
-ENDPOINT_ONGOING_EVENTS = 'ongoing_events'
-ENDPOINT_EVENT_ENDED = 'event_ended'
-
-RETRIES = 2
-IS_CODE_FOR_RETRY = lambda code: code >= 500 and code < 600
-IS_SUCCESS_CODE = lambda code: code >= 200 and code < 300
-DEFAULT_RETRY_SLEEP_TIME = 1
+_ERROR_LINES_RECENCY = 10
 
 
 def extract_time(time_str):
     """
     Convert a time string in various formats to a datetime.
 
     :param time_str: The string to convert.
@@ -154,14 +165,15 @@
     for possible_format in TIME_FORMATS:
         try:
             return datetime.datetime.strptime(time_str, possible_format)
         except ValueError:
             pass
     raise ValueError(f'Unsupported time format: "{time_str}"')
 
+
 def json_value_matches(expectation, path, blob):
     """
     Check if the value nested at a given path in a JSON blob matches the expected value.
 
     :param expectation: The value to check against.
     :param path:        A list of keys for the nested value.
     :param blob:        The JSON blob to check in.
@@ -171,41 +183,48 @@
     for p in path:
         if p in blob:
             blob = blob[p]
         else:
             return False
     return blob == expectation
 
+
 def get_rank_string(rank_class, level, percentile, place, step):
     """
     Convert the components of rank into a serializable value for recording
 
     :param rank_class: Class (e.g. Bronze, Mythic)
     :param level:      Level within the class
     :param percentile: Percentile (within Mythic)
     :param place:      Leaderboard place (within Mythic)
     :param step:       Step towards next level
 
     :returns: Serialized rank string (e.g. "Gold-3-0.0-0-2")
     """
     return '-'.join(str(x) for x in [rank_class, level, percentile, place, step])
 
+
 class Follower:
     """Follows along a log, parses the messages, and passes along the parsed data to the API endpoint."""
 
     def __init__(self, token, host):
         self.host = host
         self.token = token
+        self.json_decoder = json.JSONDecoder()
+        self._api_client = seventeenlands.api_client.ApiClient(host=host)
+        self._reinitialize()
+
+    def _reinitialize(self):
         self.buffer = []
         self.cur_log_time = datetime.datetime.fromtimestamp(0)
         self.last_utc_time = datetime.datetime.fromtimestamp(0)
         self.last_raw_time = ''
-        self.json_decoder = json.JSONDecoder()
         self.disconnected_user = None
         self.disconnected_screen_name = None
+        self.disconnected_rank = None
         self.cur_user = None
         self.cur_draft_event = None
         self.cur_rank_data = None
         self.cur_opponent_level = None
         self.cur_opponent_match_id = None
         self.current_match_id = None
         self.current_event_id = None
@@ -221,72 +240,58 @@
         self.opening_hand = defaultdict(list)
         self.drawn_hands = defaultdict(list)
         self.drawn_cards_by_instance_id = defaultdict(dict)
         self.cards_in_hand = defaultdict(list)
         self.user_screen_name = None
         self.screen_names = defaultdict(lambda: '')
         self.game_history_events = []
-        self.pending_game_submission = None
-
-
-    def __retry_post(self, endpoint, blob, num_retries=RETRIES, sleep_time=DEFAULT_RETRY_SLEEP_TIME, use_gzip=False):
-        """
-        Add client version to a JSON blob and send the data to an endpoint via post
-        request, retrying on server errors.
-
-        :param endpoint:    The http endpoint to hit.
-        :param blob:        The JSON data to send in the body of the post request.
-        :param num_retries: The number of times to retry upon failure.
-        :param sleep_time:  In seconds, the time to sleep between tries.
-
-        :returns: The response object (including status_code and text fields).
-        """
-        blob['client_version'] = CLIENT_VERSION
-        blob['token'] = self.token
-        blob['utc_time'] = self.last_utc_time.isoformat()
-
-        tries_left = num_retries + 1
-        while tries_left > 0:
-            tries_left -= 1
-            if use_gzip:
-                data = gzip.compress(json.dumps(blob).encode('utf8'))
-                response = requests.post(endpoint, data=data, headers={
-                    'content-type': 'application/json',
-                    'content-encoding': 'gzip',
-                })
-            else:
-                response = requests.post(endpoint, json=blob)
-            if not IS_CODE_FOR_RETRY(response.status_code):
-                break
-            logger.warning(f'Got response code {response.status_code}; retrying {tries_left} more times')
-            time.sleep(sleep_time)
-        logger.info(f'{response.status_code} Response: {response.text}')
-        return response
+        self.pending_game_submission = {}
+        self.pending_game_result = {}
+        self.pending_match_result = {}
+
+        self.current_debug_blob = ''
+        self.recent_lines = []
+
+        self.__clear_match_data()
+
+    def _add_base_api_data(self, blob):
+        return {
+            "token": self.token,
+            "client_version": CLIENT_VERSION,
+            "player_id": self.cur_user,
+            "time": self.cur_log_time.isoformat(),
+            "utc_time": self.last_utc_time.isoformat(),
+            "raw_time": self.last_raw_time,
+            **blob,
+        }
 
     def parse_log(self, filename, follow):
         """
         Parse messages from a log file and pass the data along to the API endpoint.
 
         :param filename: The filename for the log file to parse.
         :param follow:   Whether or not to continue looking for updates to the file after parsing
                          all the initial lines.
         """
         while True:
-            self.__clear_match_data()
+            self._reinitialize()
             last_read_time = time.time()
             last_file_size = 0
+            last_line = ''
             try:
                 with open(filename, errors='replace') as f:
                     while True:
                         line = f.readline()
                         file_size = pathlib.Path(filename).stat().st_size
                         if line:
-                            self.__append_line(line)
+                            if line != last_line:
+                                self.__append_line(line)
                             last_read_time = time.time()
                             last_file_size = file_size
+                            last_line = line
                         else:
                             self.__handle_complete_log_entry()
                             last_modified_time = os.stat(filename).st_mtime
                             if file_size < last_file_size:
                                 logger.info(f'Starting from beginning of file as file is smaller than before (previous = {last_file_size}; current = {file_size})')
                                 break
                             elif last_modified_time > last_read_time + FILE_UPDATED_FORCE_REFRESH_SECONDS:
@@ -294,19 +299,33 @@
                                 break
                             elif follow:
                                 time.sleep(SLEEP_TIME)
                             else:
                                 break
             except FileNotFoundError:
                 time.sleep(SLEEP_TIME)
+            except Exception as e:
+                self._log_error(
+                    message=f'Error parsing log: {e}',
+                    error=e,
+                    stacktrace=traceback.format_exc(),
+                )
 
             if not follow:
                 logger.info('Done processing file.')
                 break
 
+    def _log_error(self, message: str, error: Exception, stacktrace: str):
+        logger.error(message)
+        self._api_client.submit_error_info(self._add_base_api_data({
+            "blob": self.current_debug_blob,
+            "recent_lines": self.recent_lines,
+            "stacktrace": traceback.format_exc(),
+        }))
+
     def __check_detailed_logs(self, line):
         if (line.startswith('DETAILED LOGS: DISABLED')):
             logger.warning('Detailed logs are disabled in MTGA.')
             show_message(
                 title='MTGA Logging Disabled (17Lands)',
                 message=(
                     '17Lands needs detailed logging enabled in MTGA. To enable this, click the '
@@ -315,14 +334,18 @@
                 ),
             )
         elif (line.startswith('DETAILED LOGS: ENABLED')):
             logger.info('Detailed logs enabled in MTGA.')
 
     def __append_line(self, line):
         """Add a complete line (not necessarily a complete message) from the log."""
+        if len(self.recent_lines) >= _ERROR_LINES_RECENCY:
+            self.recent_lines.pop(0)
+        self.recent_lines.append(line)
+
         self.__check_detailed_logs(line)
 
         self.__maybe_handle_account_info(line)
 
         timestamp_match = TIMESTAMP_REGEX.match(line)
         if timestamp_match:
             self.last_raw_time = timestamp_match.group(1)
@@ -347,19 +370,23 @@
         if len(self.buffer) == 0:
             return
         if self.cur_log_time is None:
             self.buffer = []
             return
 
         full_log = ''.join(self.buffer)
+        self.current_debug_blob = full_log
         try:
             self.__handle_blob(full_log)
         except Exception as e:
-            logger.error(f'Error {e} while processing {full_log}')
-            logger.error(traceback.format_exc())
+            self._log_error(
+                message=f'Error {e} while processing {full_log}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
         self.buffer = []
         # self.cur_log_time = None
 
     def __maybe_get_utc_timestamp(self, blob):
         timestamp = None
         if 'timestamp' in blob:
@@ -369,16 +396,23 @@
         elif 'timestamp' in blob.get('params', {}).get('payloadObject', {}):
             timestamp = blob['params']['payloadObject']['timestamp']
 
         if timestamp is None:
             return None
 
         try:
-            seconds_since_year_1 = int(timestamp) / 10000000
-            return datetime.datetime.fromordinal(1) + datetime.timedelta(seconds=seconds_since_year_1)
+            timestamp_value = int(timestamp)
+
+            if timestamp_value < MAX_MILLISECONDS_SINCE_EPOCH:
+                return datetime.datetime.fromtimestamp(timestamp_value * 0.001)
+
+            else:
+                seconds_since_year_1 = timestamp_value / 10000000
+                return datetime.datetime.fromordinal(1) + datetime.timedelta(seconds=seconds_since_year_1)
+
         except ValueError:
             return dateutil.parser.isoparse(timestamp)
 
     def __handle_blob(self, full_log):
         """Attempt to parse a complete log message and send the data if relevant."""
         match = JSON_START_REGEX.search(full_log)
         if not match:
@@ -389,14 +423,15 @@
         except json.JSONDecodeError as e:
             logger.debug(f'Ran into error {e} when parsing at {self.cur_log_time}. Data was: {full_log}')
             return
 
         json_obj = self.__extract_payload(json_obj)
         if type(json_obj) != dict: return
 
+        maybe_time = None
         try:
             maybe_time = self.__maybe_get_utc_timestamp(json_obj)
             if maybe_time is not None:
                 self.last_utc_time = maybe_time
         except:
             pass
 
@@ -406,14 +441,16 @@
             self.__handle_joined_pod(json_obj)
         elif 'DraftStatus' in json_obj:
             self.__handle_bot_draft_pack(json_obj)
         elif 'BotDraft_DraftPick' in full_log and 'PickInfo' in json_obj:
             self.__handle_bot_draft_pick(json_obj['PickInfo'])
         elif 'LogBusinessEvents' in full_log and 'PickGrpId' in json_obj:
             self.__handle_human_draft_combined(json_obj)
+        elif 'LogBusinessEvents' in full_log and 'WinningType' in json_obj:
+            self.__handle_log_business_game_end(json_obj)
         elif 'Draft.Notify ' in full_log and 'method' not in json_obj:
             self.__handle_human_draft_pack(json_obj)
         elif 'Event_SetDeck' in full_log and 'EventName' in json_obj:
             self.__handle_deck_submission(json_obj)
         elif 'Event_GetCourses' in full_log and 'Courses' in json_obj:
             self.__handle_ongoing_events(json_obj)
         elif 'Event_ClaimPrize' in full_log and 'EventName' in json_obj:
@@ -421,39 +458,40 @@
         elif 'Draft_CompleteDraft' in full_log and 'DraftId' in json_obj:
             self.__handle_event_course(json_obj)
         elif 'authenticateResponse' in json_obj:
             self.__update_screen_name(json_obj['authenticateResponse']['screenName'])
         elif 'matchGameRoomStateChangedEvent' in json_obj:
             self.__handle_match_state_changed(json_obj)
         elif 'greToClientEvent' in json_obj and 'greToClientMessages' in json_obj['greToClientEvent']:
-            for message in json_obj['greToClientEvent']['greToClientMessages']:
-                self.__handle_gre_to_client_message(message)
+            try:
+                for message in json_obj['greToClientEvent']['greToClientMessages']:
+                    self.__handle_gre_to_client_message(message, maybe_time)
+            except Exception as e:
+                self._log_error(
+                    message=f'Error {e} parsing GRE to client messages from {json_obj}',
+                    error=e,
+                    stacktrace=traceback.format_exc(),
+                )
         elif json_value_matches('ClientToMatchServiceMessageType_ClientToGREMessage', ['clientToMatchServiceMessageType'], json_obj):
-            self.__handle_client_to_gre_message(json_obj.get('payload', {}))
+            self.__handle_client_to_gre_message(json_obj.get('payload', {}), maybe_time)
         elif json_value_matches('ClientToMatchServiceMessageType_ClientToGREUIMessage', ['clientToMatchServiceMessageType'], json_obj):
-            self.__handle_client_to_gre_ui_message(json_obj.get('payload', {}))
-        elif 'Rank_GetCombinedRankInfo' in full_log:
+            self.__handle_client_to_gre_ui_message(json_obj.get('payload', {}), maybe_time)
+        elif 'Rank_GetCombinedRankInfo' in full_log and 'limitedSeasonOrdinal' in json_obj:
             self.__handle_self_rank_info(json_obj)
         elif ' PlayerInventory.GetPlayerCardsV3 ' in full_log and 'method' not in json_obj: # Doesn't exist any more
             self.__handle_collection(json_obj)
         elif 'DTO_InventoryInfo' in json_obj:
             self.__handle_inventory(json_obj['DTO_InventoryInfo'])
         elif 'NodeStates' in json_obj and 'RewardTierUpgrade' in json_obj['NodeStates']:
             self.__handle_player_progress(json_obj)
         elif 'FrontDoorConnection.Close ' in full_log:
             self.__reset_current_user()
         elif 'Reconnect result : Connected' in full_log:
             self.__handle_reconnect_result()
 
-        if self.pending_game_submission:
-            logger.info(f'Submitting game with {len(self.pending_game_submission["history"]["events"])} history events')
-            response = self.__retry_post(f'{self.host}/{ENDPOINT_GAME_RESULT}', blob=self.pending_game_submission, use_gzip=True)
-            self.__clear_game_data()
-            self.pending_game_submission = None
-
     def __try_decode(self, blob, key):
         try:
             json_obj, _ = self.json_decoder.raw_decode(blob[key])
             return json_obj
         except Exception:
             return blob[key]
 
@@ -465,25 +503,32 @@
             if key in blob:
                 # Some messages are recursively serialized
                 return self.__extract_payload(self.__try_decode(blob, key))
 
         return blob
 
     def __update_screen_name(self, screen_name):
-        if self.user_screen_name == screen_name or '#' not in screen_name:
-            return
+        try:
+            if self.user_screen_name == screen_name or '#' not in screen_name:
+                return
 
-        self.user_screen_name = screen_name
-        user_info = {
-            'player_id': self.cur_user,
-            'screen_name': self.user_screen_name,
-            'raw_time': self.last_raw_time,
-        }
-        logger.info(f'Updating user info: {user_info}')
-        self.__retry_post(f'{self.host}/{ENDPOINT_USER}', blob=user_info)
+            self.user_screen_name = screen_name
+            user_info = {
+                'player_id': self.cur_user,
+                'screen_name': self.user_screen_name,
+            }
+            logger.info(f'Updating user info: {user_info}')
+            self._api_client.submit_user(self._add_base_api_data(user_info))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing screen name from {screen_name}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_match_state_changed(self, blob):
         game_room_info = blob.get('matchGameRoomStateChangedEvent', {}).get('gameRoomInfo', {})
         game_room_config = game_room_info.get('gameRoomConfig', {})
 
         updated_match_id = game_room_config.get('matchId')
         updated_event_id = game_room_config.get('eventId')
@@ -518,148 +563,229 @@
         if 'serviceMetadata' in game_room_config:
             self.game_service_metadata = game_room_config['serviceMetadata']
 
         if 'clientMetadata' in game_room_config:
             self.game_client_metadata = game_room_config['clientMetadata']
 
         if 'finalMatchResult' in game_room_info:
-            # If the regular game end message is lost, try to submit remaining game data on match end.
             results = game_room_info['finalMatchResult'].get('resultList', [])
             if results:
-                self.__send_game_end(results)
-            self.__clear_match_data()
+                if self.__enqueue_game_data():
+                    self.__enqueue_game_results(results)
+            self.__clear_match_data(submit_pending_game=True)
+
+    def _add_to_game_history(self, message_blob, timestamp):
+        self.game_history_events.append({
+            "_timestamp": None if timestamp is None else timestamp.isoformat(),
+            **message_blob,
+        })
 
-    def __handle_gre_to_client_message(self, message_blob):
+    def __handle_gre_to_client_message(self, message_blob, timestamp):
         """Handle messages in the 'greToClientEvent' field."""
-        # Add to game history before processing the messsage, since we may submit the game right away.
+        # Add to game history before processing the message, since we may submit the game right away.
         if message_blob['type'] in ['GREMessageType_QueuedGameStateMessage', 'GREMessageType_GameStateMessage']:
-            self.game_history_events.append(message_blob)
+            self._add_to_game_history(message_blob, timestamp)
         elif message_blob['type'] == 'GREMessageType_UIMessage' and 'onChat' in message_blob['uiMessage']:
-            self.game_history_events.append(message_blob)
+            self._add_to_game_history(message_blob, timestamp)
 
         if message_blob['type'] == 'GREMessageType_ConnectResp':
             self.__handle_gre_connect_response(message_blob)
 
         elif message_blob['type'] == 'GREMessageType_GameStateMessage':
-            system_seat_ids = message_blob.get('systemSeatIds', [])
-            if len(system_seat_ids) > 0:
-                self.seat_id = system_seat_ids[0]
-
-            game_state_message = message_blob.get('gameStateMessage', {})
-
-            if 'gameInfo' in game_state_message:
-                game_info = game_state_message['gameInfo']
-                if game_info.get('matchID', self.current_match_id) != self.current_match_id:
-                    self.current_match_id = game_info['matchID']
-                    self.current_event_id = None
+            try:
+                system_seat_ids = message_blob.get('systemSeatIds', [])
+                if len(system_seat_ids) > 0:
+                    self.seat_id = system_seat_ids[0]
+
+                game_state_message = message_blob.get('gameStateMessage', {})
+
+                if 'gameInfo' in game_state_message:
+                    game_info = game_state_message['gameInfo']
+                    if game_info.get('matchID', self.current_match_id) != self.current_match_id:
+                        self.current_match_id = game_info['matchID']
+                        self.current_event_id = None
 
-            turn_info = game_state_message.get('turnInfo', {})
-            players = game_state_message.get('players', [])
+                turn_info = game_state_message.get('turnInfo', {})
+                players = game_state_message.get('players', [])
 
-            if turn_info.get('turnNumber'):
-                self.turn_count = turn_info.get('turnNumber')
-            else:
-                turns_sum = sum(p.get('turnNumber', 0) for p in players)
-                self.turn_count = max(self.turn_count, turns_sum)
+                if turn_info.get('turnNumber'):
+                    self.turn_count = turn_info.get('turnNumber')
+                else:
+                    turns_sum = sum(p.get('turnNumber', 0) for p in players)
+                    self.turn_count = max(self.turn_count, turns_sum)
 
-            for game_object in game_state_message.get('gameObjects', []):
-                if game_object['type'] not in ('GameObjectType_Card', 'GameObjectType_SplitCard'):
-                    continue
-                owner = game_object['ownerSeatId']
-                instance_id = game_object['instanceId']
-                card_id = game_object['overlayGrpId']
-
-                self.objects_by_owner[owner][instance_id] = card_id
-
-            for zone in game_state_message.get('zones', []):
-                if zone['type'] == 'ZoneType_Hand':
-                    owner = zone['ownerSeatId']
-                    player_objects = self.objects_by_owner[owner]
-                    hand_card_ids = zone.get('objectInstanceIds', [])
-                    self.cards_in_hand[owner] = [player_objects.get(instance_id) for instance_id in hand_card_ids if instance_id]
-                    for instance_id in hand_card_ids:
-                        card_id = player_objects.get(instance_id)
-                        if instance_id is not None and card_id is not None:
-                            self.drawn_cards_by_instance_id[owner][instance_id] = card_id
-
-            players_deciding_hand = {
-                (p['systemSeatNumber'], p.get('mulliganCount', 0))
-                for p in players
-                if p.get('pendingMessageType') == 'ClientMessageType_MulliganResp'
-            }
-            for (player_id, mulligan_count) in players_deciding_hand:
-                if self.starting_team_id is None:
-                    self.starting_team_id = turn_info.get('activePlayer')
-                self.opening_hand_count_by_seat[player_id] += 1
-
-                if mulligan_count == len(self.drawn_hands[player_id]):
-                    self.drawn_hands[player_id].append(self.cards_in_hand[player_id].copy())
-
-            if len(self.opening_hand) == 0 and ('Phase_Beginning', 'Step_Upkeep', 1) == (turn_info.get('phase'), turn_info.get('step'), turn_info.get('turnNumber')):
-                for (owner, hand) in self.cards_in_hand.items():
-                    self.opening_hand[owner] = hand.copy()
+                for game_object in game_state_message.get('gameObjects', []):
+                    if game_object['type'] not in ('GameObjectType_Card', 'GameObjectType_SplitCard'):
+                        continue
+                    owner = game_object['ownerSeatId']
+                    instance_id = game_object['instanceId']
+                    card_id = game_object['overlayGrpId']
+
+                    self.objects_by_owner[owner][instance_id] = card_id
+
+                for zone in game_state_message.get('zones', []):
+                    if zone['type'] == 'ZoneType_Hand':
+                        owner = zone['ownerSeatId']
+                        player_objects = self.objects_by_owner[owner]
+                        hand_card_ids = zone.get('objectInstanceIds', [])
+                        self.cards_in_hand[owner] = [player_objects.get(instance_id) for instance_id in hand_card_ids if instance_id]
+                        for instance_id in hand_card_ids:
+                            card_id = player_objects.get(instance_id)
+                            if instance_id is not None and card_id is not None:
+                                self.drawn_cards_by_instance_id[owner][instance_id] = card_id
+
+                players_deciding_hand = {
+                    (p['systemSeatNumber'], p.get('mulliganCount', 0))
+                    for p in players
+                    if p.get('pendingMessageType') == 'ClientMessageType_MulliganResp'
+                }
+                for (player_id, mulligan_count) in players_deciding_hand:
+                    if self.starting_team_id is None:
+                        self.starting_team_id = turn_info.get('activePlayer')
+                    self.opening_hand_count_by_seat[player_id] += 1
+
+                    if mulligan_count == len(self.drawn_hands[player_id]):
+                        self.drawn_hands[player_id].append(self.cards_in_hand[player_id].copy())
+
+                if len(self.opening_hand) == 0 and ('Phase_Beginning', 'Step_Upkeep', 1) == (turn_info.get('phase'), turn_info.get('step'), turn_info.get('turnNumber')):
+                    for (owner, hand) in self.cards_in_hand.items():
+                        self.opening_hand[owner] = hand.copy()
+
+                self.__maybe_handle_game_over_stage(game_state_message)
+
+            except Exception as e:
+                self._log_error(
+                    message=f'Error {e} parsing GRE message from {message_blob}',
+                    error=e,
+                    stacktrace=traceback.format_exc(),
+                )
 
-            self.__maybe_handle_game_over_stage(game_state_message)
 
     def __handle_gre_connect_response(self, blob):
-        deck_info = blob.get('connectResp', {}).get('deckMessage', {})
-        self.current_game_maindeck = deck_info.pop('deckCards', [])
-        self.current_game_sideboard = deck_info.pop('sideboardCards', [])
-        self.current_game_additional_deck_info = deck_info
-
-    def __handle_client_to_gre_message(self, payload):
-        if payload['type'] == 'ClientMessageType_SelectNResp':
-            self.game_history_events.append(payload)
-
-        if payload['type'] == 'ClientMessageType_SubmitDeckResp':
-            deck_info = payload['submitDeckResp']['deck']
+        try:
+            deck_info = blob.get('connectResp', {}).get('deckMessage', {})
             self.current_game_maindeck = deck_info.pop('deckCards', [])
             self.current_game_sideboard = deck_info.pop('sideboardCards', [])
             self.current_game_additional_deck_info = deck_info
 
-    def __handle_client_to_gre_ui_message(self, payload):
-        if 'onChat' in payload['uiMessage']:
-            self.game_history_events.append(payload)
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing GRE connect response from {blob}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+    def __handle_client_to_gre_message(self, payload, timestamp):
+        try:
+            if payload['type'] == 'ClientMessageType_SelectNResp':
+                self._add_to_game_history(payload, timestamp)
+
+            if payload['type'] == 'ClientMessageType_SubmitDeckResp':
+                try:
+                    self.__clear_game_data()
+                    deck_info = payload['submitDeckResp']['deck']
+                    self.current_game_maindeck = deck_info.pop('deckCards', [])
+                    self.current_game_sideboard = deck_info.pop('sideboardCards', [])
+                    self.current_game_additional_deck_info = deck_info
+
+                except Exception as e:
+                    self._log_error(
+                        message=f'Error {e} parsing GRE deck submission from {payload}',
+                        error=e,
+                        stacktrace=traceback.format_exc(),
+                    )
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing GRE to client messages from {payload}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+    def __handle_client_to_gre_ui_message(self, payload, timestamp):
+        try:
+            if 'onChat' in payload['uiMessage']:
+                self._add_to_game_history(payload, timestamp)
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing GRE to client UI messages from {payload}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+    def __handle_log_business_game_end(self, payload):
+        try:
+            if self.starting_team_id is None:
+                self.starting_team_id = payload.get('StartingTeamId')
+
+            if self.__enqueue_game_data():
+                self.pending_game_result = {
+                    'game_number': payload.get('GameNumber'),
+                    'won': self.seat_id == payload.get('WinningTeamId'),
+                    'win_type': payload.get('WinningType'),
+                    'game_end_reason': payload.get('WinningReason'),
+                }
+                logger.info(f'Added pending game result via LogBusinessEvents {self.pending_game_result}')
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing game end from LogBusinessEvents: {payload}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __maybe_handle_game_over_stage(self, game_state_message):
         game_info = game_state_message.get('gameInfo', {})
         if game_info.get('stage') != 'GameStage_GameOver':
             return
 
         results = game_info.get('results')
         if results:
-            self.__send_game_end(results)
+            if self.__enqueue_game_data():
+                self.__enqueue_game_results(results)
 
-        if game_info.get('matchState') == 'MatchState_MatchComplete':
-            self.__clear_match_data()
+    def __maybe_submit_pending_game(self):
+        if self.pending_game_submission and self.pending_game_result:
+            full_game = {
+                **self.pending_game_result,
+                **self.pending_match_result,
+                **self.pending_game_submission,
+            }
+            logger.info(f'Submitting queued game result')
+            self._api_client.submit_game_result(self._add_base_api_data(full_game))
+            self.pending_game_submission = {}
+            self.__clear_game_data()
 
-    def __has_pending_game_data(self):
-        return len(self.drawn_cards_by_instance_id) > 0 and len(self.game_history_events) > 5
+    def __clear_game_data(self, submit_pending_game=True):
+        if submit_pending_game:
+            self.__maybe_submit_pending_game()
 
-    def __clear_game_data(self):
         self.turn_count = 0
         self.objects_by_owner.clear()
         self.opening_hand_count_by_seat.clear()
         self.opening_hand.clear()
         self.drawn_hands.clear()
         self.drawn_cards_by_instance_id.clear()
         self.starting_team_id = None
         self.game_history_events.clear()
         self.current_game_maindeck = None
         self.current_game_sideboard = None
         self.current_game_additional_deck_info = None
         self.game_service_metadata = None
         self.game_client_metadata = None
+        self.pending_game_result = {}
+        self.pending_match_result = {}
 
-    def __clear_match_data(self):
+    def __clear_match_data(self, submit_pending_game=False):
         self.screen_names.clear()
         self.current_match_id = None
         self.current_event_id = None
         self.seat_id = None
-        self.__clear_game_data()
+        self.__clear_game_data(submit_pending_game=submit_pending_game)
 
     def __maybe_handle_account_info(self, line):
         match = ACCOUNT_INFO_REGEX.match(line)
         if match:
             screen_name = match.group(1)
             self.cur_user = match.group(2)
             self.__update_screen_name(screen_name)
@@ -667,297 +793,410 @@
 
         match = MATCH_ACCOUNT_INFO_REGEX.match(line)
         if match:
             self.cur_user = match.group(2) or match.group(3)
 
     def __handle_ongoing_events(self, json_obj):
         """Handle 'Event_GetCourses' messages."""
-        event = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'courses': json_obj['Courses'],
-        }
-        logger.info(f'Updated ongoing events')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_ONGOING_EVENTS}', blob=event)
+        try:
+            event = {
+                'courses': json_obj['Courses'],
+            }
+            logger.info(f'Updated ongoing events')
+            self._api_client.submit_ongoing_events(self._add_base_api_data(event))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing ongoing event from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_claim_prize(self, json_obj):
         """Handle 'Event_ClaimPrize' messages."""
-        event = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'event_name': json_obj['EventName'],
-        }
-        logger.info(f'Event ended: {event}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_EVENT_ENDED}', blob=event)
+        try:
+            event = {
+                'event_name': json_obj['EventName'],
+            }
+            logger.info(f'Event ended: {event}')
+            self._api_client.submit_event_ended(self._add_base_api_data(event))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing claim prize event from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_event_course(self, json_obj):
         """Handle messages linking draft id to event name."""
-        event = {
-            'player_id': self.cur_user,
-            'event_name': json_obj['InternalEventName'],
-            'time': self.cur_log_time.isoformat(),
-            'draft_id': json_obj['DraftId'],
-            'course_id': json_obj['CourseId'],
-            'card_pool': json_obj['CardPool'],
-        }
-        logger.info(f'Event course: {event}')
-        self.__retry_post(f'{self.host}/{ENDPOINT_EVENT_COURSE_SUBMISSION}', blob=event)
+        try:
+            event = {
+                'event_name': json_obj['InternalEventName'],
+                'draft_id': json_obj['DraftId'],
+                'course_id': json_obj['CourseId'],
+                'card_pool': json_obj['CardPool'],
+            }
+            logger.info(f'Event course: {event}')
+            self._api_client.submit_event_course_submission(self._add_base_api_data(event))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing partial event course from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+    def __has_pending_game_data(self):
+        return len(self.drawn_cards_by_instance_id) > 0 and len(self.game_history_events) > 5
+
+    def __enqueue_game_results(self, results):
+        try:
+            game_results = [r for r in results if r.get('scope') == 'MatchScope_Game']
+            if game_results:
+                this_game_result = game_results[-1]
+                self.pending_game_result = {
+                    'game_number': max(1, len(game_results)),
+                    'won': self.seat_id == this_game_result.get('winningTeamId'),
+                    'win_type': this_game_result.get('result'),
+                    'game_end_reason': this_game_result.get('reason'),
+                }
+                logger.info(f'Added pending game result {self.pending_game_result}')
+
+            match_result = next((r for r in results if r.get('scope') == 'MatchScope_Match'), {})
+            if match_result:
+                self.pending_match_result = {
+                    'won_match': self.seat_id == match_result.get('winningTeamId'),
+                    'match_result_type': match_result.get('result'),
+                    'match_end_reason': match_result.get('reason'),
+                }
+                logger.info(f'Added pending match result {self.pending_match_result}')
 
-    def __send_game_end(self, results):
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing game result',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+    def __enqueue_game_data(self):
         if not self.__has_pending_game_data():
-            return
+            return False
 
-        game_results = [r for r in results if r.get('scope') == 'MatchScope_Game']
-        this_game_result = game_results[-1]
-        won = self.seat_id == this_game_result.get('winningTeamId')
-        game_number = max(1, len(game_results))
-        win_type = this_game_result.get('result')
-        game_end_reason = this_game_result.get('reason')
-
-        match_result = next((r for r in results if r.get('scope') == 'MatchScope_Match'), {})
-        won_match = self.seat_id == match_result.get('winningTeamId')
-        match_result_type = match_result.get('result')
-        match_end_reason = match_result.get('reason')
-
-
-        logger.debug(f'End of game. Cards by owner: {self.objects_by_owner}')
-
-        opponent_id = 2 if self.seat_id == 1 else 1
-        opponent_card_ids = [c for c in self.objects_by_owner.get(opponent_id, {}).values()]
-
-        if self.current_match_id != self.cur_opponent_match_id:
-            self.cur_opponent_level = None
-
-        game = {
-            'player_id': self.cur_user,
-            'event_name': self.current_event_id,
-            'match_id': self.current_match_id,
-            'time': self.cur_log_time.isoformat(),
-            'game_number': game_number,
-            'on_play': self.seat_id == self.starting_team_id,
-            'won': won,
-            'win_type': win_type,
-            'game_end_reason': game_end_reason,
-            'won_match': won_match,
-            'match_result_type': match_result_type,
-            'match_end_reason': match_end_reason,
-            'opening_hand': self.opening_hand[self.seat_id],
-            'mulligans': self.drawn_hands[self.seat_id][:-1],
-            'drawn_hands': self.drawn_hands[self.seat_id],
-            'drawn_cards': list(self.drawn_cards_by_instance_id[self.seat_id].values()),
-            'mulligan_count': self.opening_hand_count_by_seat[self.seat_id] - 1,
-            'opponent_mulligan_count': self.opening_hand_count_by_seat[opponent_id] - 1,
-            'turns': self.turn_count,
-            'duration': -1,
-            'opponent_card_ids': opponent_card_ids,
-            'rank_data': self.cur_rank_data,
-            'opponent_rank': self.cur_opponent_level,
-            'maindeck_card_ids': self.current_game_maindeck,
-            'sideboard_card_ids': self.current_game_sideboard,
-            'additional_deck_info': self.current_game_additional_deck_info,
-            'service_metadata': self.game_service_metadata,
-            'client_metadata': self.game_client_metadata,
-        }
-        logger.info(f'Completed game: {game}')
+        try:
+            opponent_id = 2 if self.seat_id == 1 else 1
+            opponent_card_ids = [c for c in self.objects_by_owner.get(opponent_id, {}).values()]
 
-        # Add the history to the blob after logging to avoid printing excessive logs
-        logger.info(f'Adding game history ({len(self.game_history_events)} events)')
-        game['history'] = {
-            'seat_id': self.seat_id,
-            'opponent_seat_id': opponent_id,
-            'screen_name': self.screen_names[self.seat_id],
-            'opponent_screen_name': self.screen_names[opponent_id],
-            'events': self.game_history_events,
-        }
+            if self.current_match_id != self.cur_opponent_match_id:
+                self.cur_opponent_level = None
+
+            game = {
+                'event_name': self.current_event_id,
+                'match_id': self.current_match_id,
+                'on_play': self.seat_id == self.starting_team_id,
+                'opening_hand': self.opening_hand[self.seat_id],
+                'mulligans': self.drawn_hands[self.seat_id][:-1],
+                'drawn_hands': self.drawn_hands[self.seat_id],
+                'drawn_cards': list(self.drawn_cards_by_instance_id[self.seat_id].values()),
+                'mulligan_count': self.opening_hand_count_by_seat[self.seat_id] - 1,
+                'opponent_mulligan_count': self.opening_hand_count_by_seat[opponent_id] - 1,
+                'turns': self.turn_count,
+                'duration': -1,
+                'opponent_card_ids': opponent_card_ids,
+                'rank_data': self.cur_rank_data,
+                'opponent_rank': self.cur_opponent_level,
+                'maindeck_card_ids': self.current_game_maindeck,
+                'sideboard_card_ids': self.current_game_sideboard,
+                'additional_deck_info': self.current_game_additional_deck_info,
+                'service_metadata': self.game_service_metadata,
+                'client_metadata': self.game_client_metadata,
+            }
+            logger.info(f'Completed game: {game}')
+
+            # Add the history to the blob after logging to avoid printing excessive logs
+            logger.info(f'Adding game history ({len(self.game_history_events)} events)')
+            game['history'] = {
+                'seat_id': self.seat_id,
+                'opponent_seat_id': opponent_id,
+                'screen_name': self.screen_names[self.seat_id],
+                'opponent_screen_name': self.screen_names[opponent_id],
+                'events': self.game_history_events,
+            }
+
+            self.pending_game_submission = copy.deepcopy(game)
+            return True
 
-        self.pending_game_submission = copy.deepcopy(game)
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing game data',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+            return False
 
     def __handle_login(self, json_obj):
         """Handle 'Client.Connected' messages."""
-        self.__clear_game_data()
+        self.__clear_game_data(submit_pending_game=False)
 
-        self.cur_user = json_obj['params']['payloadObject']['playerId']
-        screen_name = json_obj['params']['payloadObject']['screenName']
-        self.__update_screen_name(screen_name)
+        try:
+            self.cur_user = json_obj['params']['payloadObject']['playerId']
+            screen_name = json_obj['params']['payloadObject']['screenName']
+            self.__update_screen_name(screen_name)
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing login from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_bot_draft_pack(self, json_obj):
         """Handle 'DraftStatus' messages."""
         if json_obj['DraftStatus'] == 'PickNext':
             self.__clear_game_data()
+
+            try:
+                self.cur_draft_event = json_obj['EventName']
+                pack = {
+                    'event_name': json_obj['EventName'],
+                    'pack_number': int(json_obj['PackNumber']),
+                    'pick_number': int(json_obj['PickNumber']),
+                    'card_ids': [int(x) for x in json_obj['DraftPack']],
+                }
+                logger.info(f'Draft pack: {pack}')
+                self._api_client.submit_draft_pack(self._add_base_api_data(pack))
+
+            except Exception as e:
+                self._log_error(
+                    message=f'Error {e} parsing draft pack from {json_obj}',
+                    error=e,
+                    stacktrace=traceback.format_exc(),
+                )
+
+    def __handle_bot_draft_pick(self, json_obj):
+        """Handle 'Draft.MakePick messages."""
+        self.__clear_game_data()
+
+        try:
             self.cur_draft_event = json_obj['EventName']
-            pack = {
-                'player_id': self.cur_user,
+            pick = {
                 'event_name': json_obj['EventName'],
-                'time': self.cur_log_time.isoformat(),
                 'pack_number': int(json_obj['PackNumber']),
                 'pick_number': int(json_obj['PickNumber']),
-                'card_ids': [int(x) for x in json_obj['DraftPack']],
+                'card_id': int(json_obj['CardId']),
             }
-            logger.info(f'Draft pack: {pack}')
-            response = self.__retry_post(f'{self.host}/{ENDPOINT_DRAFT_PACK}', blob=pack)
+            logger.info(f'Draft pick: {pick}')
+            self._api_client.submit_draft_pick(self._add_base_api_data(pick))
 
-    def __handle_bot_draft_pick(self, json_obj):
-        """Handle 'Draft.MakePick messages."""
-        self.__clear_game_data()
-        self.cur_draft_event = json_obj['EventName']
-        pick = {
-            'player_id': self.cur_user,
-            'event_name': json_obj['EventName'],
-            'time': self.cur_log_time.isoformat(),
-            'pack_number': int(json_obj['PackNumber']),
-            'pick_number': int(json_obj['PickNumber']),
-            'card_id': int(json_obj['CardId']),
-        }
-        logger.info(f'Draft pick: {pick}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_DRAFT_PICK}', blob=pick)
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing draft pick from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_joined_pod(self, json_obj):
         """Handle 'Event_Join' messages."""
         self.__clear_game_data()
-        self.cur_draft_event = json_obj['EventName']
 
-        logger.info(f'Joined draft pod: {self.cur_draft_event}')
+        try:
+            self.cur_draft_event = json_obj['EventName']
+            logger.info(f'Joined draft pod: {self.cur_draft_event}')
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing join pod event from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_human_draft_combined(self, json_obj):
         """Handle combined human draft pack/pick messages."""
         self.__clear_game_data()
-        self.cur_draft_event = json_obj['EventId']
-        pack = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'draft_id': json_obj['DraftId'],
-            'event_name': json_obj['EventId'],
-            'pack_number': int(json_obj['PackNumber']),
-            'pick_number': int(json_obj['PickNumber']),
-            'card_ids': json_obj['CardsInPack'],
-            'method': 'LogBusiness',
-        }
-        logger.info(f'Human draft pack (combined): {pack}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_HUMAN_DRAFT_PACK}', blob=pack)
-        pick = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'draft_id': json_obj['DraftId'],
-            'event_name': json_obj['EventId'],
-            'pack_number': int(json_obj['PackNumber']),
-            'pick_number': int(json_obj['PickNumber']),
-            'card_id': int(json_obj['PickGrpId']),
-            'auto_pick': json_obj['AutoPick'],
-            'time_remaining': json_obj['TimeRemainingOnPick'],
-        }
-        logger.info(f'Human draft pick (combined): {pick}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_HUMAN_DRAFT_PICK}', blob=pick)
+
+        try:
+            self.cur_draft_event = json_obj['EventId']
+            pack = {
+                'draft_id': json_obj['DraftId'],
+                'event_name': json_obj['EventId'],
+                'pack_number': int(json_obj['PackNumber']),
+                'pick_number': int(json_obj['PickNumber']),
+                'card_ids': json_obj['CardsInPack'],
+                'method': 'LogBusiness',
+            }
+            logger.info(f'Human draft pack (combined): {pack}')
+            self._api_client.submit_human_draft_pack(self._add_base_api_data(pack))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing human draft pack from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
+
+        try:
+            pick = {
+                'draft_id': json_obj['DraftId'],
+                'event_name': json_obj['EventId'],
+                'pack_number': int(json_obj['PackNumber']),
+                'pick_number': int(json_obj['PickNumber']),
+                'card_id': int(json_obj['PickGrpId']),
+                'auto_pick': json_obj['AutoPick'],
+                'time_remaining': json_obj['TimeRemainingOnPick'],
+            }
+            logger.info(f'Human draft pick (combined): {pick}')
+            self._api_client.submit_human_draft_pick(self._add_base_api_data(pick))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing human draft pick from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_human_draft_pack(self, json_obj):
         """Handle 'Draft.Notify' messages."""
         self.__clear_game_data()
-        pack = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'draft_id': json_obj['draftId'],
-            'event_name': self.cur_draft_event,
-            'pack_number': int(json_obj['SelfPack']),
-            'pick_number': int(json_obj['SelfPick']),
-            'card_ids': [int(x) for x in json_obj['PackCards'].split(',')],
-            'method': 'Draft.Notify',
-        }
-        logger.info(f'Human draft pack (Draft.Notify): {pack}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_HUMAN_DRAFT_PACK}', blob=pack)
+
+        try:
+            pack = {
+                'draft_id': json_obj['draftId'],
+                'event_name': self.cur_draft_event,
+                'pack_number': int(json_obj['SelfPack']),
+                'pick_number': int(json_obj['SelfPick']),
+                'card_ids': [int(x) for x in json_obj['PackCards'].split(',')],
+                'method': 'Draft.Notify',
+            }
+            logger.info(f'Human draft pack (Draft.Notify): {pack}')
+            self._api_client.submit_human_draft_pack(self._add_base_api_data(pack))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing human draft pack from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_deck_submission(self, json_obj):
         """Handle 'Event_SetDeck' messages."""
         self.__clear_game_data()
-        decks = json_obj['Deck']
-        deck = {
-            'player_id': self.cur_user,
-            'event_name': json_obj['EventName'],
-            'time': self.cur_log_time.isoformat(),
-            'maindeck_card_ids': [d['cardId'] for d in decks['MainDeck'] for i in range(d['quantity'])],
-            'sideboard_card_ids': [d['cardId'] for d in decks['Sideboard'] for i in range(d['quantity'])],
-            'companion': decks['Companions'][0]['cardId'] if len(decks['Companions']) > 0 else 0,
-            'is_during_match': False,
-        }
-        logger.info(f'Deck submission (Event_SetDeck): {deck}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_DECK_SUBMISSION}', blob=deck)
+
+        try:
+            decks = json_obj['Deck']
+            deck = {
+                'event_name': json_obj['EventName'],
+                'maindeck_card_ids': [d['cardId'] for d in decks['MainDeck'] for i in range(d['quantity'])],
+                'sideboard_card_ids': [d['cardId'] for d in decks['Sideboard'] for i in range(d['quantity'])],
+                'companion': decks['Companions'][0]['cardId'] if len(decks['Companions']) > 0 else 0,
+                'is_during_match': False,
+            }
+            logger.info(f'Deck submission (Event_SetDeck): {deck}')
+            self._api_client.submit_deck_submission(self._add_base_api_data(deck))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing deck submission from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_self_rank_info(self, json_obj):
         """Handle 'Rank_GetCombinedRankInfo' messages."""
-        self.cur_rank_data = json_obj
-        self.cur_user = json_obj.get('playerId', self.cur_user)
-        logger.info(f'Parsed rank info for {self.cur_user}: {self.cur_rank_data}')
-        response = self.__retry_post(f'{self.host}/{ENDPOINT_RANK}', blob={
-            'player_id':self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'rank_data': self.cur_rank_data,
-            'limited_rank': None,
-            'constructed_rank': None,
-        })
+        try:
+            self.cur_rank_data = json_obj
+            self.cur_user = json_obj.get('playerId', self.cur_user)
+            logger.info(f'Parsed rank info for {self.cur_user}: {self.cur_rank_data}')
+            data = {
+                'rank_data': self.cur_rank_data,
+                'limited_rank': None,
+                'constructed_rank': None,
+            }
+            self._api_client.submit_rank(self._add_base_api_data(data))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing self rank info from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_collection(self, json_obj):
         """Handle 'PlayerInventory.GetPlayerCardsV3' messages."""
         if self.cur_user is None:
             logger.info(f'Skipping collection submission because player id is still unknown')
             return
 
         collection = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
             'card_counts': json_obj,
         }
         logger.info(f'Collection submission of {len(json_obj)} cards')
-        self.__retry_post(f'{self.host}/{ENDPOINT_COLLECTION}', blob=collection)
+        self._api_client.submit_collection(self._add_base_api_data(collection))
 
     def __handle_inventory(self, json_obj):
         """Handle 'InventoryInfo' messages."""
-        json_obj = {k: v for k, v in json_obj.items() if k in {
-            'Gems',
-            'Gold',
-            'TotalVaultProgress',
-            'wcTrackPosition',
-            'WildCardCommons',
-            'WildCardUnCommons',
-            'WildCardRares',
-            'WildCardMythics',
-            'DraftTokens',
-            'SealedTokens',
-            'Boosters',
-            'Changes',
-        }}
-        blob = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'inventory': json_obj,
-        }
-        logger.info(f'Submitting inventory: {blob}')
-        self.__retry_post(f'{self.host}/{ENDPOINT_INVENTORY}', blob=blob)
+        try:
+            json_obj = {k: v for k, v in json_obj.items() if k in {
+                'Gems',
+                'Gold',
+                'TotalVaultProgress',
+                'wcTrackPosition',
+                'WildCardCommons',
+                'WildCardUnCommons',
+                'WildCardRares',
+                'WildCardMythics',
+                'DraftTokens',
+                'SealedTokens',
+                'Boosters',
+                'Changes',
+            }}
+            blob = {
+                'inventory': json_obj,
+            }
+            logger.info(f'Submitting inventory: {blob}')
+            self._api_client.submit_inventory(self._add_base_api_data(blob))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing inventory from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __handle_player_progress(self, json_obj):
         """Handle mastery pass messages."""
-        blob = {
-            'player_id': self.cur_user,
-            'time': self.cur_log_time.isoformat(),
-            'progress': json_obj,
-        }
-        logger.info(f'Submitting mastery progress')
-        self.__retry_post(f'{self.host}/{ENDPOINT_PLAYER_PROGRESS}', blob=blob)
+        try:
+            blob = {
+                'progress': json_obj,
+            }
+            logger.info(f'Submitting mastery progress')
+            self._api_client.submit_player_progress(self._add_base_api_data(blob))
+
+        except Exception as e:
+            self._log_error(
+                message=f'Error {e} parsing mastery progress from {json_obj}',
+                error=e,
+                stacktrace=traceback.format_exc(),
+            )
 
     def __reset_current_user(self):
         logger.info('User logged out from MTGA')
         if self.cur_user is not None:
             self.disconnected_user = self.cur_user
             self.disconnected_screen_name = self.user_screen_name
+            self.disconnected_rank = self.cur_rank_data
 
         self.cur_user = None
         self.user_screen_name = None
+        self.cur_rank_data = None
 
     def __handle_reconnect_result(self):
         logger.info('Reconnected - restoring prior user info')
 
         self.cur_user = self.disconnected_user
         self.user_screen_name = self.disconnected_screen_name
+        self.cur_rank_data = self.disconnected_rank
 
 
 def validate_uuid_v4(maybe_uuid):
     if maybe_uuid is None:
         return None
     try:
         uuid.UUID(maybe_uuid, version=4)
@@ -1075,27 +1314,19 @@
             + 'commands in the terminal, depending on your installation method:\n'
             + 'brew update && brew upgrade seventeenlands\n'
             + 'pip3 install --user --upgrade seventeenlands')
 
     show_message(title, message)
 
 def verify_version(host, prompt_if_update_required):
-    for i in range(3):
-        response = requests.get(f'{host}/{ENDPOINT_CLIENT_VERSION}', params={
-            'client': 'python',
-            'version': CLIENT_VERSION[:-2],
-        })
-
-        if not IS_CODE_FOR_RETRY(response.status_code):
-            break
-        logger.warning(f'Got response code {response.status_code}; retrying')
-        time.sleep(DEFAULT_RETRY_SLEEP_TIME)
-    else:
-        logger.warning('Could not get response from server for minimum client version. Assuming version is valid.')
-        return True
+    api_client = seventeenlands.api_client.ApiClient(host=host)
+    response = api_client.get_client_version_info(params={
+        'client': 'python',
+        'version': CLIENT_VERSION[:-2],
+    })
 
     logger.info(f'Got minimum client version response: {response.text}')
     blob = json.loads(response.text)
     this_version = [int(i) for i in CLIENT_VERSION.split('.')[:-1]]
     min_supported_version = [int(i) for i in blob['min_version'].split('.')]
     logger.info(f'Minimum supported version: {min_supported_version}; this version: {this_version}')
 
@@ -1114,15 +1345,19 @@
         filepaths = (args.log_file, )
 
     follow = not args.once
 
     follower = Follower(token, host=args.host)
 
     # if running in "normal" mode...
-    if args.log_file is None and args.host == API_ENDPOINT and follow:
+    if (
+        args.log_file is None
+        and args.host == seventeenlands.api_client.DEFAULT_HOST
+        and follow
+    ):
         # parse previous log once at startup to catch up on any missed events
         for filename in POSSIBLE_PREVIOUS_FILEPATHS:
             if os.path.exists(filename):
                 logger.info(f'Parsing the previous log {filename} once')
                 follower.parse_log(filename=filename, follow=False)
                 break
 
@@ -1143,16 +1378,16 @@
 def main():
     parser = argparse.ArgumentParser(description='MTGA log follower')
 
     config_token = get_config()
 
     parser.add_argument('-l', '--log_file',
         help=f'Log filename to process. If not specified, will try one of {POSSIBLE_CURRENT_FILEPATHS}')
-    parser.add_argument('--host', default=API_ENDPOINT,
-        help=f'Host to submit requests to. If not specified, will use {API_ENDPOINT}')
+    parser.add_argument('--host', default=seventeenlands.api_client.DEFAULT_HOST,
+        help=f'Host to submit requests to. If not specified, will use {seventeenlands.api_client.DEFAULT_HOST}')
     parser.add_argument('--token', default=config_token,
                         help=f'Token of the user. If not specified, will use the token at {CONFIG_FILE}')
     parser.add_argument('--once', action='store_true',
         help='Whether to stop after parsing the file once (default is to continue waiting for updates to the file)')
 
     args = parser.parse_args()
```

### Comparing `seventeenlands-0.1.39/seventeenlands.egg-info/PKG-INFO` & `seventeenlands-0.1.40/seventeenlands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventeenlands
-Version: 0.1.39
+Version: 0.1.40
 Summary: Utility to upload MTG Arena data to 17Lands.com
 Home-page: https://github.com/rconroy293/mtga-log-client
 Author: Robert Conroy
 Author-email: seventeenlands@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

