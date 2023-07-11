# Comparing `tmp/oms-mqclient-2.1.1.tar.gz` & `tmp/oms-mqclient-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.1.1.tar", last modified: Thu Jul  6 22:28:21 2023, max compression
+gzip compressed data, was "oms-mqclient-2.2.0.tar", last modified: Tue Jul 11 01:28:57 2023, max compression
```

## Comparing `oms-mqclient-2.1.1.tar` & `oms-mqclient-2.2.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.795826 oms-mqclient-2.1.1/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-06 22:28:19.000000 oms-mqclient-2.1.1/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5808 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.795826 oms-mqclient-2.1.1/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12421 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    12368 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15483 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    22595 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2731 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.795826 oms-mqclient-2.1.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7026 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    33482 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.574231 oms-mqclient-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 01:28:57.574231 oms-mqclient-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.566231 oms-mqclient-2.2.0/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 01:28:55.000000 oms-mqclient-2.2.0/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.566231 oms-mqclient-2.2.0/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13328 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    15335 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    24593 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.566231 oms-mqclient-2.2.0/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-07-11 01:28:57.574231 oms-mqclient-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.562231 oms-mqclient-2.2.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    33482 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5586 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.1.1/LICENSE` & `oms-mqclient-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/PKG-INFO` & `oms-mqclient-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.1.1/README.md` & `oms-mqclient-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/mqclient/__init__.py` & `oms-mqclient-2.2.0/mqclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.1.1/mqclient/broker_client_interface.py` & `oms-mqclient-2.2.0/mqclient/broker_client_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 import pickle
 from enum import Enum, auto
 from typing import Any, AsyncGenerator, Dict, Optional, Union
 
 MessageID = Union[int, str, bytes]
 
-TIMEOUT_MILLIS_DEFAULT = 1000  # milliseconds
-RETRY_DELAY = 1  # seconds
-TRY_ATTEMPTS = 3  # ex: 3 means 1 initial try and 2 retries
-
 
 class ConnectingFailedException(Exception):
     """Raised when a `connect()` fails."""
 
 
 class ClosingFailedException(Exception):
     """Raised when a `close()` fails."""
@@ -118,15 +114,20 @@
     async def close(self) -> None:
         """Close interface to queue."""
 
 
 class Pub(RawQueue):
     """Publisher queue."""
 
-    async def send_message(self, msg: bytes) -> None:
+    async def send_message(
+        self,
+        msg: bytes,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Send a message on a queue."""
         raise NotImplementedError()
 
 
 class Sub(RawQueue):
     """Subscriber queue."""
 
@@ -138,29 +139,46 @@
     @staticmethod
     def _to_message(*args: Any) -> Optional[Message]:
         """Convert broker_client-specific payload to standardized Message
         type."""
         raise NotImplementedError()
 
     async def get_message(
-        self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
+        self,
+        timeout_millis: Optional[int],
+        retries: int,
+        retry_delay: int,
     ) -> Optional[Message]:
         """Get a single message from a queue."""
         raise NotImplementedError()
 
-    async def ack_message(self, msg: Message) -> None:
+    async def ack_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Ack a message from the queue."""
         raise NotImplementedError()
 
-    async def reject_message(self, msg: Message) -> None:
+    async def reject_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Reject (nack) a message from the queue."""
         raise NotImplementedError()
 
     def message_generator(  # NOTE: no `async` b/c it's abstract; overriding methods will need `async`
-        self, timeout: int = 60, propagate_error: bool = True
+        self,
+        timeout: int,
+        propagate_error: bool,
+        retries: int,
+        retry_delay: int,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Asynchronously generate messages with variable timeout.
         Yield `None` on `athrow()`.
 
         Keyword Arguments:
```

### Comparing `oms-mqclient-2.1.1/mqclient/broker_client_manager.py` & `oms-mqclient-2.2.0/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.2.0/mqclient/broker_clients/apachepulsar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Back-end using Apache Pulsar."""
 
 import asyncio
+import functools
 import logging
-import time
 from typing import AsyncGenerator, Optional
 
 import pulsar  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
-    RETRY_DELAY,
-    TIMEOUT_MILLIS_DEFAULT,
-    TRY_ATTEMPTS,
     AlreadyClosedException,
     ClosingFailedException,
     Message,
     Pub,
     RawQueue,
     Sub,
 )
+from . import utils
 
 LOGGER = logging.getLogger("mqclient.pulsar")
 
 
 class Pulsar(RawQueue):
     """Base Pulsar wrapper.
 
@@ -119,21 +117,36 @@
         """Close connection."""
         LOGGER.debug(log_msgs.CLOSING_PUB)
         await super().close()
         if not self.producer:
             raise ClosingFailedException("No producer to sub.")
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
-    async def send_message(self, msg: bytes) -> None:
+    async def send_message(
+        self,
+        msg: bytes,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Send a message on a queue."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.producer:
             raise RuntimeError("queue is not connected")
 
-        self.producer.send(msg)
+        await utils.auto_retry_call(
+            func=functools.partial(
+                self.producer.send,
+                msg,
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
 class PulsarSub(Pulsar, Sub):
     """Wrapper around pulsar.Consumer.
 
     Extends:
@@ -200,88 +213,119 @@
         if isinstance(id_, pulsar._pulsar.MessageId):  # pylint: disable=I1101,W0212
             return Message(id_.serialize(), data)
         # Send original data
         else:
             return Message(id_, data)
 
     async def get_message(
-        self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
+        self,
+        timeout_millis: Optional[int],
+        retries: int,
+        retry_delay: int,
     ) -> Optional[Message]:
         """Get a single message from a queue.
 
         To endlessly block until a message is available, set
         `timeout_millis=None`.
         """
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self.consumer:
             raise RuntimeError("queue is not connected")
 
-        for i in range(TRY_ATTEMPTS):
-            if i > 0:
-                LOGGER.debug(
-                    f"{log_msgs.GETMSG_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
-                )
-
-            try:
-                recvd = self.consumer.receive(timeout_millis=timeout_millis)
-                msg = PulsarSub._to_message(recvd)
-                if msg:
-                    LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg}).")
-                    return msg
-                else:
-                    LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
-                    return None
-
-            except Exception as e:
-                # https://github.com/apache/pulsar/issues/3127
-                if str(e) == "Pulsar error: TimeOut":
-                    LOGGER.debug(log_msgs.GETMSG_TIMEOUT_ERROR)
-                    return None
-                # https://github.com/apache/pulsar/issues/3127
-                if str(e) == "Pulsar error: AlreadyClosed":
-                    await self.close()
-                    time.sleep(RETRY_DELAY)
-                    await self.connect()
-                    continue
-                LOGGER.debug(
-                    f"{log_msgs.GETMSG_RAISE_OTHER_ERROR} ({e.__class__.__name__})."
-                )
-                raise
-
-        LOGGER.debug(log_msgs.GETMSG_CONNECTION_ERROR_MAX_RETRIES)
-        raise Exception("Pulsar connection error")
+        try:
+            pulsar_msg = await utils.auto_retry_call(
+                func=functools.partial(
+                    self.consumer.receive,
+                    timeout_millis=timeout_millis,
+                ),
+                retries=retries,
+                retry_delay=retry_delay,
+                close=self.close,
+                connect=self.connect,
+                logger=LOGGER,
+                nonretriable_conditions=lambda e: str(e) == "Pulsar error: TimeOut",
+            )
+        except Exception as e:
+            # https://github.com/apache/pulsar/issues/3127
+            # consumer timed out so there's nothing left in the tube
+            if str(e) == "Pulsar error: TimeOut":
+                LOGGER.debug(log_msgs.GETMSG_TIMEOUT_ERROR)
+                return None
+            raise
+        if msg := PulsarSub._to_message(pulsar_msg):
+            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg}).")
+            return msg
+        else:
+            LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
+            return None
 
-    async def ack_message(self, msg: Message) -> None:
+    async def ack_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self.consumer:
             raise RuntimeError("queue is not connected")
 
         if isinstance(msg.msg_id, bytes):
-            self.consumer.acknowledge(pulsar.MessageId.deserialize(msg.msg_id))
+            pulsar_msg = pulsar.MessageId.deserialize(msg.msg_id)
         else:
-            self.consumer.acknowledge(msg.msg_id)
+            pulsar_msg = msg.msg_id
 
+        await utils.auto_retry_call(
+            func=functools.partial(
+                self.consumer.acknowledge,
+                pulsar_msg,
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg}).")
 
-    async def reject_message(self, msg: Message) -> None:
+    async def reject_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self.consumer:
             raise RuntimeError("queue is not connected")
 
         if isinstance(msg.msg_id, bytes):
-            self.consumer.negative_acknowledge(pulsar.MessageId.deserialize(msg.msg_id))
+            pulsar_msg = pulsar.MessageId.deserialize(msg.msg_id)
         else:
-            self.consumer.negative_acknowledge(msg.msg_id)
+            pulsar_msg = msg.msg_id
 
+        await utils.auto_retry_call(
+            func=functools.partial(
+                self.consumer.negative_acknowledge,
+                pulsar_msg,
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg}).")
 
     async def message_generator(
-        self, timeout: int = 60, propagate_error: bool = True
+        self,
+        timeout: int,
+        propagate_error: bool,
+        retries: int,
+        retry_delay: int,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
@@ -293,15 +337,19 @@
             raise RuntimeError("queue is not connected")
 
         msg = None
         try:
             while True:
                 # get message
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
-                msg = await self.get_message(timeout_millis=timeout * 1000)
+                msg = await self.get_message(
+                    timeout_millis=timeout * 1000,
+                    retries=retries,
+                    retry_delay=retry_delay,
+                )
                 if msg is None:
                     LOGGER.info(log_msgs.MSGGEN_NO_MESSAGE_LOOK_BACK_IN_QUEUE)
                     break
 
                 # yield message to consumer
                 try:
                     LOGGER.debug(f"{log_msgs.MSGGEN_YIELDING_MESSAGE} [{msg}]")
```

### Comparing `oms-mqclient-2.1.1/mqclient/broker_clients/nats.py` & `oms-mqclient-2.2.0/mqclient/broker_clients/nats.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 """Back-end using NATS."""
 
 
+import functools
 import logging
 import math
-import time
-from functools import partial
-from typing import (
-    Any,
-    AsyncGenerator,
-    Awaitable,
-    Callable,
-    List,
-    Optional,
-    TypeVar,
-    cast,
-)
+from typing import Any, AsyncGenerator, List, Optional, TypeVar, cast
 
 import nats
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
-    RETRY_DELAY,
-    TIMEOUT_MILLIS_DEFAULT,
-    TRY_ATTEMPTS,
     ClosingFailedException,
     Message,
     Pub,
     RawQueue,
     Sub,
 )
+from ..config import DEFAULT_TIMEOUT_MILLIS
+from . import utils
 
 LOGGER = logging.getLogger("mqclient.nats")
 
 T = TypeVar("T")  # the callable/awaitable return type
 
 
 async def _anext(gen: AsyncGenerator[Any, Any], default: Any) -> Any:
@@ -42,39 +31,14 @@
     """
     try:
         return await gen.__anext__()
     except StopAsyncIteration:
         return default
 
 
-async def try_call(self: "NATS", func: Callable[..., Awaitable[T]]) -> T:
-    """Call `func` with auto-retries."""
-    i = 0
-    while True:
-        if i > 0:
-            LOGGER.debug(
-                f"{log_msgs.TRYCALL_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
-            )
-
-        try:
-            return await func()
-        except nats.errors.TimeoutError:
-            raise
-        except Exception as e:  # pylint:disable=broad-except
-            LOGGER.debug(f"[try_call()] Encountered exception: '{e}'")
-            if i == TRY_ATTEMPTS - 1:
-                LOGGER.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
-                raise
-
-        await self.close()
-        time.sleep(RETRY_DELAY)
-        await self.connect()
-        i += 1
-
-
 class NATS(RawQueue):
     """Base NATS wrapper, using JetStream.
 
     Extends:
         RawQueue
     """
 
@@ -94,15 +58,15 @@
         LOGGER.debug(f"Stream & Subject: {stream_id}/{self.subject}")
 
     async def connect(self) -> None:
         """Set up connection and channel."""
         await super().connect()
         self._nats_client = await nats.connect(self.endpoint)  # type: ignore[arg-type]
         # Create JetStream context
-        self.js = self._nats_client.jetstream(timeout=TIMEOUT_MILLIS_DEFAULT // 1000)
+        self.js = self._nats_client.jetstream(timeout=DEFAULT_TIMEOUT_MILLIS // 1000)
         await self.js.add_stream(name=self.stream_id, subjects=[self.subject])
 
     async def close(self) -> None:
         """Close connection."""
         await super().close()
         if not self._nats_client:
             raise ClosingFailedException("No connection to close.")
@@ -130,22 +94,36 @@
 
     async def close(self) -> None:
         """Close pub (no-op)."""
         LOGGER.debug(log_msgs.CLOSING_PUB)
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
-    async def send_message(self, msg: bytes) -> None:
+    async def send_message(
+        self,
+        msg: bytes,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Send a message (publish)."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.js:
             raise RuntimeError("JetStream is not connected")
 
-        ack: nats.js.api.PubAck = await try_call(
-            self, partial(self.js.publish, self.subject, msg)
+        ack: nats.js.api.PubAck = await utils.auto_retry_call(
+            func=functools.partial(
+                self.js.publish,
+                self.subject,
+                msg,
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
         )
         LOGGER.debug(f"Sent Message w/ Ack: {ack}")
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
 class NATSSub(NATS, Sub):
     """Wrapper around queue with prefetch-queue, using JetStream.
@@ -199,97 +177,156 @@
             subject=self.subject,
             reply=cast(str, msg.msg_id),  # we know this is str b/c `_to_message()`
             data=msg.data,
             headers=None,  # default
         )
 
     async def _get_messages(
-        self, timeout_millis: Optional[int], num_messages: int
+        self,
+        timeout_millis: Optional[int],
+        num_messages: int,
+        retries: int,
+        retry_delay: int,
     ) -> List[Message]:
         """Get n messages.
 
         The subscriber pulls a specific number of messages. The actual
         number of messages pulled may be smaller than `num_messages`.
         """
         if not self._subscription:
             raise RuntimeError("Subscriber is not connected")
 
         if not timeout_millis:
-            timeout_millis = TIMEOUT_MILLIS_DEFAULT
+            timeout_millis = DEFAULT_TIMEOUT_MILLIS
 
         try:
-            nats_msgs: List[nats.aio.msg.Msg] = await try_call(
-                self,
-                partial(
+            nats_msgs: List[nats.aio.msg.Msg] = await utils.auto_retry_call(
+                func=functools.partial(
                     self._subscription.fetch,
                     num_messages,
                     int(math.ceil(timeout_millis / 1000)),
                 ),
+                retries=retries,
+                retry_delay=retry_delay,
+                close=self.close,
+                connect=self.connect,
+                logger=LOGGER,
+                nonretriable_conditions=lambda e: isinstance(
+                    e, nats.errors.TimeoutError
+                ),
             )
         except nats.errors.TimeoutError:
+            LOGGER.debug(log_msgs.GETMSG_TIMEOUT_ERROR)
+            return []
+        if not nats_msgs:
+            LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
             return []
-
         msgs = []
         for recvd in nats_msgs:
-            msg = self._to_message(recvd)
-            if msg:
+            if msg := self._to_message(recvd):
+                LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg}).")
                 msgs.append(msg)
         return msgs
 
     async def get_message(
-        self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
+        self,
+        timeout_millis: Optional[int],
+        retries: int,
+        retry_delay: int,
     ) -> Optional[Message]:
         """Get a message."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self._subscription:
             raise RuntimeError("Subscriber is not connected.")
 
         try:
-            msg = (await self._get_messages(timeout_millis, 1))[0]
-            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg}).")
+            msg = (
+                await self._get_messages(
+                    timeout_millis,
+                    1,
+                    retries,
+                    retry_delay,
+                )
+            )[0]
             return msg
         except IndexError:
-            LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
             return None
 
     async def _gen_messages(
-        self, timeout_millis: Optional[int], num_messages: int
+        self,
+        timeout_millis: Optional[int],
+        num_messages: int,
+        retries: int,
+        retry_delay: int,
     ) -> AsyncGenerator[Message, None]:
         """Continuously generate messages until there are no more."""
         if not self._subscription:
             raise RuntimeError("Subscriber is not connected.")
 
         while True:
-            msgs = await self._get_messages(timeout_millis, num_messages)
+            msgs = await self._get_messages(
+                timeout_millis,
+                num_messages,
+                retries,
+                retry_delay,
+            )
             if not msgs:
                 return
             for msg in msgs:
                 yield msg
 
-    async def ack_message(self, msg: Message) -> None:
+    async def ack_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
         # Acknowledges the received messages so they will not be sent again.
-        await try_call(self, partial(self._from_message(msg).ack))
+        await utils.auto_retry_call(
+            func=self._from_message(msg).ack,  # type: ignore[arg-type]
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
 
-    async def reject_message(self, msg: Message) -> None:
+    async def reject_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
-        await try_call(self, partial(self._from_message(msg).nak))  # yes, it's "nak"
+        await utils.auto_retry_call(
+            func=self._from_message(msg).nak,  # type: ignore[arg-type]  # yes, it's "nak"
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def message_generator(
-        self, timeout: int = 60, propagate_error: bool = True
+        self,
+        timeout: int,
+        propagate_error: bool,
+        retries: int,
+        retry_delay: int,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
@@ -298,15 +335,20 @@
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
         msg = None
         try:
-            gen = self._gen_messages(timeout * 1000, self.prefetch)
+            gen = self._gen_messages(
+                timeout * 1000,
+                self.prefetch,
+                retries,
+                retry_delay,
+            )
             while True:
                 # get message
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
                 msg = await _anext(gen, None)
                 if msg is None:
                     LOGGER.info(log_msgs.MSGGEN_NO_MESSAGE_LOOK_BACK_IN_QUEUE)
                     break
```

### Comparing `oms-mqclient-2.1.1/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.2.0/mqclient/broker_clients/rabbitmq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Back-end using RabbitMQ."""
 
+import functools
 import logging
-import time
 import urllib
-from functools import partial
-from typing import Any, AsyncGenerator, Callable, Dict, Optional, Tuple, Union
+from typing import Any, AsyncGenerator, AsyncIterator, Dict, Optional, Tuple, Union
 
 import pika  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
-    RETRY_DELAY,
-    TIMEOUT_MILLIS_DEFAULT,
-    TRY_ATTEMPTS,
     AlreadyClosedException,
     ClosingFailedException,
     ConnectingFailedException,
     Message,
     Pub,
     RawQueue,
     Sub,
 )
+from . import utils
 
 StrDict = Dict[str, Any]
 
 LOGGER = logging.getLogger("mqclient.rabbitmq")
 
 
 HUMAN_PATTERN = "[SCHEME://][USER[:PASS]@]HOST[:PORT][/VIRTUAL_HOST]"
@@ -124,15 +121,15 @@
             raise ClosingFailedException("No channel to close.")
         if not self.connection:
             raise ClosingFailedException("No connection to close.")
         if self.connection.is_closed:
             raise AlreadyClosedException()
 
         try:
-            self.channel.cancel()
+            # self.channel.cancel() -- done by self.connection.close()
             self.connection.close()
         except Exception as e:
             raise ClosingFailedException() from e
 
         if self.channel.is_open:
             LOGGER.warning("Channel remains open after connection close.")
 
@@ -166,36 +163,48 @@
 
     async def close(self) -> None:
         """Close connection."""
         LOGGER.debug(log_msgs.CLOSING_PUB)
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
-    async def send_message(self, msg: bytes) -> None:
+    async def send_message(
+        self,
+        msg: bytes,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Send a message on a queue.
 
         Args:
             address (str): address of queue
             name (str): name of queue on address
 
         Returns:
             RawQueue: queue
         """
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
-        await try_call(
-            self,
-            partial(
+        await utils.auto_retry_call(
+            func=functools.partial(
                 self.channel.basic_publish,
                 exchange="",
                 routing_key=self.queue,
                 body=msg,
             ),
+            nonretriable_conditions=lambda e: isinstance(
+                e, pika.exceptions.AMQPChannelError
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
         )
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
 class RabbitMQSub(RabbitMQ, Sub):
     """Wrapper around queue with prefetch-queue QoS.
 
@@ -235,79 +244,151 @@
         """
         LOGGER.debug(log_msgs.CLOSING_SUB)
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_SUB)
 
     @staticmethod
     def _to_message(  # type: ignore[override]  # noqa: F821 # pylint: disable=W0221
-        method_frame: Optional[pika.spec.Basic.GetOk], body: Optional[Union[str, bytes]]
+        method_frame: Optional[pika.spec.Basic.GetOk],
+        body: Optional[Union[str, bytes]],
     ) -> Optional[Message]:
         """Transform RabbitMQ-Message to Message type."""
         if not method_frame or body is None:
             return None
 
         if isinstance(body, str):
             return Message(method_frame.delivery_tag, body.encode())
         else:
             return Message(method_frame.delivery_tag, body)
 
+    async def _iter_messages(
+        self,
+        timeout_millis: Optional[int],
+        retries: int,
+        retry_delay: int,
+    ) -> AsyncIterator[Optional[Message]]:
+        if not self.channel:
+            raise RuntimeError("queue is not connected")
+
+        iterator = self.channel.consume(
+            self.queue,
+            inactivity_timeout=timeout_millis / 1000.0 if timeout_millis else None,
+        )
+
+        while True:
+            try:
+                pika_msg = await utils.auto_retry_call(
+                    func=functools.partial(next, iterator),
+                    nonretriable_conditions=lambda e: isinstance(
+                        e, (pika.exceptions.AMQPChannelError, StopIteration)
+                    ),
+                    retries=retries,
+                    retry_delay=retry_delay,
+                    close=self.close,
+                    connect=self.connect,
+                    logger=LOGGER,
+                )
+            except StopIteration:
+                LOGGER.debug(log_msgs.GETMSG_TIMEOUT_ERROR)
+                return
+            if msg := RabbitMQSub._to_message(pika_msg[0], pika_msg[2]):  # type: ignore[index]
+                LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg.msg_id!r}).")
+                yield msg
+            else:
+                LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
+                yield None
+
     async def get_message(
-        self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
+        self,
+        timeout_millis: Optional[int],
+        retries: int,
+        retry_delay: int,
     ) -> Optional[Message]:
         """Get a message from a queue."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
-        gen = partial(
-            self.channel.consume,
-            self.queue,
-            inactivity_timeout=timeout_millis / 1000.0 if timeout_millis else None,
-        )
-        async for method_frame, _, body in try_yield(self, gen):
-            msg = RabbitMQSub._to_message(method_frame, body)  # None -> timeout
+        msg = None
+        async for msg in self._iter_messages(timeout_millis, retries, retry_delay):
+            # None -> timeout
             break  # get just one message
 
         # self.channel.cancel()  # this is done by `open_sub_one()` *after* ack/nack via `close()`
 
-        if msg:
-            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg.msg_id!r}).")
-            return msg
-        else:
-            LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
-            return None
+        return msg
 
-    async def ack_message(self, msg: Message) -> None:
+    async def ack_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Ack a message from the queue.
 
         Note that RabbitMQ acks messages in-order, so acking message 3
         of 3 in-progress messages will ack them all.
         """
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
-        await try_call(self, partial(self.channel.basic_ack, msg.msg_id))
+        await utils.auto_retry_call(
+            func=functools.partial(
+                self.channel.basic_ack,
+                msg.msg_id,
+            ),
+            nonretriable_conditions=lambda e: isinstance(
+                e, pika.exceptions.AMQPChannelError
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
 
-    async def reject_message(self, msg: Message) -> None:
+    async def reject_message(
+        self,
+        msg: Message,
+        retries: int,
+        retry_delay: int,
+    ) -> None:
         """Reject (nack) a message from the queue.
 
         Note that RabbitMQ acks messages in-order, so nacking message 3
         of 3 in-progress messages will nack them all.
         """
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
-        await try_call(self, partial(self.channel.basic_nack, msg.msg_id))
+        await utils.auto_retry_call(
+            func=functools.partial(
+                self.channel.basic_nack,
+                msg.msg_id,
+            ),
+            nonretriable_conditions=lambda e: isinstance(
+                e, pika.exceptions.AMQPChannelError
+            ),
+            retries=retries,
+            retry_delay=retry_delay,
+            close=self.close,
+            connect=self.connect,
+            logger=LOGGER,
+        )
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def message_generator(
-        self, timeout: int = 60, propagate_error: bool = True
+        self,
+        timeout: int,
+        propagate_error: bool,
+        retries: int,
+        retry_delay: int,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
@@ -316,19 +397,15 @@
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
         msg = None
         try:
-            gen = partial(self.channel.consume, self.queue, inactivity_timeout=timeout)
-
-            async for method_frame, _, body in try_yield(self, gen):
-                # get message
-                msg = RabbitMQSub._to_message(method_frame, body)
+            async for msg in self._iter_messages(timeout * 1000, retries, retry_delay):
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
                 if not msg:
                     LOGGER.info(log_msgs.MSGGEN_NO_MESSAGE_LOOK_BACK_IN_QUEUE)
                     break
 
                 # yield message to consumer
                 try:
@@ -355,79 +432,14 @@
             LOGGER.debug(log_msgs.MSGGEN_GENERATOR_EXITED)
 
         # Done with generator, one way or another
         finally:
             self.channel.cancel()
 
 
-async def try_call(queue: RabbitMQ, func: Callable[..., Any]) -> Any:
-    """Try to call `func` and return value.
-
-    Try up to `TRY_ATTEMPTS` times, for connection-related errors.
-    """
-    for i in range(TRY_ATTEMPTS):
-        if i > 0:
-            LOGGER.debug(
-                f"{log_msgs.TRYCALL_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
-            )
-
-        try:
-            return func()
-        except pika.exceptions.ConnectionClosedByBroker:
-            LOGGER.debug(log_msgs.TRYCALL_CONNECTION_CLOSED_BY_BROKER)
-        # Do not recover on channel errors
-        except pika.exceptions.AMQPChannelError as err:
-            LOGGER.error(f"{log_msgs.TRYCALL_RAISE_AMQP_CHANNEL_ERROR} {err}.")
-            raise
-        # Recover on all other connection errors
-        except pika.exceptions.AMQPConnectionError:
-            LOGGER.debug(log_msgs.TRYCALL_AMQP_CONNECTION_ERROR)
-
-        await queue.close()
-        time.sleep(RETRY_DELAY)
-        await queue.connect()
-
-    LOGGER.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
-    raise Exception("RabbitMQ connection error")
-
-
-async def try_yield(
-    queue: RabbitMQ, func: Callable[..., Any]
-) -> AsyncGenerator[Any, None]:
-    """Try to call `func` and yield value(s).
-
-    Try up to `TRY_ATTEMPTS` times, for connection-related errors.
-    """
-    for i in range(TRY_ATTEMPTS):
-        if i > 0:
-            LOGGER.debug(
-                f"{log_msgs.TRYYIELD_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
-            )
-
-        try:
-            for x in func():  # pylint: disable=invalid-name
-                yield x
-        except pika.exceptions.ConnectionClosedByBroker:
-            LOGGER.debug(log_msgs.TRYYIELD_CONNECTION_CLOSED_BY_BROKER)
-        # Do not recover on channel errors
-        except pika.exceptions.AMQPChannelError as err:
-            LOGGER.error(f"{log_msgs.TRYYIELD_RAISE_AMQP_CHANNEL_ERROR} {err}.")
-            raise
-        # Recover on all other connection errors
-        except pika.exceptions.AMQPConnectionError:
-            LOGGER.debug(log_msgs.TRYYIELD_AMQP_CONNECTION_ERROR)
-
-        await queue.close()
-        time.sleep(RETRY_DELAY)
-        await queue.connect()
-
-    LOGGER.debug(log_msgs.TRYYIELD_CONNECTION_ERROR_MAX_RETRIES)
-    raise Exception("RabbitMQ connection error")
-
-
 class BrokerClient(broker_client_interface.BrokerClient):
     """RabbitMQ Pub-Sub BrokerClient Factory.
 
     Extends:
         BrokerClient
     """
```

### Comparing `oms-mqclient-2.1.1/mqclient/log_msgs.py` & `oms-mqclient-2.2.0/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/mqclient/queue.py` & `oms-mqclient-2.2.0/mqclient/queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Queue class encapsulating a pub-sub messaging system."""
 
 import contextlib
+import functools
 import logging
 import os
 import sys
 import types
 import uuid
 from typing import (
     Any,
@@ -16,14 +17,20 @@
     Optional,
     Type,
 )
 
 from . import broker_client_manager
 from . import telemetry as wtt
 from .broker_client_interface import AckException, Message, NackException, Pub, Sub
+from .config import (
+    DEFAULT_EXCEPT_ERRORS,
+    DEFAULT_RETRIES,
+    DEFAULT_RETRY_DELAY,
+    DEFAULT_TIMEOUT,
+)
 
 LOGGER = logging.getLogger("mqclient")
 
 
 # deprecation check
 for envvar in ["RABBITMQ_HEARTBEAT", "PULSAR_UNACKED_MESSAGES_TIMEOUT_SEC"]:
     if os.getenv(envvar):
@@ -57,32 +64,40 @@
 
     def __init__(
         self,
         broker_client: str,
         address: str = "localhost",
         name: str = "",
         prefetch: int = 1,
-        timeout: int = 60,
+        timeout: int = DEFAULT_TIMEOUT,
         ack_timeout: Optional[int] = None,
-        except_errors: bool = True,
+        retry_delay: int = DEFAULT_RETRY_DELAY,  # seconds
+        retries: int = DEFAULT_RETRIES,  # ex: 2 means 1 initial try and 2 retries
+        except_errors: bool = DEFAULT_EXCEPT_ERRORS,
         auth_token: str = "",
     ) -> None:
         self._broker_client = broker_client_manager.get_broker_client(broker_client)
         self._address = address
         self._name = name if name else Queue.make_name()
         self._prefetch = prefetch
         self._auth_token = auth_token
 
         if ack_timeout is not None and ack_timeout <= 0:
             raise ValueError("timeout must be positive")
         self._ack_timeout = ack_timeout
 
-        # publics
-        self._timeout = 0
+        # properties
+        self._timeout = -1
         self.timeout = timeout
+        self._retries = -1
+        self.retries = retries
+        self._retry_delay = -1
+        self.retry_delay = retry_delay
+
+        # publics
         self.except_errors = except_errors
 
     @staticmethod
     def make_name() -> str:
         """Return a pseudo-unique string that is a legal queue identifier.
 
         This name is valid for any broker_client chosen.
@@ -97,14 +112,38 @@
     @timeout.setter
     def timeout(self, val: int) -> None:
         LOGGER.debug(f"Setting timeout to {val}")
         if val < 1:
             raise ValueError("timeout must be positive")
         self._timeout = val
 
+    @property
+    def retries(self) -> int:
+        """Get the retries value."""
+        return self._retries
+
+    @retries.setter
+    def retries(self, val: int) -> None:
+        LOGGER.debug(f"Setting retries to {val}")
+        if val < 0:
+            raise ValueError("retries must be non-negative")
+        self._retries = val
+
+    @property
+    def retry_delay(self) -> int:
+        """Get the retry_delay value."""
+        return self._retry_delay
+
+    @retry_delay.setter
+    def retry_delay(self, val: int) -> None:
+        LOGGER.debug(f"Setting retry_delay to {val}")
+        if val < 1:
+            raise ValueError("retry_delay must be positive")
+        self._retry_delay = val
+
     async def _create_pub_queue(self) -> Pub:
         """Wrap `self._broker_client.create_pub_queue()` with instance's
         config."""
         return await self._broker_client.create_pub_queue(
             self._address,
             self._name,
             self._auth_token,
@@ -148,15 +187,15 @@
 
         Returns:
             QueuePubResource -- the object to invoke `.send()` on
         """
         pub = await self._create_pub_queue()
 
         try:
-            yield QueuePubResource(pub)
+            yield QueuePubResource(pub, self.retries, self.retry_delay)
         finally:
             await pub.close()
 
     @wtt.spanned(
         these=[
             "self._broker_client",
             "self._address",
@@ -167,15 +206,19 @@
         ]
     )
     async def _safe_ack(self, sub: Sub, msg: Message) -> None:
         """Acknowledge the message."""
         # pylint:disable=protected-access
         if msg._ack_status == Message.AckStatus.NONE:
             try:
-                await sub.ack_message(msg)
+                await sub.ack_message(
+                    msg,
+                    retries=self.retries,
+                    retry_delay=self.retry_delay,
+                )
                 msg._ack_status = Message.AckStatus.ACKED  # mark after success
             except Exception as e:
                 raise AckException(f"Acking failed on broker_client: {msg}") from e
         elif msg._ack_status == Message.AckStatus.NACKED:
             raise AckException(
                 f"Message has already been nacked, it cannot be acked: {msg}"
             )
@@ -196,15 +239,19 @@
         ]
     )
     async def _safe_nack(self, sub: Sub, msg: Message) -> None:
         """Reject/nack the message."""
         # pylint:disable=protected-access
         if msg._ack_status == Message.AckStatus.NONE:
             try:
-                await sub.reject_message(msg)
+                await sub.reject_message(
+                    msg,
+                    retries=self.retries,
+                    retry_delay=self.retry_delay,
+                )
                 msg._ack_status = Message.AckStatus.NACKED  # mark after success
             except Exception as e:
                 raise NackException(f"Nacking failed on broker_client: {msg}") from e
         elif msg._ack_status == Message.AckStatus.NACKED:
             # needless, so we'll skip it
             LOGGER.debug(f"Attempted to nack an already-nacked message: {msg}")
         elif msg._ack_status == Message.AckStatus.ACKED:
@@ -311,17 +358,22 @@
         Returns:
             ManualQueueSubResource -- context manager w/ iterator function
         """
         sub = await self._create_sub_queue(prefetch_override=ack_pending_limit)
 
         try:
             yield ManualQueueSubResource(
-                lambda: sub.get_message(self.timeout * 1000),
-                lambda msg: self._safe_ack(sub, msg),
-                lambda msg: self._safe_nack(sub, msg),
+                functools.partial(
+                    sub.get_message,
+                    self.timeout * 1000,
+                    retries=self.retries,
+                    retry_delay=self.retry_delay,
+                ),
+                functools.partial(self._safe_ack, sub),
+                functools.partial(self._safe_nack, sub),
                 ack_pending_limit=sub.prefetch,
             )
         finally:
             await sub.close()
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
     @wtt.spanned(
@@ -360,15 +412,19 @@
             carrier="msg.headers",
             carrier_relation=wtt.CarrierRelation.LINK,
         )
         def add_span_link(msg: Message) -> Message:
             return msg
 
         sub = await self._create_sub_queue()
-        raw_msg = await sub.get_message(self.timeout * 1000)
+        raw_msg = await sub.get_message(
+            self.timeout * 1000,
+            retries=self.retries,
+            retry_delay=self.retry_delay,
+        )
 
         if not raw_msg:  # no message -> close and exit
             await sub.close()
             raise EmptyQueueException(
                 "No message is available (`timeout` value may be too low)"
             )
 
@@ -406,23 +462,29 @@
 class TooManyMessagesPendingAckException(Exception):
     """Raised when the ack-pending limit has been surpassed."""
 
 
 class QueuePubResource:
     """A manager class around `Pub.send_message()`."""
 
-    def __init__(self, pub: Pub):
+    def __init__(self, pub: Pub, retries: int, retry_delay: int):
         self.pub = pub
+        self.retries = retries
+        self.retry_delay = retry_delay
 
     @wtt.spanned(kind=wtt.SpanKind.PRODUCER)
     async def send(self, data: Any) -> None:
         """Send a message."""
         msg_bytes = Message.serialize(data, headers=wtt.inject_links_carrier())
         LOGGER.info(f"Sending Message: {sys.getsizeof(msg_bytes)} bytes")
-        await self.pub.send_message(msg_bytes)
+        await self.pub.send_message(
+            msg_bytes,
+            retries=self.retries,
+            retry_delay=self.retry_delay,
+        )
 
 
 class ManualQueueSubResource:
     """A manager class around `Sub.get_message()`."""
 
     def __init__(
         self,
@@ -515,14 +577,16 @@
         if self._sub and self._gen:
             raise RuntimeError("A 'QueueSubResource' instance cannot be re-entered.")
 
         self._sub = await self.queue._create_sub_queue()
         self._gen = self._sub.message_generator(
             timeout=self.queue.timeout,
             propagate_error=(not self.queue.except_errors),
+            retries=self.queue.retries,
+            retry_delay=self.queue.retry_delay,
         )
 
         self._span = wtt.get_current_span()
         self._span_carrier = wtt.inject_span_carrier()
 
         return self
```

### Comparing `oms-mqclient-2.1.1/mqclient/telemetry.py` & `oms-mqclient-2.2.0/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.2.0/oms_mqclient.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.1.1/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.2.0/oms_mqclient.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 mqclient/__init__.py
 mqclient/broker_client_interface.py
 mqclient/broker_client_manager.py
+mqclient/config.py
 mqclient/log_msgs.py
 mqclient/py.typed
 mqclient/queue.py
 mqclient/telemetry.py
 mqclient/broker_clients/__init__.py
 mqclient/broker_clients/apachepulsar.py
 mqclient/broker_clients/nats.py
 mqclient/broker_clients/rabbitmq.py
+mqclient/broker_clients/utils.py
 oms_mqclient.egg-info/PKG-INFO
 oms_mqclient.egg-info/SOURCES.txt
 oms_mqclient.egg-info/dependency_links.txt
 oms_mqclient.egg-info/requires.txt
 oms_mqclient.egg-info/top_level.txt
 tests/abstract_broker_client_tests/__init__.py
 tests/abstract_broker_client_tests/integrate_broker_client_interface.py
```

### Comparing `oms-mqclient-2.1.1/setup.cfg` & `oms-mqclient-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 from typing import Any, List, Optional
 from unittest.mock import Mock
 
 import asyncstdlib as asl
 import pytest
 from mqclient.broker_client_interface import BrokerClient, Message
+from mqclient.config import DEFAULT_RETRIES, DEFAULT_RETRY_DELAY, DEFAULT_TIMEOUT
 from mqclient.queue import Queue
 
 from .utils import is_inst_name
 
 
 class BrokerClientUnitTest:
     """Unit test suite interface for specified broker_client."""
@@ -81,28 +82,36 @@
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 1, "", None
         )
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
-        await sub.ack_message(Message(12, b""))
+        await sub.ack_message(
+            Message(12, b""),
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         self._get_ack_mock_fn(mock_con).assert_called_with(12)
 
     @pytest.mark.asyncio
     async def test_reject_message(self, mock_con: Any, queue_name: str) -> None:
         """Test rejecting message."""
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 1, "", None
         )
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
-        await sub.reject_message(Message(12, b""))
+        await sub.reject_message(
+            Message(12, b""),
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         self._get_nack_mock_fn(mock_con).assert_called_with(12)
 
     @pytest.mark.asyncio
     async def test_message_generator_00(self, mock_con: Any, queue_name: str) -> None:
         """Test message generator."""
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 1, "", None
@@ -115,15 +124,22 @@
         num_msgs = 100
 
         fake_data = ["baz-{i}".encode("utf-8") for i in range(num_msgs)]
         fake_ids = [i * 10 for i in range(num_msgs)]
         await self._enqueue_mock_messages(mock_con, fake_data, fake_ids)
 
         msg: Optional[Message]
-        async for i, msg in asl.enumerate(sub.message_generator()):
+        async for i, msg in asl.enumerate(
+            sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=True,
+                retries=DEFAULT_RETRIES,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            )
+        ):
             logging.debug(i)
             if i > 0:  # see if previous msg was acked
                 # prev_id = (i - 1) * 10
                 # would be called by Queue
                 self._get_ack_mock_fn(mock_con).assert_not_called()
             assert msg is not None
             assert msg.msg_id == fake_ids[i]
@@ -149,15 +165,22 @@
         fake_ids = [12, 20]
         await self._enqueue_mock_messages(
             mock_con, fake_data, fake_ids, append_none=False
         )
 
         m = None
         msg: Optional[Message]
-        async for i, msg in asl.enumerate(sub.message_generator()):
+        async for i, msg in asl.enumerate(
+            sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=True,
+                retries=DEFAULT_RETRIES,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            )
+        ):
             m = msg
             if i == 0:
                 break
 
         assert m is not None
         assert m.msg_id == 12
         assert m.payload == b"foo, bar"
@@ -176,15 +199,22 @@
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         await self._enqueue_mock_messages(mock_con, [b"foo, bar"], [12])
 
         m = None
         msg: Optional[Message]
-        async for i, msg in asl.enumerate(sub.message_generator()):
+        async for i, msg in asl.enumerate(
+            sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=True,
+                retries=DEFAULT_RETRIES,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            )
+        ):
             assert i < 1
             m = msg
         assert m is not None
         assert m.msg_id == 12
         assert m.payload == b"foo, bar"
         self._get_ack_mock_fn(mock_con).assert_not_called()  # would be called by Queue
         # would be called by Queue
@@ -217,15 +247,20 @@
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         fake_data = [b"baz-0", b"baz-1", b"baz-2"]
         fake_ids = [0, 1, 2]
         await self._enqueue_mock_messages(mock_con, fake_data, fake_ids)
 
-        gen = sub.message_generator()
+        gen = sub.message_generator(
+            timeout=DEFAULT_TIMEOUT,
+            propagate_error=True,
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         i = 0
         async for msg in gen:
             logging.debug(i)
             if i > 0:  # see if previous msg was acked
                 # would be called by Queue
                 self._get_ack_mock_fn(mock_con).assert_not_called()
 
@@ -254,15 +289,20 @@
 
         fake_data = [b"baz-0", b"baz-1", b"baz-2"]
         fake_ids = [0, 1, 2]
         await self._enqueue_mock_messages(
             mock_con, fake_data, fake_ids, append_none=False
         )
 
-        gen = sub.message_generator()  # propagate_error=True
+        gen = sub.message_generator(
+            timeout=DEFAULT_TIMEOUT,
+            propagate_error=True,
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )  # propagate_error=True
         i = 0
         async for msg in gen:
             logging.debug(i)
             assert i < 3
             if i > 0:  # see if previous msg was acked
                 # would be called by Queue
                 self._get_ack_mock_fn(mock_con).assert_not_called()
@@ -302,15 +342,20 @@
         if num_msgs % 2 == 0:
             raise RuntimeError("`num_msgs` must be odd, so last message is nacked")
 
         fake_data = [f"baz-{i}".encode("utf-8") for i in range(num_msgs)]
         fake_ids = [i * 10 for i in range(num_msgs)]
         await self._enqueue_mock_messages(mock_con, fake_data, fake_ids)
 
-        gen = sub.message_generator(propagate_error=False)
+        gen = sub.message_generator(
+            timeout=DEFAULT_TIMEOUT,
+            propagate_error=False,
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         i = 0
         async for msg in gen:
             logging.debug(i)
 
             assert msg is not None
             assert msg.msg_id == i * 10
             assert msg.payload == fake_data[i]
@@ -342,15 +387,20 @@
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         await self._enqueue_mock_messages(mock_con, [b"baz"], [0], append_none=False)
 
         excepted = False
         try:
-            async for msg in sub.message_generator(propagate_error=False):
+            async for msg in sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=False,
+                retries=DEFAULT_RETRIES,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            ):
                 logging.debug(msg)
                 raise Exception
         except Exception:
             excepted = True  # QueueSubResource would've suppressed the Exception
         assert excepted
 
         # would be called by Queue
```

### Comparing `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/integrate/conftest.py` & `oms-mqclient-2.2.0/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/integrate/test_nats.py` & `oms-mqclient-2.2.0/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/integrate/test_pulsar.py` & `oms-mqclient-2.2.0/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.2.0/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.1/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.2.0/tests/unit/pulsar/test_pulsar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Unit Tests for Pulsar BrokerClient."""
 
 from typing import Any, List
 
 import pytest
 from mqclient import broker_client_manager
 from mqclient.broker_client_interface import Message
+from mqclient.config import (
+    DEFAULT_RETRIES,
+    DEFAULT_RETRY_DELAY,
+    DEFAULT_TIMEOUT,
+    DEFAULT_TIMEOUT_MILLIS,
+)
 
 from ...abstract_broker_client_tests.unit_tests import BrokerClientUnitTest
 
 
 class TestUnitApachePulsar(BrokerClientUnitTest):
     """Unit test suite interface for Apache Pulsar broker_client."""
 
@@ -66,15 +72,19 @@
 
     @pytest.mark.asyncio
     async def test_send_message(self, mock_con: Any, queue_name: str) -> None:
         """Test sending message."""
         pub = await self.broker_client.create_pub_queue(
             "localhost", queue_name, "", None
         )
-        await pub.send_message(b"foo, bar, baz")
+        await pub.send_message(
+            b"foo, bar, baz",
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         mock_con.return_value.create_producer.return_value.send.assert_called_with(
             b"foo, bar, baz"
         )
 
     @pytest.mark.asyncio
     async def test_get_message(self, mock_con: Any, queue_name: str) -> None:
         """Test getting message."""
@@ -83,15 +93,19 @@
         )
         mock_con.return_value.subscribe.return_value.receive.return_value.data.return_value = Message.serialize(
             "foo, bar"
         )
         mock_con.return_value.subscribe.return_value.receive.return_value.message_id.return_value = (
             12
         )
-        m = await sub.get_message()
+        m = await sub.get_message(
+            timeout_millis=DEFAULT_TIMEOUT_MILLIS,
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
 
         assert m is not None
         assert m.msg_id == 12
         assert m.data == "foo, bar"
 
     @pytest.mark.asyncio
     async def test_message_generator_10_upstream_error(
@@ -102,19 +116,43 @@
         Generator should raise Exception originating upstream (a.k.a.
         from pulsar-package code).
         """
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 1, "", None
         )
 
-        mock_con.return_value.subscribe.return_value.receive.side_effect = Exception()
-        with pytest.raises(Exception):
-            _ = [m async for m in sub.message_generator()]
-        # would be called by Queue
-        self._get_close_mock_fn(mock_con).assert_not_called()
+        retries = 2  # >= 0
+
+        class _MyException(Exception):
+            pass
+
+        mock_con.return_value.subscribe.return_value.receive.side_effect = (
+            _MyException()
+        )
+        with pytest.raises(_MyException):
+            async for m in sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=True,
+                retries=retries,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            ):
+                pass
+        # would be called by Queue one more time
+        assert self._get_close_mock_fn(mock_con).call_count == retries
+
+        # reset for next call
+        self._get_close_mock_fn(mock_con).reset_mock()
 
         # `propagate_error` attribute has no affect (b/c it deals w/ *downstream* errors)
-        mock_con.return_value.subscribe.return_value.receive.side_effect = Exception()
-        with pytest.raises(Exception):
-            _ = [m async for m in sub.message_generator(propagate_error=False)]
-        # would be called by Queue
-        self._get_close_mock_fn(mock_con).assert_not_called()
+        mock_con.return_value.subscribe.return_value.receive.side_effect = (
+            _MyException()
+        )
+        with pytest.raises(_MyException):
+            async for m in sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=False,
+                retries=retries,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            ):
+                pass
+        # would be called by Queue one more time
+        assert self._get_close_mock_fn(mock_con).call_count == retries
```

### Comparing `oms-mqclient-2.1.1/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.2.0/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Unit Tests for RabbitMQ/Pika BrokerClient."""
 
 import itertools
-import unittest
 from typing import Any, List, Optional, Tuple
 from unittest.mock import MagicMock
 
 import pika  # type: ignore[import]
 import pytest
 from mqclient import broker_client_manager
 from mqclient.broker_client_interface import Message
 from mqclient.broker_clients.rabbitmq import HUMAN_PATTERN, _get_credentials, _parse_url
+from mqclient.config import (
+    DEFAULT_RETRIES,
+    DEFAULT_RETRY_DELAY,
+    DEFAULT_TIMEOUT,
+    DEFAULT_TIMEOUT_MILLIS,
+)
 
 from ...abstract_broker_client_tests.unit_tests import BrokerClientUnitTest
 
 
 class TestUnitRabbitMQ(BrokerClientUnitTest):
     """Unit test suite interface for RabbitMQ broker_client."""
 
@@ -41,15 +46,17 @@
     ) -> None:
         """Place messages on the mock queue."""
         if len(data) != len(ids):
             raise AttributeError("`data` and `ids` must have the same length.")
         messages = [(MagicMock(delivery_tag=i), None, d) for d, i in zip(data, ids)]
         if append_none:
             messages += [(None, None, None)]  # type: ignore
-        mock_con.return_value.channel.return_value.consume.return_value = messages
+        mock_con.return_value.channel.return_value.consume.return_value.__next__.side_effect = (
+            messages
+        )
 
     @pytest.mark.asyncio
     async def test_create_pub_queue(self, mock_con: Any, queue_name: str) -> None:
         """Test creating pub queue."""
         pub = await self.broker_client.create_pub_queue(
             "localhost", queue_name, "", None
         )
@@ -59,39 +66,49 @@
     @pytest.mark.asyncio
     async def test_create_sub_queue(self, mock_con: Any, queue_name: str) -> None:
         """Test creating sub queue."""
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 213, "", None
         )
         assert sub.queue == queue_name  # type: ignore
-        assert sub.prefetch == 213  # type: ignore
+        assert sub.prefetch == 213
         mock_con.return_value.channel.assert_called()
 
     @pytest.mark.asyncio
     async def test_send_message(self, mock_con: Any, queue_name: str) -> None:
         """Test sending message."""
         pub = await self.broker_client.create_pub_queue(
             "localhost", queue_name, "", None
         )
-        await pub.send_message(b"foo, bar, baz")
+        await pub.send_message(
+            b"foo, bar, baz",
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         mock_con.return_value.channel.return_value.basic_publish.assert_called_with(
             exchange="", routing_key=queue_name, body=b"foo, bar, baz"
         )
 
     @pytest.mark.asyncio
     async def test_get_message(self, mock_con: Any, queue_name: str) -> None:
         """Test getting message."""
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 1, "", None
         )
         mock_con.return_value.is_closed = False  # HACK - manually set attr
 
         fake_message = (MagicMock(delivery_tag=12), None, Message.serialize("foo, bar"))
-        mock_con.return_value.channel.return_value.consume.return_value = [fake_message]
-        m = await sub.get_message()
+        mock_con.return_value.channel.return_value.consume.return_value.__next__.side_effect = [
+            fake_message
+        ]
+        m = await sub.get_message(
+            timeout_millis=DEFAULT_TIMEOUT_MILLIS,
+            retries=DEFAULT_RETRIES,
+            retry_delay=DEFAULT_RETRY_DELAY,
+        )
         assert m is not None
         assert m.msg_id == 12
         assert m.data == "foo, bar"
 
     @pytest.mark.asyncio
     async def test_message_generator_10_upstream_error(
         self, mock_con: Any, queue_name: str
@@ -102,28 +119,52 @@
         from pika-package code).
         """
         sub = await self.broker_client.create_sub_queue(
             "localhost", queue_name, 1, "", None
         )
         mock_con.return_value.is_closed = False  # HACK - manually set attr
 
-        err_msg = (unittest.mock.ANY, None, b"foo, bar")
-        mock_con.return_value.channel.return_value.consume.return_value = [err_msg]
-        with pytest.raises(Exception):
-            _ = [m async for m in sub.message_generator()]
-        # would be called by Queue
-        self._get_close_mock_fn(mock_con).assert_not_called()
+        retries = 2  # >= 0
+
+        class _MyException(Exception):
+            pass
+
+        mock_con.return_value.channel.return_value.consume.return_value.__next__.side_effect = (
+            _MyException
+        )
+        with pytest.raises(_MyException):
+            async for m in sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=True,
+                retries=retries,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            ):
+                pass
+
+        # would be called by Queue one more time
+        assert self._get_close_mock_fn(mock_con).call_count == retries
+
+        # reset for next call
+        self._get_close_mock_fn(mock_con).reset_mock()
 
         # `propagate_error` attribute has no affect (b/c it deals w/ *downstream* errors)
-        err_msg = (unittest.mock.ANY, None, b"foo, bar")
-        mock_con.return_value.channel.return_value.consume.return_value = [err_msg]
-        with pytest.raises(Exception):
-            _ = [m async for m in sub.message_generator(propagate_error=False)]
-        # would be called by Queue
-        self._get_close_mock_fn(mock_con).assert_not_called()
+        mock_con.return_value.channel.return_value.consume.return_value.__next__.side_effect = (
+            _MyException
+        )
+        with pytest.raises(_MyException):
+            async for m in sub.message_generator(
+                timeout=DEFAULT_TIMEOUT,
+                propagate_error=False,
+                retries=retries,
+                retry_delay=DEFAULT_RETRY_DELAY,
+            ):
+                pass
+
+        # would be called by Queue one more time
+        assert self._get_close_mock_fn(mock_con).call_count == retries
 
 
 class TestUnitRabbitMQHelpers:
     """Unit test rabbitmq-specific helper functions."""
 
     def test_000(self) -> None:
         """Sanity check the constants."""
```

