# Comparing `tmp/ref-man-py-0.6.4.tar.gz` & `tmp/ref-man-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ref-man-py-0.6.4.tar", max compression
+gzip compressed data, was "ref-man-py-0.7.0.tar", max compression
```

## Comparing `ref-man-py-0.6.4.tar` & `ref-man-py-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    34283 2017-09-30 07:16:25.000000 ref-man-py-0.6.4/LICENSE.md
--rw-r--r--   0        0        0     2691 2022-07-24 20:52:26.312571 ref-man-py-0.6.4/README.org
--rw-r--r--   0        0        0     1307 2023-03-23 04:15:27.924260 ref-man-py-0.6.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-23 04:15:48.733900 ref-man-py-0.6.4/ref_man_py/__init__.py
--rw-r--r--   0        0        0     4206 2023-01-17 22:27:57.904496 ref-man-py-0.6.4/ref_man_py/__main__.py
--rw-r--r--   0        0        0     3784 2022-05-09 11:56:28.414910 ref-man-py-0.6.4/ref_man_py/arxiv.py
--rw-r--r--   0        0        0    11046 2022-11-13 09:04:35.071567 ref-man-py-0.6.4/ref_man_py/cache.py
--rw-r--r--   0        0        0      669 2022-01-29 10:41:51.281358 ref-man-py-0.6.4/ref_man_py/const.py
--rw-r--r--   0        0        0     6137 2023-03-02 12:01:23.377255 ref-man-py-0.6.4/ref_man_py/data.py
--rw-r--r--   0        0        0     3776 2022-01-29 10:41:51.281358 ref-man-py-0.6.4/ref_man_py/dblp.py
--rw-r--r--   0        0        0      959 2022-01-29 10:31:10.835813 ref-man-py-0.6.4/ref_man_py/debug_ss.js
--rw-r--r--   0        0        0     7563 2022-11-13 09:09:12.704648 ref-man-py-0.6.4/ref_man_py/files_cache.py
--rw-r--r--   0        0        0     2397 2023-01-11 23:45:01.384950 ref-man-py-0.6.4/ref_man_py/filters.py
--rw-r--r--   0        0        0        0 2022-01-29 10:41:51.281358 ref-man-py-0.6.4/ref_man_py/py.typed
--rw-r--r--   0        0        0     1803 2022-01-29 10:41:51.281358 ref-man-py-0.6.4/ref_man_py/q_helper.py
--rw-r--r--   0        0        0    44460 2023-02-09 21:26:36.683363 ref-man-py-0.6.4/ref_man_py/semantic_scholar.py
--rw-r--r--   0        0        0     6952 2022-08-31 20:21:13.910949 ref-man-py-0.6.4/ref_man_py/semantic_search.py
--rw-r--r--   0        0        0    35184 2023-03-23 04:06:24.261677 ref-man-py-0.6.4/ref_man_py/service.py
--rw-r--r--   0        0        0      452 2022-12-27 02:24:05.070490 ref-man-py-0.6.4/ref_man_py/ss_default.json
--rw-r--r--   0        0        0      532 2022-12-27 02:22:41.303899 ref-man-py-0.6.4/ref_man_py/ss_default.json.bak.2
--rw-r--r--   0        0        0     6727 2023-03-02 13:12:15.488631 ref-man-py-0.6.4/ref_man_py/util.py
--rw-r--r--   0        0        0     3912 2023-03-23 04:18:06.884451 ref-man-py-0.6.4/setup.py
--rw-r--r--   0        0        0     4050 2023-03-23 04:18:06.884810 ref-man-py-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    34283 2017-09-30 07:16:25.000000 ref-man-py-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     2691 2022-07-24 20:52:26.312571 ref-man-py-0.7.0/README.org
+-rw-r--r--   0        0        0     1361 2023-07-11 06:50:16.117741 ref-man-py-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-11 06:50:40.192329 ref-man-py-0.7.0/ref_man_py/__init__.py
+-rw-r--r--   0        0        0     4621 2023-07-11 06:23:01.977746 ref-man-py-0.7.0/ref_man_py/__main__.py
+-rw-r--r--   0        0        0     3784 2022-05-09 11:56:28.414910 ref-man-py-0.7.0/ref_man_py/arxiv.py
+-rw-r--r--   0        0        0    11046 2022-11-13 09:04:35.071567 ref-man-py-0.7.0/ref_man_py/cache.py
+-rw-r--r--   0        0        0      669 2022-01-29 10:41:51.281358 ref-man-py-0.7.0/ref_man_py/const.py
+-rw-r--r--   0        0        0    11138 2023-07-05 08:26:32.355658 ref-man-py-0.7.0/ref_man_py/cvf.py
+-rw-r--r--   0        0        0     6137 2023-03-02 12:01:23.377255 ref-man-py-0.7.0/ref_man_py/data.py
+-rw-r--r--   0        0        0     3776 2022-01-29 10:41:51.281358 ref-man-py-0.7.0/ref_man_py/dblp.py
+-rw-r--r--   0        0        0      959 2022-01-29 10:31:10.835813 ref-man-py-0.7.0/ref_man_py/debug_ss.js
+-rw-r--r--   0        0        0     7563 2022-11-13 09:09:12.704648 ref-man-py-0.7.0/ref_man_py/files_cache.py
+-rw-r--r--   0        0        0     2397 2023-01-11 23:45:01.384950 ref-man-py-0.7.0/ref_man_py/filters.py
+-rw-r--r--   0        0        0      206 2023-07-11 06:55:26.518422 ref-man-py-0.7.0/ref_man_py/headers_default.json
+-rw-r--r--   0        0        0      707 2023-07-11 07:19:57.983205 ref-man-py-0.7.0/ref_man_py/log.py
+-rw-r--r--   0        0        0        0 2022-01-29 10:41:51.281358 ref-man-py-0.7.0/ref_man_py/py.typed
+-rw-r--r--   0        0        0     1803 2022-01-29 10:41:51.281358 ref-man-py-0.7.0/ref_man_py/q_helper.py
+-rw-r--r--   0        0        0    44681 2023-07-11 07:14:35.074739 ref-man-py-0.7.0/ref_man_py/semantic_scholar.py
+-rw-r--r--   0        0        0     7357 2023-07-11 02:29:29.884875 ref-man-py-0.7.0/ref_man_py/semantic_search.py
+-rw-r--r--   0        0        0    28888 2023-07-11 07:14:12.720122 ref-man-py-0.7.0/ref_man_py/service.py
+-rw-r--r--   0        0        0      394 2023-07-11 07:21:40.680445 ref-man-py-0.7.0/ref_man_py/ss_default.json
+-rw-r--r--   0        0        0     6727 2023-03-02 13:12:15.488631 ref-man-py-0.7.0/ref_man_py/util.py
+-rw-r--r--   0        0        0     3934 2023-07-11 07:29:30.734062 ref-man-py-0.7.0/setup.py
+-rw-r--r--   0        0        0     4086 2023-07-11 07:29:30.734423 ref-man-py-0.7.0/PKG-INFO
```

### Comparing `ref-man-py-0.6.4/LICENSE.md` & `ref-man-py-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/README.org` & `ref-man-py-0.7.0/README.org`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/pyproject.toml` & `ref-man-py-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ref-man-py"
-version = "0.6.4"
+version = "0.7.0"
 description = "Ref Man Python Module"
 authors = ["Akshay <akshay.badola.cs@gmail.com>"]
 license = "AGPL-3"
 readme = "README.org"
 homepage = "https://github.com/akshaybadola/ref-man-py"
 classifiers=[
     "Development Status :: 3 - Alpha",
@@ -16,25 +16,27 @@
     "Programming Language :: Python :: 3.11",
     "Natural Language :: English",
     "Topic :: Education",
     "Topic :: Scientific/Engineering",
     "Topic :: Text Editors :: Emacs",
 ]
 keywords = ['emacs', 'semanticscholar', 'bibliography', 'ref-man']
+exclude = ["ref_man_py/*.bak.*"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.26.0"
 flask = "^1.1.2"
 beautifulsoup4 = "^4.9.1"
 psutil = "^5.8.0"
 PyYAML = "^5.4.1"
 lxml = "^4.6.4"
 common_pyutil = "^0.8.5"
 aiohttp = "^3.8.1"
+MarkupSafe = "2.0.1"
 typing-extensions = {version = "*", python = "3.7.x"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 poetry = "^1.1.8"
 toml = "^0.10.2"
 pytest-cov = "^3.0.0"
```

### Comparing `ref-man-py-0.6.4/ref_man_py/__main__.py` & `ref-man-py-0.7.0/ref_man_py/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,38 +42,48 @@
     parser.add_argument("--batch-size", "-b", dest="batch_size", type=int, default=16,
                         help="Simultaneous connections to DBLP")
     parser.add_argument("--chrome-debugger-path", dest="chrome_debugger_path", type=Path,
                         default="",
                         help="Path to chrome debugger script which can validate " +
                         "Semantic Scholar Search params (optional)")
     parser.add_argument("--debug", action="store_true", help="Run in debug mode")
+    parser.add_argument("--logfile", help="Logfile for logging")
+    parser.add_argument("--logdir", type=Path, help="Directory where logfile will be stored")
+    parser.add_argument("--logfile-verbosity", type=str, default="debug",
+                        choices=["error", "info", "debug"],
+                        help="Verbosity level for logfile if given")
     parser.add_argument("--verbosity", "-v", type=str, default="info",
-                        choices=["error", "info", "debug"], help="Verbosity level")
+                        choices=["error", "info", "debug"], help="Verbosity level for stdout")
     parser.add_argument("--version", action="store_true",
                         help="Print version and exit.")
     args = parser.parse_args()
     if args.version:
         print(f"ref-man-server version {__version__}")
         sys.exit(0)
     from .service import RefMan
-    kwargs = {"host": args.host,
-              "port": args.port,
-              "proxy_port": args.proxy_port,
-              "proxy_everything": args.proxy_everything,
-              "proxy_everything_port": args.proxy_everything_port,
-              "data_dir": args.data_dir,
-              "refs_cache_dir": args.refs_cache_dir,
-              "config_dir": Path(args.config_dir),
-              "local_pdfs_dir": args.local_pdfs_dir,
-              "remote_pdfs_dir": args.remote_pdfs_dir,
-              "remote_links_cache": args.remote_links_cache,
-              "batch_size": args.batch_size,
-              "chrome_debugger_path": args.chrome_debugger_path,
-              "debug": args.debug,
-              "verbosity": args.verbosity,
-              "threaded": args.threaded}
+    kwargs = {
+        "host": args.host,
+        "port": args.port,
+        "proxy_port": args.proxy_port,
+        "proxy_everything": args.proxy_everything,
+        "proxy_everything_port": args.proxy_everything_port,
+        "data_dir": args.data_dir,
+        "refs_cache_dir": args.refs_cache_dir,
+        "config_dir": Path(args.config_dir),
+        "local_pdfs_dir": args.local_pdfs_dir,
+        "remote_pdfs_dir": args.remote_pdfs_dir,
+        "remote_links_cache": args.remote_links_cache,
+        "batch_size": args.batch_size,
+        "chrome_debugger_path": args.chrome_debugger_path,
+        "debug": args.debug,
+        "logdir": args.logdir,
+        "logfile": args.logfile,
+        "logfile_verbosity": args.logfile_verbosity,
+        "verbosity": args.verbosity,
+        "threaded": args.threaded,
+    }
     service = RefMan(**kwargs)
     service.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ref-man-py-0.6.4/ref_man_py/arxiv.py` & `ref-man-py-0.7.0/ref_man_py/arxiv.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/cache.py` & `ref-man-py-0.7.0/ref_man_py/cache.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/const.py` & `ref-man-py-0.7.0/ref_man_py/const.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/data.py` & `ref-man-py-0.7.0/ref_man_py/data.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/dblp.py` & `ref-man-py-0.7.0/ref_man_py/dblp.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/debug_ss.js` & `ref-man-py-0.7.0/ref_man_py/debug_ss.js`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/files_cache.py` & `ref-man-py-0.7.0/ref_man_py/files_cache.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/filters.py` & `ref-man-py-0.7.0/ref_man_py/filters.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/q_helper.py` & `ref-man-py-0.7.0/ref_man_py/q_helper.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/ref_man_py/semantic_scholar.py` & `ref-man-py-0.7.0/ref_man_py/semantic_scholar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import List, Dict, Optional, Union, Tuple, Any, Callable, cast
 import os
 import json
 import math
 import time
 import random
-import requests
+import logging
 from pathlib import Path
 import asyncio
+
 import sys
 if sys.version_info.minor > 7:
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+import requests
 import aiohttp
 from common_pyutil.monitor import Timer
 
 from .filters import (year_filter, author_filter, num_citing_filter,
                       num_influential_count_filter, venue_filter, title_filter)
 from .data import CitationsCache
+from .log import info, debug, warn, error
 
 
 timer = Timer()
 
 
 class SubConfigType(TypedDict):
     limit: int
@@ -124,14 +127,15 @@
                                          "influentialcitationcount": num_influential_count_filter,
                                          "venue": venue_filter,
                                          "title": title_filter}
         return _filters
 
     def __init__(self, config_file=None, cache_dir=None, refs_cache_dir=None):
         self.load_config(config_file)
+        self.logger = logging.getLogger("ref-man")
         self._api_key = self._config.get("api_key", None)
         self._root_url = "https://api.semanticscholar.org/graph/v1"
         self._cache_dir = Path(cache_dir or self._config.get("cache", None))
         if not self._cache_dir or not Path(self._cache_dir).exists():
             raise FileExistsError(f"{self._cache_dir} doesn't exist")
         self._refs_cache_dir = refs_cache_dir
         self._in_memory: Dict[str, StoredDataType] = {}
@@ -539,15 +543,15 @@
                 print(f"Force fetching from Semantic Scholar for {ID}")
                 return self.store_details_and_get(ID, no_transform)
         else:
             print(f"Fetching from Semantic Scholar for {ID}")
             return self.store_details_and_get(ID, no_transform)
 
     # TODO: Don't we expect the other data to be in cache?
-    def _corpus_id(self, id_type: str, ID: str) -> Union[str, int]:
+    def id_to_corpus_id(self, id_type: str, ID: str) -> Union[str, int]:
         ids = {"doi": f"DOI:{ID}",
                "mag": f"MAG:{ID}",
                "arxiv": f"ARXIV:{ID}",
                "acl": f"ACL:{ID}",
                "pubmed": f"PMID:{ID}",
                "url": f"URL:{ID}"}
         if id_type == "ss":
@@ -1080,11 +1084,13 @@
 
         """
         terms = "+".join(query.split(" "))
         fields = ",".join(self._config["search"]["fields"])
         limit = self._config["search"]["limit"]
         url = f"{self._root_url}/paper/search?query={terms}&fields={fields}&limit={limit}"
         response = self._get(url)
+        debug(f"Searching for {query}")
         if response.status_code == 200:
-            return response.content
+            debug(f"Got some results for {query}")
+            return response.content  # type: ignore
         else:
             return json.dumps({"error": json.loads(response.content)})
```

### Comparing `ref-man-py-0.6.4/ref_man_py/semantic_search.py` & `ref-man-py-0.7.0/ref_man_py/semantic_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import List, Dict, Union, Optional
 from pathlib import Path
+from urllib import parse
 import json
 from subprocess import Popen, PIPE
 import shlex
 
 import requests
 
 
 class SemanticSearch:
     # Example params:
     #
     # {'queryString': '', 'page': 1, 'pageSize': 10, 'sort': 'relevance',
-    #  'authors': [], 'coAuthors': [], 'venues': [], 'yearFilter': None,
+    #  'authors': [], 'coAuthors': [], 'venues': [], 'year_filter': None,
     #  'requireViewablePdf': False, 'publicationTypes': [], 'externalContentTypes': [],
     #  'fieldsOfStudy': ['computer-science'], 'useFallbackRankerService': False,
     #  'useFallbackSearchCluster': False, 'hydrateWithDdb': True, 'includeTldrs': False,
     #  'performTitleMatch': True, 'includeBadges': False, 'tldrModelVersion': 'v2.0.0',
     #  'getQuerySuggestions': False}
 
     """Semantic Scholar Search Module
@@ -25,19 +26,24 @@
     Args:
         debugger_path: Optional path to a JS debugger file.
                        Used for getting the arguments from Semantic Scholar Search
                        API from a chrome debugger websocket.
     """
     def __init__(self, debugger_path: Optional[Path]):
         self.params_file = Path(__file__).parent.joinpath("ss_default.json")
+        self.headers_file = Path(__file__).parent.joinpath("headers_default.json")
         with open(self.params_file) as f:
             self.default_params = json.load(f)
         self.params = self.default_params.copy()
         if debugger_path and debugger_path.exists():
             self.update_params(debugger_path)
+        with open(self.headers_file) as f:
+            self.headers = json.load(f)
+        self.root_url = "https://www.semanticscholar.org/"
+        self.search_url = parse.urljoin(self.root_url, "api/1/search")
 
     def update_params(self, debugger_path: Path) -> None:
         """Update the parameters for Semantic Scholar Search if possible
 
         Args:
             debugger_path: Optional path to a JS debugger file.
 
@@ -115,31 +121,33 @@
         :code:`publicationTypes` in :code:`kwargs` can be ["Conference", "JournalArticle"]
         :code:`yearFilter` has to be a :class:`dict` of type {"max": 1995, "min": 1990}
 
         """
         params = self.params.copy()
         params["queryString"] = query
         if 'yearFilter' in kwargs:
-            yearFilter = kwargs['yearFilter']
-            if yearFilter and not ("min" in yearFilter and "max" in yearFilter and
-                                   yearFilter["max"] > yearFilter["min"]):
+            year_filter = kwargs['yearFilter']
+            if year_filter and not ("min" in year_filter and "max" in year_filter and
+                                    year_filter["max"] > year_filter["min"]):
                 print("Invalid Year Filter. Disabling.")
-                yearFilter = None
-            params['yearFilter'] = yearFilter
+                year_filter = None
+            params['yearFilter'] = year_filter
         if cs_only:
             params['fieldsOfStudy'] = ['computer-science']
         else:
             params['fieldsOfStudy'] = []
         for k, v in kwargs.items():
             if k in params and isinstance(v, type(params[k])):
                 params[k] = v
-        headers = {'User-agent': 'Mozilla/5.0', 'Origin': 'https://www.semanticscholar.org'}
-        print("Sending request to semanticscholar search with query" +
-              f": {query} and params {self.params}")
+        headers = {"referer": f"{self.root_url}/search?q={parse.quote(query)}&sort=relevance",
+                   **self.headers}
+        print(f"Sending request to semanticscholar search with query: {query},"
+              f" params {params}, headers {headers}")
         response = requests.post("https://www.semanticscholar.org/api/1/search",
                                  headers=headers, json=params)
         if response.status_code == 200:
             results = json.loads(response.content)["results"]
             print(f"Got {len(results)} results for query: {query}")
-            return response.content  # already json
+            # already json
+            return response.content  # type: ignore
         else:
             return json.dumps({"error": f"ERROR for {query}, {str(response.content)}"})
```

### Comparing `ref-man-py-0.6.4/ref_man_py/service.py` & `ref-man-py-0.7.0/ref_man_py/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from typing import List, Dict, Optional, Tuple, Union
 import json
-import operator
 import os
-import re
 import time
 from pathlib import Path
 from threading import Thread
 from multiprocessing import Process
 
 import yaml
 import requests
 import psutil
 from flask import Flask, request, Response
 from werkzeug import serving
 
-import bs4
-from bs4 import BeautifulSoup
-
-from common_pyutil.log import get_stream_logger
+from common_pyutil.log import get_file_and_stream_logger, get_stream_logger
 
 from . import __version__
 from .const import default_headers
 from .util import (fetch_url_info, fetch_url_info_parallel,
                    parallel_fetch, post_json_wrapper, check_proxy_port)
 from .arxiv import arxiv_get, arxiv_fetch, arxiv_helper
 from .dblp import dblp_helper
+from .cvf import CVF
 from .semantic_scholar import SemanticScholar
 from .semantic_search import SemanticSearch
 from .cache import CacheHelper
 
 
 app = Flask("RefMan")
 
@@ -57,30 +53,33 @@
                     implemented for that method.
         chrome_debugger_path: Path for the chrome debugger script.
                               Used to validate the Semantic Scholar search api, as
                               the params can change sometimes. If it's not given then
                               default params are used and the user must update the params
                               in case of an error.
         debug: Whether to start the service in debug mode
-        verbosity: Verbosity control
+        logfile: Optional log file for logging
+        logfile_verbosity: logfile verbosity level
+        verbosity: stdiout verbosity level
         threaded: Start the flask server in threaded mode. Defaults to :code:`True`.
 
     :code:`remote_pdfs_dir` has to be an :code:`rclone` path and the pdf files from
     :code:`local_pdfs_dir` is synced to that with :code:`rclone`.
 
     """
     # TODO: Generate default config and place in config dir.
     #       As of now only SemanticScholar configuration is loaded if it exists
     # TODO: Also allow the user to add config options like request headers,
     #       proxy ports, data_dir etc.
-    def __init__(self, host: str, port: int, proxy_port: int, proxy_everything: bool,
+    def __init__(self, *, host: str, port: int, proxy_port: int, proxy_everything: bool,
                  proxy_everything_port: int, data_dir: Path, refs_cache_dir: Path,
                  config_dir: Path, local_pdfs_dir: Path,
                  remote_pdfs_dir: Path, remote_links_cache: Path,
                  batch_size: int, chrome_debugger_path: Path,
+                 logfile: str, logdir: Path, logfile_verbosity: str,
                  debug: bool, verbosity: str, threaded: bool):
         self.host = host
         self.port = port
         self.batch_size = batch_size
         self.data_dir = data_dir
         self.config_dir = config_dir
         self.refs_cache_dir = refs_cache_dir
@@ -92,48 +91,45 @@
         self.proxy_everything_port = proxy_everything_port
         self.chrome_debugger_path = Path(chrome_debugger_path) if chrome_debugger_path else None
         if not self.config_dir.exists():
             os.makedirs(self.config_dir)
         self.config_file: Optional[Path] = self.config_dir.joinpath("config.json")
         self.config_file = self.config_file if self.config_file.exists() else None
         self.debug = debug
+
+        self.logfile = logfile
+        self.logdir = logdir
+        self.logfile_verbosity = logfile_verbosity
         self.verbosity = verbosity
         self.threaded = threaded
 
-        self._requests_timeout = 5
-        self._requests_fetch_url_timeout = 60
+        self._requests_timeout = 60
 
         self.init_loggers()
         if self.config_file:
             self.logi(f"Loaded config file {self.config_file}")
 
-        self.cvf_url_root = "https://openaccess.thecvf.com"
-        self.soups: Dict[Tuple, bs4.Tag] = {}
-        self.cvf_pdf_links: Dict[Tuple, List[str]] = {}
-        # self.load_cvf_files()
-        self.load_cvf_pdf_links()
         self.s2 = SemanticScholar(config_file=self.config_file, cache_dir=self.data_dir,
                                   refs_cache_dir=self.refs_cache_dir)
         self.init_remote_cache()
 
+        self.cvf_helper = CVF(self.config_dir, self.logger)
+
         # NOTE: Checks only once for the proxy, see util.check_proxy
         #       for a persistent solution
         self.check_proxies()
         # NOTE: Although this is still use here, SS may phase it out
         #       in favour of the graph/search
         self.semantic_search = SemanticSearch(self.chrome_debugger_path)
         self._app = app
         self.init_routes()
 
     def _get(self, url: str, **kwargs) -> requests.Response:
         return requests.get(url, timeout=self._requests_timeout, **kwargs)
 
-    def _get_url(self, url: str, **kwargs) -> requests.Response:
-        return requests.get(url, timeout=self._requests_fetch_url_timeout, **kwargs)
-
     def init_remote_cache(self):
         """Initialize cache (and map) of remote and local pdf files.
 
         The files can be synced from and to an :code:`rclone` remote.
 
         """
         self.update_cache_run = None
@@ -143,159 +139,33 @@
                             Path(self.remote_links_cache), self.logger)
         else:
             self.pdf_cache_helper = None
             self.logger.warning("All arguments required for pdf cache not given.\n"
                                 "Will not maintain remote pdf links cache.")
 
     def init_loggers(self):
-        # We set "error" to warning
         verbosity_levels = {"info", "error", "debug"}
-        if self.verbosity not in verbosity_levels:
-            self.verbosity = "info"
-            self.logger = get_stream_logger("ref_man_logger", log_level=self.verbosity)
-            self.logger.warning(f"{self.verbosity} was not in known levels. " +
-                                f"Set to {self.verbosity}")
+        self.verbosity = (self.verbosity in verbosity_levels and self.verbosity) or "info"
+        self.logfile_verbosity = (self.logfile_verbosity in verbosity_levels and
+                                  self.logfile_verbosity) or "debug"
+        if self.logdir and self.logfile:
+            _, self.logger = get_file_and_stream_logger(logger_name="ref-man",
+                                                        logdir=str(self.logdir.absolute()),
+                                                        log_file_name=self.logfile,
+                                                        new_file=False,
+                                                        file_log_level=self.logfile_verbosity,
+                                                        stream_log_level=self.verbosity,
+                                                        logger_level="debug")
+            self.logger.info(f"Log file is {self.logdir}/{self.logfile}")
+            self.logger.debug(f"File log level is set to {self.logfile_verbosity}")
+            self.logger.debug(f"Stream log level is set to {self.verbosity}")
         else:
-            self.logger = get_stream_logger("ref_man_logger", log_level=self.verbosity)
+            self.logger = get_stream_logger("ref-man", log_level=self.verbosity)
             self.logger.debug(f"Log level is set to {self.verbosity}.")
 
-    def load_cvf_files(self):
-        """Load the CVF Soups from HTML files.
-
-        XML parses via :class:`BeautifulSoup` are maintained for easy
-        fetching of an article in case it's availble.
-
-        """
-        self.cvf_files = [os.path.join(self.config_dir, f)
-                          for f in os.listdir(self.config_dir)
-                          if re.match(r'^(cvpr|iccv)', f.lower())
-                          and not f.endswith("_pdfs")]
-        self.logger.debug("Loading CVF soups.")
-        for cvf in self.cvf_files:
-            if not cvf.endswith("_pdfs"):
-                match = re.match(r'^(cvpr|iccv)(.*?)([0-9]+)',
-                                 Path(cvf).name, flags=re.IGNORECASE)
-                if match:
-                    venue, _, year = map(str.lower, match.groups())
-                    with open(cvf) as f:
-                        self.soups[(venue, year)] = BeautifulSoup(f.read(), features="lxml")
-                else:
-                    self.logger.error(f"Could not load file {cvf}")
-        self.logger.debug(f"Loaded conference files {self.soups.keys()}")
-
-    def load_cvf_pdf_links(self):
-        """Load the CVF PDF links saved from HTML files.
-
-        """
-        self.cvf_pdf_link_files = [os.path.join(self.config_dir, f)
-                                   for f in os.listdir(self.config_dir)
-                                   if re.match(r'^(cvpr|iccv)', f.lower())
-                                   and f.endswith("_pdfs")]
-        self.logger.debug("Loading CVF pdf links.")
-        for fname in self.cvf_pdf_link_files:
-            match = re.match(r'^(cvpr|iccv)(.*?)([0-9]+)',
-                             Path(fname).name, flags=re.IGNORECASE)
-            if match:
-                venue, _, year = map(str.lower, match.groups())
-                with open(fname) as f:
-                    self.cvf_pdf_links[(venue, year)] = f.read().split("\n")
-            else:
-                self.logger.error(f"Could not load pdf links from {fname}")
-        self.logger.debug(f"Loaded PDF links {self.cvf_pdf_links.keys()}")
-
-    def maybe_download_cvf_day_pages(self, response, venue, year):
-        soup = BeautifulSoup(response.content, features="lxml")
-        links = soup.find_all("a")
-        regexp = f"(/)?({venue.upper()}{year}(.py)?).+"
-        last_link_attrs = links[-1].attrs
-        venue_match = re.match(regexp, last_link_attrs['href'])
-        venue_group = venue_match and venue_match.group(2)
-        if "href" in last_link_attrs and venue_group:
-            day_links = [*filter(lambda x: re.match(r"Day [0-9]+?: ([0-9-+])", x.text),
-                                 soup.find_all("a"))]
-            content = []
-            for i, dl in enumerate(day_links):
-                day = re.match(r"Day [0-9]+?: ([0-9-]+)", dl.text).groups()[0]
-                d_url = f"{self.cvf_url_root}/{venue_group}?day={day}"
-                resp = self._get(d_url)
-                if not resp.ok:
-                    err = f"Status code {response.status_code} for {d_url}"
-                    raise requests.HTTPError(err)
-                content.append(resp.content)
-                self.logd(f"Fetched page {i+1} for {venue.upper()}{year} and {day}")
-            soup_content = BeautifulSoup("")
-            for c in content:
-                soup_content.extend(BeautifulSoup(c, features="lxml").html)
-            return soup_content.decode()
-        self.logd(f"Fetched page for {venue.upper()}{year}")
-        return response.content.decode()
-
-    def download_cvf_page_and_update_soups(self, venue, year):
-        url = f"{self.cvf_url_root}/{venue.upper()}{year}"
-        response = self._get(url)
-        if response.ok:
-            content = self.maybe_download_cvf_day_pages(response, venue, year)
-        else:
-            err = f"Status code {response.status_code} for {url}"
-            raise requests.HTTPError(err)
-        fname = self.config_dir.joinpath(f"{venue.upper()}{year}")
-        with open(fname, "w") as f:
-            f.write(content)
-        with open(fname) as f:
-            self.soups[(venue.lower(), year)] = BeautifulSoup(content, features="lxml")
-
-    def return_link_subr(self, title, matches) -> str:
-        if not matches:
-            return f"URL Not found for {title}"
-        elif len(matches) == 1:
-            href = matches[0].group(0)
-        else:
-            matches.sort(key=lambda x: operator.abs(operator.sub(*x.span())))
-            href = matches[-1].group(0)
-        href = "https://openaccess.thecvf.com/" + href.lstrip("/")
-        return f"{title};{href}"
-
-    def find_link_from_soups(self, keys, title) -> Optional[str]:
-        links = []
-        for k in keys:
-            links.extend(self.soups[k].find_all("a"))
-        if links:
-            regexp = ".*" + ".*".join([*filter(None, title.split(" "))][:3]) + ".*\\.pdf$"
-            matches = [*filter(None, map(lambda x: re.match(regexp, x["href"], flags=re.IGNORECASE)
-                                         if "href" in x.attrs else None, links))]
-            return self.return_link_subr(title, matches)
-        else:
-            return None
-
-    def find_pdf_link(self, keys, title) -> Optional[str]:
-        links = []
-        for k in keys:
-            links.extend(self.cvf_pdf_links[k])
-        if links:
-            regexp = ".*" + ".*".join([*filter(None, title.split(" "))][:3]) + ".*\\.pdf$"
-            matches = [*filter(None, map(lambda x: re.match(regexp, x, flags=re.IGNORECASE), links))]
-            return self.return_link_subr(title, matches)
-        else:
-            return None
-
-    def save_cvf_pdf_links_and_update(self, venue: str, year: str, soup) -> None:
-        links = soup.find_all("a")
-        pdf_links = [x["href"] for x in links
-                     if "href" in x.attrs and x["href"].endswith(".pdf")]
-        fname = self.config_dir.joinpath(f"{venue.upper()}{year}_pdfs")
-        with open(fname, "w") as f:
-            f.write("\n".join(pdf_links))
-        self.cvf_pdf_links[(venue, year)] = pdf_links
-
-    def read_cvf_pdf_links(self, venue: str, year: str) -> List[str]:
-        fname = self.config_dir.joinpath(f"{venue.upper()}{year}_pdfs")
-        with open(fname) as f:
-            pdf_links = f.read().split("\n")
-        return pdf_links
-
     def logi(self, msg: str) -> str:
         self.logger.info(msg)
         return msg
 
     def logd(self, msg: str) -> str:
         self.logger.debug(msg)
         return msg
@@ -381,15 +251,15 @@
                 id = request.args["id"]
             else:
                 return json.dumps("NO ID GIVEN")
             if "id_type" in request.args:
                 id_type = request.args["id_type"]
             else:
                 return json.dumps("NO ID_TYPE GIVEN")
-            data = self.s2.get_corpus_id(id_type, id)
+            data = self.s2.id_to_corpus_id(id_type, id)
             return json.dumps(data)
 
         @app.route("/s2_config", methods=["GET"])
         def s2_config():
             return json.dumps(self.s2._config)
 
         @app.route("/s2_details/<ssid>", methods=["GET"])
@@ -616,27 +486,27 @@
             #         pdf_data = f.read()
             #     response = make_response(pdf_data)
             #     response.headers["Content-Type"] = "application/pdf"
             #     return response
             self.logger.debug(f"Fetching {url} with proxies {self.proxies}")
             if not noproxy and self.proxies:
                 try:
-                    response = self._get_url(url, headers=default_headers, proxies=self.proxies)
+                    response = self._get(url, headers=default_headers, proxies=self.proxies)
                 except requests.exceptions.Timeout:
                     self.logger.error("Proxy not reachable. Fetching without proxy")
                     self.proxies = None
-                    response = self._get_url(url, headers=default_headers)
+                    response = self._get(url, headers=default_headers)
                 except requests.exceptions.ProxyError:
                     self.logger.error("Proxy not reachable. Fetching without proxy")
                     self.proxies = None
-                    response = self._get_url(url, headers=default_headers)
+                    response = self._get(url, headers=default_headers)
             else:
                 if not noproxy:
                     self.logger.warning("Proxy dead. Fetching without proxy")
-                response = self._get_url(url, headers=default_headers)
+                response = self._get(url, headers=default_headers)
             if url.startswith("http:") or response.url.startswith("https:"):
                 return Response(response.content)
             elif response.url != url:
                 if response.headers["Content-Type"] in\
                    {"application/pdf", "application/octet-stream"}:
                     return Response(response.content)
                 elif response.headers["Content-Type"].startswith("text"):
@@ -713,26 +583,15 @@
             else:
                 title = request.args["title"]
             if "venue" not in request.args:
                 return self.loge("Error. Venue not in request")
             else:
                 venue = request.args["venue"].lower()
             year = request.args.get("year")
-            if year:
-                keys = [(v, y) for v, y in self.cvf_pdf_links if v == venue and y == year]
-            else:
-                keys = [(v, y) for v, y in self.cvf_pdf_links if v == venue]
-                year = ",".join([y for v, y in self.soups if v == venue])
-            if not keys and year:
-                self.logd(f"Fetching page(s) for {venue.upper()}{year}")
-                self.download_cvf_page_and_update_soups(venue, year)
-                self.save_cvf_pdf_links_and_update(venue, year, self.soups[(venue, year)])
-                keys = [(v, y) for v, y in self.soups if v == venue and y == year]
-            # maybe_link = self.find_soup(keys, title)
-            maybe_link = self.find_pdf_link(keys, title)
+            maybe_link = self.cvf_helper.get_pdf_link(title, venue, year)
             if maybe_link:
                 return maybe_link
             else:
                 return f"{title} not found for {venue} in {year}"
 
         @app.route("/echo", methods=["GET"])
         def echo():
```

### Comparing `ref-man-py-0.6.4/ref_man_py/util.py` & `ref-man-py-0.7.0/ref_man_py/util.py`

 * *Files identical despite different names*

### Comparing `ref-man-py-0.6.4/setup.py` & `ref-man-py-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 packages = \
 ['ref_man_py']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
+['MarkupSafe==2.0.1',
+ 'PyYAML>=5.4.1,<6.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'beautifulsoup4>=4.9.1,<5.0.0',
  'common_pyutil>=0.8.5,<0.9.0',
  'flask>=1.1.2,<2.0.0',
  'lxml>=4.6.4,<5.0.0',
  'psutil>=5.8.0,<6.0.0',
  'requests>=2.26.0,<3.0.0']
@@ -22,15 +23,15 @@
 
 entry_points = \
 {'console_scripts': ['ref_man = ref_man_py.__main__:main',
                      'test = pytest:main']}
 
 setup_kwargs = {
     'name': 'ref-man-py',
-    'version': '0.6.4',
+    'version': '0.7.0',
     'description': 'Ref Man Python Module',
     'long_description': "* ref-man-py\n\n  Python Module for ~ref-man~ (See https://github.com/akshaybadola/ref-man).\n\n  Network requests and xml parsing can be annoying in emacs, so ref-man uses a\n  separate python process for efficient (and sometimes parallel) fetching of\n  network requests.\n\n* Features\n\n** Persistent Service with Flask\n   - Can easily integrate with other applications\n   - Parallel fetching of large number of entries from supported websites\n     (DBLP, ArXiv etc.)\n\n** HTTP integration with Semantic Scholar API (https://www.semanticscholar.org/product/api)\n   - Fetch with multiple IDs like arxiv, ACL etc.\n   - Local files based cache to avoid redundant requests\n   - +Fetches all metadata in one go (Will change soon as Semantic Scholar is\n     updating its API)+\n   - Now uses the Semantic Scholar Graph API\n\n** Experimental (and undocumented) Semantic Scholar Search API\n   - Mostly gleaned through analyzing network requests. Helpful for searching\n     articles.\n\n** HTTP integration with DBLP and ArXiv\n   - Supports multiple parallel requests for batch updates\n\n** Fetch PDF from a given URL\n   - Easier to fetch using python than with Emacs's callbacks\n\n** Option for proxying requests\n   - Particularly useful for PDFs if you're tunneling to your institution from\n     home or some other location and the article you want is with institutional\n     (IP based) access only.\n\n* Roadmap\n\n** More Tests\n   - Coverage is low.\n   - Need to remove some code which isn't used.\n   - Some parts need to be rewritten.\n\n** Change to new Semantic Scholar API (*Done*)\n   Semantic Scholar is changing its API. See https://www.semanticscholar.org/product/api\n   we should migrate to new ~graph/v1/paper~ API.\n\n** Integrate ~common_pyutil.net.Get~\n   It has support for progress tracking. Helpful when network is slow and when\n   downloading large files.\n\n** ASGI server\n   With websockets for better Async integration.\n\n** Integrate more services\n   There're semi-working/broken functions for CrossRef and some other services in\n   ~ref-man~. They can be exported to python perhaps.\n\n* Wishlist\n\n** Serve Org files on the fly as html\n   Will help in integrating a larger userbase. Perhaps also with a py-to-lisp\n   (hy like maybe) interface so that elementary scripting on the org backend can\n   be done.\n\n** Ultimately integrate ~pndconf~ also\n   A document preparation toolchain (See https://github.com/akshaybadola/pndconf),\n   which is integrated with ~ref-man~.\n\n* License\n\n  All the code in this repo except for external services and libraries are\n  licensed under AGPL 3.0 (or later). See LICENSE.md in this repo. To learn more\n  about AGPL see https://www.gnu.org/licenses/agpl-3.0.en.html.\n",
     'author': 'Akshay',
     'author_email': 'akshay.badola.cs@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/akshaybadola/ref-man-py',
```

### Comparing `ref-man-py-0.6.4/PKG-INFO` & `ref-man-py-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ref-man-py
-Version: 0.6.4
+Version: 0.7.0
 Summary: Ref Man Python Module
 Home-page: https://github.com/akshaybadola/ref-man-py
 License: AGPL-3
 Keywords: emacs,semanticscholar,bibliography,ref-man
 Author: Akshay
 Author-email: akshay.badola.cs@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Editors :: Emacs
+Requires-Dist: MarkupSafe (==2.0.1)
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: common_pyutil (>=0.8.5,<0.9.0)
 Requires-Dist: flask (>=1.1.2,<2.0.0)
 Requires-Dist: lxml (>=4.6.4,<5.0.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
```

