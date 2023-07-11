# Comparing `tmp/flardl-0.0.2.tar.gz` & `tmp/flardl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flardl-0.0.2.tar", max compression
+gzip compressed data, was "flardl-0.0.3.tar", max compression
```

## Comparing `flardl-0.0.2.tar` & `flardl-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1958 2023-06-26 23:44:15.902744 flardl-0.0.2/LICENSE
--rw-r--r--   0        0        0      243 2023-06-26 23:44:15.902744 flardl-0.0.2/LICENSE.logo.txt
--rw-r--r--   0        0        0     5376 2023-06-26 23:44:15.902744 flardl-0.0.2/README.md
--rw-r--r--   0        0        0     2732 2023-06-26 23:44:30.726867 flardl-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      748 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/common.py
--rw-r--r--   0        0        0     1581 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/dict_to_indexed_list.py
--rwxr-xr-x   0        0        0     3420 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/downloaders.py
--rwxr-xr-x   0        0        0    11759 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/multidispatcher.py
--rw-r--r--   0        0        0        0 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/py.typed
--rwxr-xr-x   0        0        0    11572 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/queue_stats.py
--rw-r--r--   0        0        0     6716 1970-01-01 00:00:00.000000 flardl-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-07-11 15:17:41.761070 flardl-0.0.3/LICENSE
+-rw-r--r--   0        0        0      243 2023-07-11 15:17:41.761070 flardl-0.0.3/LICENSE.logo.txt
+-rw-r--r--   0        0        0     5376 2023-07-11 15:17:41.761070 flardl-0.0.3/README.md
+-rw-r--r--   0        0        0     2762 2023-07-11 15:17:54.413354 flardl-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      624 2023-07-11 15:17:41.765070 flardl-0.0.3/src/flardl/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-11 15:17:41.765070 flardl-0.0.3/src/flardl/common.py
+-rw-r--r--   0        0        0     1581 2023-07-11 15:17:41.765070 flardl-0.0.3/src/flardl/dict_to_indexed_list.py
+-rwxr-xr-x   0        0        0     8126 2023-07-11 15:17:54.413354 flardl-0.0.3/src/flardl/downloader.py
+-rwxr-xr-x   0        0        0     4225 2023-07-11 15:17:41.769070 flardl-0.0.3/src/flardl/instrumented_streams.py
+-rwxr-xr-x   0        0        0     7146 2023-07-11 15:17:54.413354 flardl-0.0.3/src/flardl/multidispatcher.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:17:41.769070 flardl-0.0.3/src/flardl/py.typed
+-rwxr-xr-x   0        0        0    11622 2023-07-11 15:17:41.769070 flardl-0.0.3/src/flardl/stream_stats.py
+-rw-r--r--   0        0        0     6716 1970-01-01 00:00:00.000000 flardl-0.0.3/PKG-INFO
```

### Comparing `flardl-0.0.2/LICENSE` & `flardl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flardl-0.0.2/README.md` & `flardl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flardl-0.0.2/pyproject.toml` & `flardl-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flardl"
-version = "0.0.2"
+version = "0.0.3"
 description = "Flardl"
 authors = ["Joel Berendzen <joel@generisbio.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/hydrationdynamics/flardl"
 repository = "https://github.com/hydrationdynamics/flardl"
 documentation = "https://flardl.readthedocs.io"
@@ -37,15 +37,15 @@
 httpx = {extras = ["http2"], version = ">=0.23.3"}
 loguru = ">=0.6.0"
 tqdm = ">=4.64.1"
 uvloop = { version = ">=0.17.0", markers = "sys_platform != 'win32'"}
 trio = "^0.22.0"
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 flake8 = ">=4.0.1"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
@@ -67,14 +67,15 @@
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 # test deps for this package
 loguru-mypy = ">=0.0.4"
 pandas = ">=1.4.0"
 pandas-stubs = ">=1.5.2.221124"
 pytest-datadir-mgr = ">1.3.1"
+pytest-trio = ">=0.8.0"
 
 [tool.bandit]
 exclude_dirs = ["tests/", "noxfile.py"]
 skips = ["B101", "B311"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `flardl-0.0.2/src/flardl/__init__.py` & `flardl-0.0.3/src/flardl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,12 +6,10 @@
 from .common import INDEX_KEY  # noqa: F401
 from .common import MAX  # noqa: F401
 from .common import MIN  # noqa: F401
 from .common import NOBS  # noqa: F401
 from .common import RAVG  # noqa: F401
 from .common import SUM  # noqa: F401
 from .common import VALUE  # noqa: F401
-from .dict_to_indexed_list import zip_dict_to_indexed_list  # noqa: F401
-from .downloaders import MockDownloader  # noqa: F401
 from .multidispatcher import MultiDispatcher  # noqa: F401
-from .queue_stats import QueueStats  # noqa: F401
-from .queue_stats import WorkerStat  # noqa: F401
+from .stream_stats import StreamStats  # noqa: F401
+from .stream_stats import WorkerStat  # noqa: F401
```

### Comparing `flardl-0.0.2/src/flardl/common.py` & `flardl-0.0.3/src/flardl/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,53 @@
-"""Flardl--download list of URLs from a list of federated servers."""
+"""Shared constants, parameters, and routines."""
 from time import time
 from typing import Optional
 from typing import Union
 
 # third-party imports
 import numpy as np
 
 
 # The following globals are also attribute names,
 # don't change one without the other.
 ALL = "all"
 AVG = "avg"
 HIST = "history"
+INDEX_KEY = "idx"
 MAX = "max"
 MIN = "min"
 NOBS = "n_obs"
 RAVG = "r_avg"
 SUM = "sum"
 VALUE = "value"
-# pretty labels for substat names
+
+# Pretty labels for substat names.
 STAT_SUBLABELS = {
     VALUE: "",
     SUM: "total ",
     AVG: "average ",
     MIN: "min ",
     MAX: "max ",
     NOBS: "# ",
     HIST: "history ",
     RAVG: "rolling average ",
 }
-INDEX_KEY = "idx"
-# constants
 DEFAULT_ROUNDING = 2  # digits after decimal
 DEFAULT_MAX_RETRIES = 0
 TIME_ROUNDING = 1  # digits, milliseconds
 RATE_ROUNDING = 1  # digits, inverse seconds
 TIME_EPSILON = 0.01  # milliseconds
 BYTES_TO_MEGABITS = 8.0 / 1024.0 / 1024.0
 RANDOM_SEED = 87507
 DEFAULT_ZIPF_EXPONENT = 1.5  # more divergent as it gets closer to 1
 DEFAULT_ZIPF_SCALE = 1000
 DEFAULT_ZIPF_MIN = 1024
-# type defs
 NUMERIC_TYPE = Union[int, float]
 OPTIONAL_NUMERIC = Optional[NUMERIC_TYPE]
 OPTIONAL_NUMERIC_LIST = Union[OPTIONAL_NUMERIC, list[NUMERIC_TYPE]]
-TIME_ROUNDING = 1  # digits, milliseconds
 SIMPLE_TYPES = Union[int, float, bool, str, None]
 
 
 class RandomValueGenerator:
     """Seeded, reproducible random-value generation."""
 
     def __init__(
@@ -66,15 +64,15 @@
         self.zipf_exponent = zipf_exponent
 
     def get_wait_time(self, rate: float) -> float:
         """Given rate, return wait time from an exponential distribution."""
         return self.rng.exponential(1.0 / rate)
 
     def zipf_with_min(self) -> int:
-        """Return a Zipf's law-distributed integer with minimum.
+        """Return a Zipf-law-distributed integer with minimum.
 
         This distribution approximately describes many file-size
         distributions arising from natural language and human-written
         code (though code standards discourage large files). It
         is a sensitive function of the exponent, with exponents
         near 1.0 generating a higher divergence. For exponents
         greater than 2, there is only a small likelihood of
```

### Comparing `flardl-0.0.2/src/flardl/dict_to_indexed_list.py` & `flardl-0.0.3/src/flardl/dict_to_indexed_list.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.2/src/flardl/multidispatcher.py` & `flardl-0.0.3/src/flardl/multidispatcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,106 @@
-"""Work is dispatched to multiple workers and results collected via asynchio queues."""
+"""Work is dispatched to multiple workers and results collected via AnyIO streams."""
 from __future__ import annotations
 
-import math
 import sys
-from collections import Counter
 from typing import Any
-from typing import Union
-from typing import cast
+from typing import Optional
 
 # third-party imports
 import anyio
 import loguru
 from loguru import logger as mylogger
 
 from .common import DEFAULT_MAX_RETRIES
 from .common import INDEX_KEY
-from .common import RATE_ROUNDING
-from .common import TIME_EPSILON
+from .common import SIMPLE_TYPES
 from .common import MillisecondTimer
-from .queue_stats import QueueStats
-
-
-SIMPLE_TYPES = Union[int, float, str, None]
-LAUNCH_KEY = "launch_t"
-
-
-def get_index_value(item: dict[str, SIMPLE_TYPES]) -> int:
-    """Return value of index key."""
-    return cast(int, item[INDEX_KEY])
-
-
-class ArgumentStream:
-    """A stream of dictionaries to be used as arguments."""
-
-    def __init__(
-        self,
-        arg_list: list[dict[str, SIMPLE_TYPES]],
-        in_process: dict[str, Any],
-        timer: MillisecondTimer,
-    ):
-        """Initialize data structure for in-flight stats."""
-        self.send_stream, self.receive_stream = anyio.create_memory_object_stream(
-            max_buffer_size=math.inf
-        )
-        for args in arg_list:
-            self.send_stream.send_nowait(args)
-        self.n_args = len(arg_list)
-        self.inflight = in_process
-        self.timer = timer
-        self.launch_rate = 0.0
-        self.worker_counter: Counter[str] = Counter()
-        self._lock = anyio.Lock()
-
-    async def put(
-        self,
-        args,
-        /,
-        worker_name: str | None = None,
-        worker_count: int | None = None,
-    ):
-        """Put on results queue and update stats."""
-        worker_name = cast(str, worker_name)
-        worker_count = cast(int, worker_count)
-        async with self._lock:
-            del self.inflight[worker_name][worker_count]
-        await self.send_stream.send(args)
-
-    async def get(self, /, worker_name: str | None = None, **kwargs):
-        """Track de-queuing by worker."""
-        worker_name = cast(str, worker_name)
-        q_entry = self.receive_stream.receive_nowait(**kwargs)
-        async with self._lock:
-            self.worker_counter[worker_name] += 1
-            worker_count = self.worker_counter[worker_name]
-            if worker_name not in self.inflight:
-                self.inflight[worker_name] = {}
-            idx = q_entry[INDEX_KEY]
-            launch_time = self.timer.time()
-            self.launch_rate = round(
-                idx * 1000.0 / (launch_time + TIME_EPSILON), RATE_ROUNDING
-            )
-            self.inflight[worker_name][worker_count] = {
-                INDEX_KEY: idx,
-                "queue_depth": len(self.inflight[worker_name]),
-                LAUNCH_KEY: launch_time,
-                "cum_launch_rate": self.launch_rate,
-            }
-        return q_entry, worker_count
-
-
-class FailureStream:
-    """Anyio stream to track failures."""
-
-    launch_stats_out: list[str] = []
-
-    def __init__(
-        self,
-        in_process: dict[str, Any],
-    ) -> None:
-        """Init stats for queue."""
-        self.send_stream, self.receive_stream = anyio.create_memory_object_stream(
-            max_buffer_size=math.inf
-        )
-        self.inflight = in_process
-        self.count = 0
-        self._lock = anyio.Lock()
-
-    async def put(
-        self,
-        args,
-        /,
-        worker_name: str | None = None,
-        worker_count: int | None = None,
-    ):
-        """Put on results queue and update stats."""
-        worker_name = cast(str, worker_name)
-        worker_count = cast(int, worker_count)
-        launch_stats = self.inflight[worker_name][worker_count]
-        for result_name in self.launch_stats_out:
-            args[result_name] = launch_stats[result_name]
-        async with self._lock:
-            self.count += 1
-            del self.inflight[worker_name][worker_count]
-        await self.send_stream.send(args)
-
-    def get_all(self) -> list[dict[str, SIMPLE_TYPES]]:
-        """Return sorted list of stream contents."""
-        stream_contents = []
-        while True:
-            try:
-                stream_contents.append(self.receive_stream.receive_nowait())
-            except anyio.WouldBlock:
-                break
-        return sorted(stream_contents, key=get_index_value)
-
-
-class ResultStream(FailureStream):
-    """Stream for results."""
-
-    launch_stats_out = [LAUNCH_KEY]
+from .dict_to_indexed_list import NonStringIterable
+from .dict_to_indexed_list import zip_dict_to_indexed_list
+from .downloader import Downloader
+from .downloader import MockDownloader
+from .instrumented_streams import ArgumentStream
+from .instrumented_streams import FailureStream
+from .instrumented_streams import ResultStream
+from .stream_stats import StreamStats
 
 
 class MultiDispatcher:
     """Runs multiple single-site dispatchers sharing streams."""
 
-    def __init__(
+    def __init__(  # noqa: C901
         self,
-        worker_list: list,
+        all_worker_defs: list[dict[str, Any]],
         /,
+        worker_list: list[str] | None = None,
         max_retries: int = DEFAULT_MAX_RETRIES,
         logger: loguru.Logger | None = None,
         quiet: bool = False,
         history_len: int = 0,
+        output_dir: str | None = None,
+        mock: bool = False,
     ) -> None:
         """Save list of dispatchers."""
         if logger is None:
             self._logger = mylogger
         else:
             self._logger = logger
-        self.workers = worker_list
+        all_worker_names = [w["name"] for w in all_worker_defs]
+        if worker_list is None:
+            worker_defs = all_worker_defs
+        else:
+            worker_defs = []
+            for worker_name in worker_list:
+                try:
+                    worker_idx = all_worker_names.index(worker_name)
+                except ValueError:
+                    self._logger.error(f"Worker name {worker_name} not found.")
+                    sys.exit(1)
+                worker_defs.append(all_worker_defs[worker_idx])
+        self.workers = []
+        if mock:
+            worker_factory = MockDownloader
+        else:
+            worker_factory = Downloader
+        for i, worker_def in enumerate(worker_defs):
+            try:
+                worker = worker_factory(
+                    i, self._logger, output_dir, quiet, **worker_def
+                )
+            except Exception as e:
+                self._logger.warning(
+                    f"Worker {worker_def['name']} failed to initialize."
+                )
+                self._logger.warning(e)
+                continue
+            self.workers.append(worker)
+        if len(self.workers) == 0:
+            self._logger.error("No valid workers found.")
+            sys.exit(1)
         self.max_retries = max_retries
         self.exception_counter: dict[int, int] = {}
         self.n_too_many_retries = 0
         self.n_exceptions = 0
         self.quiet = quiet
-        self.queue_stats = QueueStats(worker_list, history_len=history_len)
+        self.queue_stats = StreamStats(all_worker_names, history_len=history_len)
         self._lock = anyio.Lock()
         self.inflight: dict[str, SIMPLE_TYPES] = {}
         self.timer = MillisecondTimer()
 
-    async def run(self, arg_list: list[dict[str, SIMPLE_TYPES]]):
+    async def run(
+        self,
+        args: (
+            list[dict[str, SIMPLE_TYPES]] | dict[str, NonStringIterable | SIMPLE_TYPES]
+        ),
+    ):
         """Run the multidispatcher queue."""
+        if isinstance(args, list):
+            arg_list = args
+        elif isinstance(args, dict):
+            arg_list = zip_dict_to_indexed_list(args)
         arg_q = ArgumentStream(arg_list, self.inflight, self.timer)
         result_stream = ResultStream(self.inflight)
         failure_stream = FailureStream(self.inflight)
 
         async with anyio.create_task_group() as tg:
             for worker in self.workers:
                 tg.start_soon(
@@ -257,91 +183,7 @@
             backend = "trio"
         else:
             self._logger.error(f"Unknown configuration {config}")
             sys.exit(1)
         return anyio.run(
             self.run, arg_list, backend=backend, backend_options=backend_options
         )
-
-
-class QueueWorker:
-    """Basic worker functions."""
-
-    def __init__(
-        self, name: str, logger: loguru.Logger | None = None, quiet: bool = False
-    ):
-        """Init data structures."""
-        if logger is None:
-            self._logger = mylogger
-        else:
-            self._logger = logger
-        self.name = name
-        self.n_soft_fails = 0
-        self.n_hard_fails = 0
-        self.hard_exceptions: tuple[()] | tuple[type[BaseException]] = ()
-        self.soft_exceptions: tuple[()] | tuple[type[BaseException]] = ()
-        self.work_qty_name = "bytes"
-        self.quiet = quiet
-
-    async def queue_results(
-        self,
-        result_q: ResultStream,
-        worker_count: int,
-        idx: int,
-        work_qty: float | int,
-        /,
-        **kwargs: SIMPLE_TYPES,
-    ):
-        """Put dictionary of results on ouput queue."""
-        results = {
-            INDEX_KEY: idx,
-            "worker": self.name,
-            self.work_qty_name: work_qty,
-        }
-        results.update(kwargs)
-        await result_q.put(results, worker_name=self.name, worker_count=worker_count)
-
-    async def hard_exception_handler(
-        self,
-        index: int,
-        worker_name: str,
-        worker_count: int,
-        error: Exception,
-        failure_q: FailureStream,
-    ):
-        """Handle exceptions that re-queue arguments as failed."""
-        if error.__class__ in self.soft_exceptions:
-            message = repr(error)
-            error_name = "TooManyRetries"
-        else:
-            message = str(error)
-            error_name = error.__class__.__name__
-        if not self.quiet:
-            self._logger.error(f"{error_name}: {message}")
-        failure_entry = {
-            INDEX_KEY: index,
-            "worker": worker_name,
-            "error": error_name,
-            "message": message,
-        }
-        await failure_q.put(
-            failure_entry, worker_name=worker_name, worker_count=worker_count
-        )
-
-    async def unhandled_exception_handler(self, index: int, error: Exception):
-        """Handle unhandled exceptions."""
-        self._logger.error(error)
-        await self._logger.complete()
-        sys.exit(1)
-
-    async def soft_exception_handler(
-        self,
-        kwargs: dict[str, Any],
-        worker_name: str,
-        worker_count: int,
-        error: Exception,
-        arg_q: ArgumentStream,
-    ):
-        """Handle exceptions that re-try arguments."""
-        if not self.quiet:
-            self._logger.warning(error)
-        await arg_q.put(kwargs, worker_name=worker_name, worker_count=worker_count)
```

### Comparing `flardl-0.0.2/src/flardl/queue_stats.py` & `flardl-0.0.3/src/flardl/stream_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Simple queue-associated statistical functions."""
+"""Simple stream-associated statistical functions."""
 from collections import UserDict
 from collections import deque
 from typing import Any
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 
@@ -19,19 +19,19 @@
 from .common import NUMERIC_TYPE
 from .common import RAVG
 from .common import STAT_SUBLABELS
 from .common import SUM
 from .common import VALUE
 
 
-# type defs
+# type definitions
 OPTIONAL_NUMERIC = Optional[NUMERIC_TYPE]
 OPTIONAL_NUMERIC_LIST = Union[OPTIONAL_NUMERIC, list[NUMERIC_TYPE]]
 
-QueueStatsType = TypeVar("QueueStatsType", bound="QueueStats")
+StreamStatsType = TypeVar("StreamStatsType", bound="StreamStats")
 StatType = TypeVar("StatType", bound="Stat")
 U = TypeVar("U")
 
 
 def _nn(inst: Optional[U]) -> U:
     """Not-none helper to pass mypy."""
     assert inst is not None
@@ -44,14 +44,15 @@
     if rounding == 0:
         return int(rounded_val)
     return rounded_val
 
 
 def _set_stat(instance: StatType, attrib: Attribute, val: NUMERIC_TYPE) -> NUMERIC_TYPE:
     """Round stat value and set derived quantities."""
+    _unused = (attrib,)  # noqa: F841
     rounded_val = _round(val, instance._rounding)
     instance.n_obs += 1
     if instance.value is None:
         instance.min = rounded_val
         instance.max = rounded_val
         instance.sum = rounded_val
         instance.avg = rounded_val
@@ -164,15 +165,15 @@
     substat: str
     label: Optional[str] = None
     name: Optional[str] = None
     scale: Optional[float] = None
     rounding: Optional[int] = None
 
 
-class QueueStats(UserDict):
+class StreamStats(UserDict):
     """Dictionary of per-worker queue stats with update calculations."""
 
     stat_data = {
         "retirement_t": StatData("retirement time, ms", rounding=2),
         "launch_t": StatData("launch time, ms", rounding=2),
         "service_t": StatData("service time, ns", rounding=2),
         "bytes": StatData("bytes downloaded", rounding=0),
```

### Comparing `flardl-0.0.2/PKG-INFO` & `flardl-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flardl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flardl
 Home-page: https://github.com/hydrationdynamics/flardl
 License: BSD-3-Clause
 Keywords: downloads,adaptive,federated
 Author: Joel Berendzen
 Author-email: joel@generisbio.com
 Requires-Python: >=3.9,<4
```

