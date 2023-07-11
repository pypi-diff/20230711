# Comparing `tmp/kade_drive-0.5.1.tar.gz` & `tmp/kade_drive-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kade_drive-0.5.1.tar", max compression
+gzip compressed data, was "kade_drive-0.7.0.tar", max compression
```

## Comparing `kade_drive-0.5.1.tar` & `kade_drive-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.5.1/LICENSE
--rw-r--r--   0        0        0      778 2023-07-06 05:54:09.008851 kade_drive-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.5.1/kade_drive/__init__.py
--rw-r--r--   0        0        0     1426 2023-07-06 05:42:11.364669 kade_drive-0.5.1/kade_drive/cli.py
--rw-r--r--   0        0        0     7392 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/client.py
--rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.5.1/kade_drive/core/__init__.py
--rw-r--r--   0        0        0      130 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/core/config.py
--rw-r--r--   0        0        0     9533 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/core/crawling.py
--rw-r--r--   0        0        0    18641 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/core/network.py
--rw-r--r--   0        0        0     3916 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/node.py
--rw-r--r--   0        0        0     7846 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/protocol.py
--rw-r--r--   0        0        0     8680 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/routing.py
--rw-r--r--   0        0        0     8928 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/storage.py
--rw-r--r--   0        0        0     1486 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 21:17:07.162141 kade_drive-0.5.1/kade_drive/message_system/__init__.py
--rw-r--r--   0        0        0     6617 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/message_system/message_system.py
--rw-r--r--   0        0        0     2619 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/server.py
--rw-r--r--   0        0        0      702 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/test_store_file.py
--rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.5.1/kade_drive/tests/__init__.py
--rw-r--r--   0        0        0     1698 2023-07-06 00:27:01.589732 kade_drive-0.5.1/kade_drive/tests/conftest.py
--rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.5.1/kade_drive/tests/data_to_split.txt
--rw-r--r--   0        0        0     1785 2023-07-06 00:26:57.630729 kade_drive-0.5.1/kade_drive/tests/test_node.py
--rw-r--r--   0        0        0     4631 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/tests/test_routing.py
--rw-r--r--   0        0        0        1 2023-07-06 00:26:51.787726 kade_drive-0.5.1/kade_drive/tests/test_server.py
--rw-r--r--   0        0        0      757 2023-07-06 00:47:02.811454 kade_drive-0.5.1/kade_drive/tests/test_splitdata.py
--rw-r--r--   0        0        0     1459 2023-07-06 00:47:02.811454 kade_drive-0.5.1/kade_drive/tests/test_storage.py
--rw-r--r--   0        0        0      716 2023-07-06 00:47:02.811454 kade_drive-0.5.1/kade_drive/tests/test_utils.py
--rw-r--r--   0        0        0      515 2023-07-07 06:01:44.822501 kade_drive-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 kade_drive-0.5.1/setup.py
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 kade_drive-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2165 2023-07-10 05:18:08.765855 kade_drive-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.7.0/kade_drive/__init__.py
+-rw-r--r--   0        0        0     1907 2023-07-11 18:08:36.988438 kade_drive-0.7.0/kade_drive/cli.py
+-rw-r--r--   0        0        0     8974 2023-07-11 18:36:40.105435 kade_drive-0.7.0/kade_drive/client.py
+-rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.7.0/kade_drive/core/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-06 00:47:02.809455 kade_drive-0.7.0/kade_drive/core/config.py
+-rw-r--r--   0        0        0     9561 2023-07-09 15:55:04.310834 kade_drive-0.7.0/kade_drive/core/crawling.py
+-rw-r--r--   0        0        0    20831 2023-07-11 19:05:31.237835 kade_drive-0.7.0/kade_drive/core/network.py
+-rw-r--r--   0        0        0     3915 2023-07-09 01:01:28.935150 kade_drive-0.7.0/kade_drive/core/node.py
+-rw-r--r--   0        0        0     8752 2023-07-11 18:36:40.105435 kade_drive-0.7.0/kade_drive/core/protocol.py
+-rw-r--r--   0        0        0     8819 2023-07-11 18:36:40.105435 kade_drive-0.7.0/kade_drive/core/routing.py
+-rw-r--r--   0        0        0     9825 2023-07-11 18:37:58.242000 kade_drive-0.7.0/kade_drive/core/storage.py
+-rw-r--r--   0        0        0     1319 2023-07-09 17:55:02.693868 kade_drive-0.7.0/kade_drive/core/utils.py
+-rw-r--r--   0        0        0     2778 2023-07-11 18:36:40.106435 kade_drive-0.7.0/kade_drive/server.py
+-rw-r--r--   0        0        0      769 2023-07-10 04:35:06.243561 kade_drive-0.7.0/kade_drive/test_store_file.py
+-rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.7.0/kade_drive/tests/__init__.py
+-rw-r--r--   0        0        0     1731 2023-07-07 20:16:46.224385 kade_drive-0.7.0/kade_drive/tests/conftest.py
+-rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.7.0/kade_drive/tests/data_to_split.txt
+-rw-r--r--   0        0        0     1796 2023-07-07 20:16:46.223385 kade_drive-0.7.0/kade_drive/tests/test_node.py
+-rw-r--r--   0        0        0     4642 2023-07-07 20:16:46.181385 kade_drive-0.7.0/kade_drive/tests/test_routing.py
+-rw-r--r--   0        0        0        1 2023-07-06 00:26:51.787726 kade_drive-0.7.0/kade_drive/tests/test_server.py
+-rw-r--r--   0        0        0      768 2023-07-07 20:16:46.129384 kade_drive-0.7.0/kade_drive/tests/test_splitdata.py
+-rw-r--r--   0        0        0     1459 2023-07-06 00:47:02.811454 kade_drive-0.7.0/kade_drive/tests/test_storage.py
+-rw-r--r--   0        0        0      727 2023-07-07 20:16:46.129384 kade_drive-0.7.0/kade_drive/tests/test_utils.py
+-rw-r--r--   0        0        0      760 2023-07-11 19:31:22.383949 kade_drive-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 kade_drive-0.7.0/setup.py
+-rw-r--r--   0        0        0     2739 1970-01-01 00:00:00.000000 kade_drive-0.7.0/PKG-INFO
```

### Comparing `kade_drive-0.5.1/LICENSE` & `kade_drive-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.1/kade_drive/client.py` & `kade_drive-0.7.0/kade_drive/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import pickle
 import rpyc
 from time import sleep
 from rpyc.core.protocol import PingError
-from message_system.message_system import Message_System
+from message_system.message_system import MessageSystem
 
 import logging
 
-
 try:
     logger = logging.getLogger(__name__)
 except:
     pass
 
 
 class ClientSession:
     """
     Class to handle connection to the distributed file system
     It is necessary to run ensure_connection or broadcast method before
     accessing to the other functionality
     """
 
     def __init__(
-        self, bootstrap_nodes: list[tuple[str, int]], log_level=logging.INFO
+        self, bootstrap_nodes: list[tuple[str, int]], log_level=logging.DEBUG
     ) -> None:
         logging.basicConfig(
             level=log_level,
             format="%(asctime)s  - %(name)s - %(levelname)s - %(message)s",
         )
         logging.getLogger(__name__)
         self.connection: rpyc.Connection | None = None
@@ -33,15 +32,15 @@
 
     def connect(
         self,
         time_to_reconnect=5,
         use_broadcast_if_needed: bool = False,
         update_boostrap_nodes: bool = True,
         attempts_to_reconnect=2,
-    ):
+    ) -> bool:
         self.connection, self.bootstrap_nodes = self._ensure_connection(
             self.bootstrap_nodes,
             self.connection,
             time_to_reconnect,
             use_broadcast_if_needed,
             update_boostrap_nodes,
             attempts_to_reconnect,
@@ -117,87 +116,128 @@
         if remaining_attempts_to_reconnect > 0:
             remaining_attempts_to_reconnect -= 1
             print(
                 f"Trying to reconnect to {ip} in {time_to_reconnect} seconds... attempts left: {remaining_attempts_to_reconnect}"
             )
             sleep(time_to_reconnect)
         else:
-            print(f"Connection to {ip} failed, removing from bootstrap nodes list.")
+            print(
+                f"Connection to {ip} failed, removing from bootstrap nodes list.")
             nodes_to_try.pop(0)
             return nodes_to_try, total_attempts_to_reconnect
 
         return nodes_to_try, remaining_attempts_to_reconnect
 
-    def get(self, key, apply_hash_to_key=True):
+    def get(self, key, apply_hash_to_key=True) -> tuple:
         if not self.connection:
             logger.error("No connection stablished to do get")
-            return None
-        metadata_list = self.connection.root.get(key, apply_hash_to_key)
+            return None, None
+
+        try:
+            metadata_list = self.connection.root.get(key, apply_hash_to_key)
+        except EOFError as e:
+            logger.error(
+                f"Connection lost in get when doing get rpc, exception: {e}")
+            return None, None
         logger.debug(f"METADATAAAAA {metadata_list}")
         if metadata_list:
-            logger.debug(f"metadata_list received {str(len(metadata_list) > 0)}")
+            logger.debug(
+                f"metadata_list received {str(len(metadata_list) > 0)}")
         data_received = []
 
         if metadata_list is None or len(metadata_list) == 0:
             logger.debug(f"No data with key {key}")
-            return None
+            return None, self.connection
 
         for chunk_key in metadata_list:
-            locations: list[
-                tuple[str, int]
-            ] = self.connection.root.get_file_chunk_location(chunk_key)
-            logger.debug(f"locations for chunk_key {chunk_key} are {locations}")
+            try:
+                locations: list[
+                    tuple[str, int]
+                ] = self.connection.root.get_file_chunk_location(chunk_key)
+            except EOFError as e:
+                logger.error(
+                    f"Connection lost in get when doing get_file_chunk_location, exception: {e}"
+                )
+                return None, None
+            logger.debug(
+                f"locations for chunk_key {chunk_key} are {locations}")
             if self.bootstrap_nodes[0] in locations:
                 logger.debug("Using primary connection to get chunk")
-                data_received.append(
-                    self.connection.root.rpc_get_file_chunk_value(chunk_key)
-                )
+                try:
+                    data_received.append(
+                        self.connection.root.rpc_get_file_chunk_value(
+                            chunk_key)
+                    )
+                except EOFError as e:
+                    logger.error(
+                        f"Connection lost in get when doing rpc_get_file_chunk_value, exception: {e}"
+                    )
+                    return None, None
             else:
                 conn, _ = self._ensure_connection(
                     locations,
                     None,
                     use_broadcast_if_needed=False,
                     update_boostrap_nodes=False,
                 )
                 if conn:
-                    data_received.append(conn.root.rpc_get_file_chunk_value(chunk_key))
+                    try:
+                        data_received.append(
+                            conn.root.rpc_get_file_chunk_value(chunk_key)
+                        )
+                    except EOFError as e:
+                        logger.error(
+                            f"Connection lost in get when doing rpc_get_file_chunk_value, exception: {e}"
+                        )
+                        return None, None
                 else:
                     logger.warning("No Servers to get chunk")
 
         logger.debug(f"len data received {len(data_received)}")
         data_received = b"".join(data_received)
         try:
             data_to_return = pickle.loads(data_received)
-            return data_to_return
+            return data_to_return, self.connection
         except pickle.UnpicklingError as e:
             logger.error(e)
-            return None
+            return None, self.connection
 
-    def put(self, key, value: bytes, apply_hash_to_key=True):
+    def put(self, key, value: bytes, apply_hash_to_key=True) -> tuple:
         if self.connection:
-            self.connection.root.upload_file(
-                key=key, data=value, apply_hash_to_key=apply_hash_to_key
-            )
-            sleep(1)
-            logger.info("put > Success")
+            try:
+                self.connection.root.upload_file(
+                    key=key, data=value, apply_hash_to_key=apply_hash_to_key
+                )
+                sleep(1)
+                logger.info("put > Success")
+                return True, self.connection
+            except EOFError as e:
+                logger.error(f"Connection lost in put, exception: {e}")
+
         else:
             logger.error("No connection stablished to do put")
 
+        return False, None
+
     def _update_bootstrap_nodes(self, connection: rpyc.Connection):
-        nodes_to_add = [
-            node
-            for node in connection.root.find_neighbors()
-            if node not in self.bootstrap_nodes
-        ]
-        self.bootstrap_nodes.extend(nodes_to_add)
-        logger.debug(f"Neighbors {self.bootstrap_nodes}")
+        try:
+            nodes_to_add = [
+                node
+                for node in connection.root.find_neighbors()
+                if node not in self.bootstrap_nodes
+            ]
+            self.bootstrap_nodes.extend(nodes_to_add)
+            logger.debug(f"Neighbors {self.bootstrap_nodes}")
+        except EOFError as e:
+            logger.error(
+                f"Connection lost in _update_bootstrap_nodes, exception: {e}")
 
     def broadcast(self) -> bool:
         print("Listening broadcasts")
-        ms = Message_System()
+        ms = MessageSystem()
         try:
             ip, port = ms.receive(service_name="dfs").split(" ")
             print(ip, port)
         except ValueError:
             ip = None
             port = None
         if ip:
```

### Comparing `kade_drive-0.5.1/kade_drive/core/crawling.py` & `kade_drive-0.7.0/kade_drive/core/crawling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections import Counter
 import logging
 import rpyc
-from core.node import Node, NodeHeap
-from core.protocol import FileSystemProtocol, ServerSession
+from kade_drive.core.node import Node, NodeHeap
+from kade_drive.core.protocol import FileSystemProtocol, ServerSession
 
 
 # Create a file handler
-file_handler = logging.FileHandler("log_file.log")
+# file_handler = logging.FileHandler("log_file.log")
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
-file_handler.setFormatter(formatter)
+# file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
+# logger.addHandler(file_handler)
 
 
 class SpiderCrawl:
     """
     Crawl the network and look for given 160-bit keys.
     """
```

### Comparing `kade_drive-0.5.1/kade_drive/core/network.py` & `kade_drive-0.7.0/kade_drive/core/network.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 import logging
 from rpyc import Service
 import threading
 from time import sleep
 import rpyc
 import pickle
 from rpyc.utils.server import ThreadedServer
-from core.config import Config
-from core.protocol import FileSystemProtocol, ServerSession
-from core.routing import RoutingTable
-from core.utils import digest
-from core.storage import PersistentStorage
-from core.node import Node
-from core.crawling import ChunkLocationSpiderCrawl, ValueSpiderCrawl
-from core.crawling import NodeSpiderCrawl
+from kade_drive.core.config import Config
+from kade_drive.core.protocol import FileSystemProtocol, ServerSession
+from kade_drive.core.routing import RoutingTable
+from kade_drive.core.utils import digest
+from kade_drive.core.storage import PersistentStorage
+from kade_drive.core.node import Node
+from kade_drive.core.crawling import ChunkLocationSpiderCrawl, ValueSpiderCrawl
+from kade_drive.core.crawling import NodeSpiderCrawl
+from kade_drive.core.utils import is_port_in_use
 
 # from models.file import File
 
 # Create a file handler
-file_handler = logging.FileHandler("log_file.log")
+# file_handler = logging.FileHandler("log_file.log")
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
-file_handler.setFormatter(formatter)
+# file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
+# logger.addHandler(file_handler)
 
 
 class Server:
     ksize: int
     alpha: int
     storage: PersistentStorage
     node: Node
@@ -49,15 +50,18 @@
         Args:
             ksize (int): Replication factor, determines to how many closest peers a record is replicated
             alpha (int): concurrency parameter, determines how many parallel asynchronous FIND_NODE RPC send
             node_id: The id for this node on the network.
             storage: An instance that implements the interface
                      :class:`~kademlia.storage.PersistenceStorage`
         """
+        while is_port_in_use(ip, port):
+            port += 1
 
+        logging.getLogger(f"SERVER/{port}").setLevel(logging.CRITICAL + 1)
         Server.ksize = ksize
         Server.alpha = alpha
         Server.storage = storage or PersistentStorage(config.ttl)
         Server.node = Node(
             node_id or digest(random.getrandbits(255)), ip=ip, port=str(port)
         )
         logger.debug(f"NODE ID: {Server.node.id}")
@@ -73,54 +77,62 @@
     @staticmethod
     def listen(port, interface="0.0.0.0"):
         """
         Start listening on the given port.
 
         Provide interface="::" to accept ipv6 address
         """
-        print(interface, port)
-        Server.node.ip = interface
-        Server.node.port = port
-        t = ThreadedServer(
-            ServerService,
-            port=port,
-            hostname=interface,
-            protocol_config={"allow_public_attrs": True, "allow_pickle": True},
-        )
-        t.start()
+        while True:
+            try:
+                print(interface, port)
+                Server.node.ip = interface
+                Server.node.port = port
+                t = ThreadedServer(
+                    ServerService,
+                    port=port,
+                    hostname=interface,
+                    protocol_config={
+                        "allow_public_attrs": True, "allow_pickle": True},
+                )
+                t.start()
+            except Exception as e:
+                logger.critical(f"Server Listen failed: {e}")
 
     @staticmethod
     def bootstrap(addrs: list[tuple[str, str]]):
         """
         Bootstrap the server by connecting to other known nodes in the network.
 
         Args:
             addrs: A `list` of (ip, port) `tuple` pairs.  Note that only IP
                    addresses are acceptable - hostnames will cause an error.
         """
 
-        logger.debug(f"Attempting to bootstrap node with {len(addrs)} initial contacts")
+        logger.debug(
+            f"Attempting to bootstrap node with {len(addrs)} initial contacts")
         cos = list(map(Server.bootstrap_node, addrs))
         nodes = [node for node in cos if node is not None]
-        spider = NodeSpiderCrawl(Server.node, nodes, Server.ksize, Server.alpha)
+        spider = NodeSpiderCrawl(
+            Server.node, nodes, Server.ksize, Server.alpha)
         res = spider.find()
         logger.debug("results of spider find: %s", res)
 
         return res
 
     @staticmethod
     def bootstrap_node(addr: tuple[str, str]):
         response = None
         with ServerSession(addr[0], addr[1]) as conn:
             if conn:
                 response = conn.rpc_ping(
                     (Server.node.ip, Server.node.port), Server.node.id
                 )
                 node = Node(response, addr[0], addr[1]) if response else None
-                response = FileSystemProtocol.process_response(conn, response, node)
+                response = FileSystemProtocol.process_response(
+                    conn, response, node)
 
                 return node
 
     @staticmethod
     def split_data(data: bytes, chunk_size: int):
         """Split data into chunks of less than chunk_size, it must be less than 16mb"""
         if not isinstance(data, bytes):
@@ -134,60 +146,74 @@
         count = 0
         last_position = 0
         while not (fixed_chunks == count):
             if count == 0:
                 chunks.append(data[0:chunk_size])
                 last_position = chunk_size
             else:
-                chunks.append(data[last_position : last_position + chunk_size])
+                chunks.append(data[last_position: last_position + chunk_size])
                 last_position = last_position + chunk_size
             count += 1
         return chunks
 
     @staticmethod
-    def set_digest(dkey: bytes, value, metadata=True):
+    def _handle_empty_neighbors(dkey, metadata, value, exclude_current):
+        logger.debug("There are no known neighbors to set key %s", dkey.hex())
+
+        if not exclude_current:
+            logger.info("storing in current server")
+            if metadata:
+                Server.storage.set_metadata(dkey, value, False)
+            else:
+                Server.storage.set_value(dkey, value, False)
+
+        return True
+
+    @staticmethod
+    def set_digest(
+        dkey: bytes, value, metadata=True, exclude_current=False, local_last_write=None
+    ):
         """
         Set the given SHA1 digest key (bytes) to the given value in the
         network.
         """
 
         node = Node(dkey)
         assert node is not None
         nearest = FileSystemProtocol.router.find_neighbors(node)
-        if not nearest:
-            logger.warning("There are no known neighbors to set key %s", dkey.hex())
-
-            if not Server.storage.contains(dkey):
-                logger.info("storing in current server")
-                if metadata:
-                    Server.storage.set_metadata(dkey, value, False)
-                else:
-                    Server.storage.set_value(dkey, value, False)
-
-            return True
+        logger.info(f"nearest in set_digest is {nearest}")
 
+        if not nearest or len(nearest) == 0:
+            return Server._handle_empty_neighbors(dkey, metadata, value, exclude_current)
         spider = NodeSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
         nodes = spider.find()
         logger.debug("setting '%s' on %s", dkey, list(map(str, nodes)))
 
+        if not nodes or len(nodes) == 0:
+            return Server._handle_empty_neighbors(dkey, metadata, value, exclude_current)
+        
         # if this node is close too, then store here as well
         biggest = max([n.distance_to(node) for n in nodes])
-        if Server.node.distance_to(node) < biggest:
-            if Server.storage.contains(dkey, metadata):
-                if metadata:
-                    Server.storage.set_metadata(dkey, value, False)
-                else:
-                    Server.storage.set_value(dkey, value, False)
+        if Server.node.distance_to(node) < biggest and not exclude_current:
+            if metadata:
+                Server.storage.set_metadata(dkey, value, False)
+            else:
+                Server.storage.set_value(dkey, value, False)
 
         any_result = False
         for n in nodes:
             address = (n.ip, n.port)
             with ServerSession(address[0], address[1]) as conn:
-                contains = FileSystemProtocol.call_contains(conn, n, dkey, metadata)
-                if not contains:
+                response = FileSystemProtocol.call_check_if_new_value_exists(
+                    conn, n, dkey
+                )
+                contains, date = None, None
+                if response is not None:
+                    contains, date = response
+                if local_last_write is None or date is None or date < local_last_write:
                     result = FileSystemProtocol.call_store(
                         conn, n, dkey, value, metadata
                     )
                     if result:
                         any_result = True
 
                 if contains:
@@ -197,82 +223,199 @@
         return any_result
 
     @staticmethod
     def find_replicas():
         nearest = FileSystemProtocol.router.find_neighbors(
             Server.node, Server.alpha, exclude=Server.node
         )
-        spider = NodeSpiderCrawl(Server.node, nearest, Server.ksize, Server.alpha)
+        spider = NodeSpiderCrawl(Server.node, nearest,
+                                 Server.ksize, Server.alpha)
 
         nodes = spider.find()
 
         keys_to_find = Server.storage.keys()
         keys_dict = {}
         for n in nodes:
             with ServerSession(n.ip, n.port) as conn:
                 for k, is_metadata in keys_to_find:
-                    contains = FileSystemProtocol.call_contains(conn, n, k, is_metadata)
+                    contains = FileSystemProtocol.call_contains(
+                        conn, n, k, is_metadata)
                     if contains:
                         if (k, is_metadata) not in keys_dict:
                             keys_dict[(k, is_metadata)] = 0
                         keys_dict[(k, is_metadata)] += 1
 
         return_list = []
         for k in keys_dict:
             logger.debug(k)
             if keys_dict[k] < Server.ksize:
                 return_list.append(k)
         return return_list
 
     @staticmethod
     def _refresh_table(refresh_sleep):
-        """
-        Refresh buckets that haven't had any lookups in the last hour
-        (per section 2.3 of the paper).
-        """
-
         while True:
             try:
                 sleep(refresh_sleep)
                 logger.info("Refreshing Table")
 
                 results = []
                 for node_id in FileSystemProtocol.get_refresh_ids():
                     node = Node(node_id)
                     nearest = FileSystemProtocol.router.find_neighbors(
                         node, Server.alpha
                     )
-                    spider = NodeSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
+                    spider = NodeSpiderCrawl(
+                        node, nearest, Server.ksize, Server.alpha)
 
                     results.append(spider.find())
 
-                # do our crawling
+                # Republishing keys to mantain the network updated
+
                 logger.debug("Republishing old keys")
-                for key, value, is_metadata in Server.storage.iter_older_than(5):
-                    Server.set_digest(key, value, is_metadata)
+                for (
+                    key,
+                    value,
+                    is_metadata,
+                    last_write,
+                ) in Server.storage.iter_older_than(5):
+                    Server.set_digest(key, value, is_metadata,
+                                      exclude_current=True)
                     Server.storage.update_republish(key)
                 keys_to_replicate = Server.find_replicas()
 
+                # Republishing keys that have less replicas than the replication factor
+
                 if len(keys_to_replicate):
                     for key, is_metadata in keys_to_replicate:
+                        _, local_last_write = Server.storage.check_if_new_value_exists(
+                            key
+                        )
+
                         Server.set_digest(
                             key,
                             Server.storage.get(
                                 key, metadata=is_metadata, update_timestamp=False
                             ),
                             is_metadata,
+                            exclude_current=True,
+                            local_last_write=local_last_write,
                         )
 
             except Exception as e:
                 logger.error("Thrown Exception %s", str(e))
                 pass
 
 
 @rpyc.service
 class ServerService(Service):
+    #
+    # RPC accessed by clients
+    #
+    @rpyc.exposed
+    def rpc_get_file_chunk_value(self, key):
+        return Server.storage.get(key, metadata=False)
+
+    @rpyc.exposed
+    def get(self, key, apply_hash_to_key=True):
+        """
+        Get a key if the network has it.
+
+        Returns:
+            :class:`None` if not found, the value otherwise.
+        """
+
+        logger.debug(f"Looking up key {key}")
+        if apply_hash_to_key:
+            key = digest(key)
+
+        node = Node(key)
+        nearest = FileSystemProtocol.router.find_neighbors(node)
+        if not nearest:
+            logger.debug(f"There are no known neighbors to get key {key}")
+            if Server.storage.contains(key):
+                logger.debug("Getting key from this same node")
+                return pickle.loads(Server.storage.get(key, True))
+            return None
+        spider = ValueSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
+        data = spider.find()
+        if data is None:
+            logger.debug("NONE DATA")
+            return None
+        logger.debug(f"DATA {data}")
+        metadata_list = pickle.loads(data)
+        return metadata_list
+
+    @rpyc.exposed
+    def upload_file(self, key, data: bytes, apply_hash_to_key=True):
+        chunks = Server.split_data(data, 1000)
+        logger.debug(f"chunks {len(chunks)}, {chunks}")
+        digested_chunks = [digest(c) for c in chunks]
+        metadata_list = pickle.dumps(digested_chunks)
+        processed_chunks = ((digest(c), c) for c in chunks)
+
+        for c in processed_chunks:
+            Server.set_digest(c[0], c[1], metadata=False)
+
+        logger.debug("Writting key metadata")
+        if apply_hash_to_key:
+            dkey = digest(key)
+            Server.set_digest(dkey, metadata_list)
+        else:
+            Server.set_digest(key, metadata_list)
+
+    @rpyc.exposed
+    def get_file_chunk_location(self, chunk_key):
+        logger.debug("looking file chunk location")
+        node = Node(chunk_key)
+        nearest = FileSystemProtocol.router.find_neighbors(node)
+        if not nearest:
+            logger.debug(
+                f"There are no known neighbors to get file chunk location {chunk_key}"
+            )
+            if Server.storage.contains(chunk_key, False) is not None:
+                logger.debug(
+                    f"Found in this server, {Server.node.ip}, port, {Server.node.port}"
+                )
+                return [(Server.node.ip, Server.node.port)]
+            return None
+
+        logger.debug("Initiating ChunkLocationSpiderCrawl")
+        spider = ChunkLocationSpiderCrawl(
+            node, nearest, Server.ksize, Server.alpha)
+        results = spider.find()
+        logger.debug(f"results of ChunkLocationSpider {results}")
+        return results
+
+    @rpyc.exposed
+    def rpc_find_chunk_location(
+        self, sender: tuple[str, str], nodeid: bytes, key: bytes
+    ):
+        logger.debug("entry in rpc_find_chunk_location")
+
+        source = Node(nodeid, sender[0], sender[1])
+        # if a new node is sending the request, give all data it should contain
+        address = (source.ip, source.port)
+        with ServerSession(address[0], address[1]) as conn:
+            FileSystemProtocol.wellcome_if_new(conn, source)
+        # get value from storage
+        if Server.storage.contains(key, False):
+            return {"value": (Server.node.ip, Server.node.port)}
+        return self.rpc_find_node(sender, nodeid, key)
+
+    @rpyc.exposed
+    def find_neighbors(self):
+        nearest = FileSystemProtocol.router.find_neighbors(
+            Server.node, exclude=Server.node
+        )
+        return [(i.ip, i.port) for i in nearest]
+
+    #
+    # RPCs only accessed by servers
+    #
     @rpyc.exposed
     def rpc_store(self, sender, nodeid: bytes, key: bytes, value, metadata=True):
         """Instructs a node to store a value
 
         Args:
             sender : Sender Node
             nodeid (bytes): Node to be told to store info
@@ -285,198 +428,118 @@
 
         logger.debug("Entry in rpc_store")
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
 
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
-            FileSystemProtocol.welcome_if_new(conn, source)
+            logger.info(f"wellcome_If_new in rpc_store {address}")
+            FileSystemProtocol.wellcome_if_new(conn, source)
 
         logger.debug(
             f"got a store request from %s, storing '%s'='%s' {sender}, {key}, {value}"
         )
         # store values and report success
         if metadata:
-            FileSystemProtocol.storage.set_metadata(key, value, republish_data=False)
+            FileSystemProtocol.storage.set_metadata(
+                key, value, republish_data=False)
         else:
             FileSystemProtocol.storage.set_value(key, value, metadata=False)
         return True
 
     @rpyc.exposed
     def rpc_find_value(
         self, sender: tuple[str, str], nodeid: bytes, key: bytes, metadata=True
     ):
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
-            FileSystemProtocol.welcome_if_new(conn, source)
+            logger.info(f"wellcome_If_new in find_value {address}")
+            FileSystemProtocol.wellcome_if_new(conn, source)
         # get value from storage
         if not FileSystemProtocol.storage.contains(key, metadata):
-            logger.debug(f"Value with key {key} not found, calling rpc_find_node")
+            logger.debug(
+                f"Value with key {key} not found, calling rpc_find_node")
             logger.debug(f"type of key is {type(key)}")
+
             return self.rpc_find_node(sender, nodeid, key)
 
         value = FileSystemProtocol.storage.get(key, None, metadata)
         logger.debug(f"returning value {value}")
         return {"value": value}
 
     @rpyc.exposed
-    def rpc_find_chunk_location(
-        self, sender: tuple[str, str], nodeid: bytes, key: bytes
-    ):
-        logger.debug("entry in rpc_find_chunk_location")
-
-        source = Node(nodeid, sender[0], sender[1])
-        # if a new node is sending the request, give all data it should contain
-        address = (source.ip, source.port)
-        with ServerSession(address[0], address[1]) as conn:
-            FileSystemProtocol.welcome_if_new(conn, source)
-        # get value from storage
-        if Server.storage.contains(key, False):
-            return {"value": (Server.node.ip, Server.node.port)}
-        return self.rpc_find_node(sender, nodeid, key)
-
-    @rpyc.exposed
     def rpc_ping(self, sender, nodeid: bytes):
         """Probe a Node to see if pc is online
 
         Args:
             sender : sender node
             nodeid (bytes): node to be probed
 
         Returns:
             bytes: node id if alive, None if not
         """
-        logger.debug(f"rpc ping called from {nodeid}, {sender[0]}, {sender[1]}")
+        logger.debug(
+            f"rpc ping called from {nodeid}, {sender[0]}, {sender[1]}")
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
-            FileSystemProtocol.welcome_if_new(conn, source)
+            logger.info(f"wellcome_If_new in ping {address}")
+            FileSystemProtocol.wellcome_if_new(conn, source)
         logger.debug("return ping")
         return FileSystemProtocol.source_node.id
 
     @rpyc.exposed
     def rpc_find_node(self, sender, nodeid: bytes, key: bytes):
-        logger.debug(f"finding neighbors of {int(nodeid.hex(), 16)} in local table")
+        logger.debug(
+            f"finding neighbors of {int(nodeid.hex(), 16)} in local table")
 
         source = Node(nodeid, sender[0], sender[1])
 
         logger.debug(f"node id {nodeid}")
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
-            FileSystemProtocol.welcome_if_new(conn, source)
+            logger.info(f"wellcome_If_new in find_node {address}")
+            FileSystemProtocol.wellcome_if_new(conn, source)
         # create a fictional node to perform the search
         logger.debug(f"fictional key {key}")
         logger.debug(f"SEnder [0] Sender [1] {source.ip}, {source.port}")
         node = Node(key)
         # ask for the neighbors of the node
-        neighbors = FileSystemProtocol.router.find_neighbors(node, exclude=source)
+        neighbors = FileSystemProtocol.router.find_neighbors(
+            node, exclude=source)
         logger.debug(f"neighbors of find_node: { neighbors}")
         return list(map(tuple, neighbors))
 
     @rpyc.exposed
     def rpc_contains(self, sender, nodeid: bytes, key: bytes, is_metadata=True):
         source = Node(nodeid, sender[0], sender[1])
-        # if a new node is sending the request, give all data it should contain
+        # if a new node is sending the request, givemsg all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
-            FileSystemProtocol.welcome_if_new(conn, source)
+            logger.info(f"wellcome_If_new in contains {address}")
+            FileSystemProtocol.wellcome_if_new(conn, source)
         # get value from storage
         return FileSystemProtocol.storage.contains(key, is_metadata)
 
     @rpyc.exposed
-    def rpc_get_file_chunk_value(self, key):
-        return Server.storage.get(key, metadata=False)
-
-    @rpyc.exposed
-    def bootstrappable_neighbors(self):
-        """
-        Get a :class:`list` of (ip, port) :class:`tuple` pairs suitable for
-        use as an argument to the bootstrap method.
-
-        The server should have been bootstrapped
-        already - this is just a utility for getting some neighbors and then
-        storing them if this server is going down for a while.  When it comes
-        back up, the list of nodes can be used to bootstrap.
-        """
-        neighbors = FileSystemProtocol.router.find_neighbors(Server.node)
-        return [tuple(n)[-2:] for n in neighbors]
-
-    @rpyc.exposed
-    def get(self, key, apply_hash_to_key=True):
-        """
-        Get a key if the network has it.
-
-        Returns:
-            :class:`None` if not found, the value otherwise.
-        """
-
-        logger.debug(f"Looking up key {key}")
-        if apply_hash_to_key:
-            key = digest(key)
-
-        node = Node(key)
-        nearest = FileSystemProtocol.router.find_neighbors(node)
-        if not nearest:
-            logger.debug(f"There are no known neighbors to get key {key}")
-            if Server.storage.contains(key):
-                logger.debug("Getting key from this same node")
-                return pickle.loads(Server.storage.get(key, True))
-            return None
-        spider = ValueSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
-        data = spider.find()
-        if data is None:
-            logger.debug("NONE DATA")
-            return None
-        logger.debug(f"DATA {data}")
-        metadata_list = pickle.loads(data)
-        return metadata_list
-
-    @rpyc.exposed
-    def get_file_chunk_location(self, chunk_key):
-        logger.debug("looking file chunk location")
-        node = Node(chunk_key)
-        nearest = FileSystemProtocol.router.find_neighbors(node)
-        if not nearest:
-            logger.debug(
-                f"There are no known neighbors to get file chunk location {chunk_key}"
-            )
-            if Server.storage.contains(chunk_key, False) is not None:
-                logger.debug(
-                    f"Found in this server, {Server.node.ip}, port, {Server.node.port}"
-                )
-                return [(Server.node.ip, Server.node.port)]
-            return None
-
-        logger.debug("Initiating ChunkLocationSpiderCrawl")
-        spider = ChunkLocationSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
-        results = spider.find()
-        logger.debug(f"results of ChunkLocationSpider {results}")
-        return results
-
-    @rpyc.exposed
-    def upload_file(self, key, data: bytes, apply_hash_to_key=True):
-        chunks = Server.split_data(data, 1000)
-        logger.debug(f"chunks {len(chunks)}, {chunks}")
-        digested_chunks = [digest(c) for c in chunks]
-        metadata_list = pickle.dumps(digested_chunks)
-        processed_chunks = ((digest(c), c) for c in chunks)
-
-        for c in processed_chunks:
-            Server.set_digest(c[0], c[1], metadata=False)
-
-        logger.debug("Writting key metadata")
-        if apply_hash_to_key:
-            dkey = digest(key)
-            Server.set_digest(dkey, metadata_list)
-        else:
-            Server.set_digest(key, metadata_list)
+    def rpc_check_if_new_value_exists(
+        self, sender, nodeid: bytes, key: bytes, is_metadata=True
+    ):
+        source = Node(nodeid, sender[0], sender[1])
+        # if a new node is sending the request, give all data it should contain
+        address = (source.ip, source.port)
+        with ServerSession(address[0], address[1]) as conn:
+            logger.info(f"wellcome_If_new in check_if_new_value {address}")
+            FileSystemProtocol.wellcome_if_new(conn, source)
+        # get value from storage
+        return FileSystemProtocol.storage.check_if_new_value_exists(key)
 
     @rpyc.exposed
     def set_key(self, key, value, apply_hash_to_key=True):
         """
         Set the given string key to the given value in the network.
         """
 
@@ -485,21 +548,14 @@
             raise TypeError(
                 f"Value must be of type int, float, bool, str, or bytes, received {value}"
             )
         if apply_hash_to_key:
             key = digest(key)
         return Server.set_digest(key, value)
 
-    @rpyc.exposed
-    def find_neighbors(self):
-        nearest = FileSystemProtocol.router.find_neighbors(
-            Server.node, exclude=Server.node
-        )
-        return [(i.ip, i.port) for i in nearest]
-
 
 def check_dht_value_type(value):
     """
     Checks to see if the type of the value is a valid type for
     placing in the dht.
     """
     typeset = [int, float, bool, str, bytes]
```

### Comparing `kade_drive-0.5.1/kade_drive/core/node.py` & `kade_drive-0.7.0/kade_drive/core/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import heapq
 
-
 class Node:
     """
     Simple object to encapsulate the concept of a Node (minimally an ID, but
     also possibly an IP and port if this represents a node on the network).
     This class should generally not be instantiated directly, as it is a low
     level construct mostly used by the router.
     """
```

### Comparing `kade_drive-0.5.1/kade_drive/core/protocol.py` & `kade_drive-0.7.0/kade_drive/core/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import random
 import logging
 import rpyc
 
-from core.node import Node
-from core.storage import PersistentStorage
-from core.utils import digest
+from kade_drive.core.node import Node
+from kade_drive.core.storage import logger, PersistentStorage
+from kade_drive.core.utils import digest
 
 
 # Create a file handler
-file_handler = logging.FileHandler("log_file.log")
+# file_handler = logging.FileHandler("log_file.log")
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
-file_handler.setFormatter(formatter)
+# file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
+# logger.addHandler(file_handler)
 
 
 class FileSystemProtocol:
     source_node: Node
     ksize: int
     storage: PersistentStorage
     router: None = None
@@ -63,14 +63,24 @@
             response = conn.rpc_contains(
                 address, FileSystemProtocol.source_node.id, key, is_metadata
             )
 
         return FileSystemProtocol.process_response(conn, response, node_to_ask)
 
     @staticmethod
+    def call_check_if_new_value_exists(conn, node_to_ask, key: bytes, is_metadata=True):
+        response = None
+        if conn:
+            address = (node_to_ask.ip, node_to_ask.port)
+            response = conn.rpc_check_if_new_value_exists(
+                address, FileSystemProtocol.source_node.id, key)
+
+        return FileSystemProtocol.process_response(conn, response, node_to_ask)
+
+    @staticmethod
     def call_find_node(conn, node_to_ask: Node, node_to_find: Node):
         """
         async function to call the find node rpc method
         """
 
         logger.debug("inside call find Node")
         response = None
@@ -121,25 +131,27 @@
     @staticmethod
     def call_ping(conn, node_to_ask: Node):
         """
         async function to call the ping rpc method
         """
         response = None
         address = (node_to_ask.ip, node_to_ask.port)
+        logge.info(f"calling ping {address}")
         response = None
 
         if conn:
-            response = conn.rpc_ping(address, FileSystemProtocol.source_node.id)
+            response = conn.rpc_ping(
+                address, FileSystemProtocol.source_node.id)
 
         logger.debug(f"Got Response {response}")
 
         return FileSystemProtocol.process_response(conn, response, node_to_ask)
 
     @staticmethod
-    def welcome_if_new(conn, node: Node):
+    def wellcome_if_new(conn, node: Node):
         """
         Given a new node, send it all the keys/values it should be storing,
         then add it to the routing table.
 
         @param node: A new node that just joined (or that we just found out
         about).
 
@@ -149,59 +161,69 @@
         is closer than the closest in that list, then store the key/value
         on the new node (per section 2.5 of the paper)
         """
         # if the node is in the table, do nothing
         if not FileSystemProtocol.router.is_new_node(node):
             return
 
+        # TODO uncomment this
+        if (node.ip, node.port) == (FileSystemProtocol.source_node.ip, FileSystemProtocol.source_node.port):
+            logger.critical("called wellcome if new in self")
+            return
         # add node to table
 
         logger.debug("Adding new node to contacts")
         FileSystemProtocol.router.add_contact(node)
 
         logger.info(f"never seen {node} before, adding to router")
         # iterate over storage
+
+        logger.info(f"Adding new Node to contacts {FileSystemProtocol.source_node}")
+
         for key, value, is_metadata in FileSystemProtocol.storage:
             logger.debug("entry for")
             # Create fictional node to calculate distance
             keynode = Node(digest(key))
             neighbors = FileSystemProtocol.router.find_neighbors(keynode)
 
             new_node_close = False
             this_closest = False
             # if the node is closer tan the furtherst neighbor
             # the values should be then stored in that node
-            if len(neighbors) > 2:
+            # if len(neighbors) > 2:
+            logger.info(f"neighbors in for {neighbors}")
+
+            if neighbors or len(neighbors) > 0:
                 last = neighbors[-1].distance_to(keynode)
                 new_node_close = node.distance_to(keynode) < last
                 first = neighbors[0].distance_to(keynode)
                 this_closest = (
                     FileSystemProtocol.source_node.distance_to(keynode) < first
                 )
             # if not neighbors, store data in the node
-            logger.debug(f"neighbors in for {neighbors}")
             if not neighbors or (new_node_close and this_closest):
-                logger.debug("calling call_store in welcome_if_new")
+                logger.debug("calling call_store in wellcome_if_new")
                 with ServerSession(node.ip, node.port) as conn:
-                    FileSystemProtocol.call_store(conn, node, key, value, is_metadata)
+                    FileSystemProtocol.call_store(
+                        conn, node, key, value, is_metadata)
 
     @staticmethod
     def process_response(conn, response, node: Node):
         """
         If we get a response, add the node to the routing table.  If
         we get no response, make sure it's removed from the routing table.
         """
 
         logger.debug(f"response is {response}")
         if response is None:
             logger.info(f"no response from {node}, removing from router")
             FileSystemProtocol.router.remove_contact(node)
             return response
 
-        FileSystemProtocol.welcome_if_new(conn, node)
+        FileSystemProtocol.wellcome_if_new(conn, node)
         logger.debug(f"got successful response from {node}")
         logger.debug(response)
         return response
 
 
 class ServerSession:
     """Server session context manager."""
```

### Comparing `kade_drive-0.5.1/kade_drive/core/routing.py` & `kade_drive-0.7.0/kade_drive/core/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import heapq
 import time
 import logging
 
-from core.protocol import FileSystemProtocol, ServerSession
+from kade_drive.core.protocol import FileSystemProtocol, ServerSession
 from itertools import chain
 from collections import OrderedDict
-from core.utils import shared_prefix, bytes_to_bit_string
-from core.node import Node
+from kade_drive.core.utils import shared_prefix, bytes_to_bit_string
+from kade_drive.core.node import Node
 
 
 # Create a file handler
-file_handler = logging.FileHandler("log_file.log")
+# file_handler = logging.FileHandler("log_file.log")
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
-file_handler.setFormatter(formatter)
+# file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
+# logger.addHandler(file_handler)
 
 
 class KBucket:
     """
     K is the number of entries in a bucket, their node IDs are expected to be randomly distributed within the ID-range the bucket covers
     Each node is putted in a bucket based on how far away they are from the source node.
     This way when you are looking for some node you don't have to bother all possible nodes
@@ -110,15 +110,15 @@
         index = table.get_bucket_for(startNode)
         logger.debug(f"table.buckets, {table.buckets}, {index}")
         table.buckets[index].touch_last_updated()
         logger.debug("nodes in bucket %s", table.buckets[index].nodes.values())
         self.current_nodes = table.buckets[index].get_nodes()
         logger.debug("current nodes %s", self.current_nodes)
         self.left_buckets = table.buckets[:index]
-        self.right_buckets = table.buckets[(index + 1) :]
+        self.right_buckets = table.buckets[(index + 1):]
         self.left = True
 
     def __iter__(self):
         return self
 
     def __next__(self) -> Node:
         """
@@ -186,28 +186,30 @@
         index = self.get_bucket_for(node)
         return self.buckets[index].is_new_node(node)
 
     def add_contact(self, node: Node):
         index = self.get_bucket_for(node)
         bucket = self.buckets[index]
 
-        logger.debug(f"previous nodes in bucket of index {index}, {bucket.get_nodes()}")
+        logger.debug(
+            f"previous nodes in bucket of index {index}, {bucket.get_nodes()}")
         # this will succeed unless the bucket is full
         if bucket.add_node(node):
             logger.debug(f"Bucket nodes:  {bucket.get_nodes()}")
             return
 
         # Per section 4.2 of paper, split if the bucket has the node
         # in its range or if the depth is not congruent to 0 mod 5
         if bucket.has_in_range(self.node) or bucket.depth() % 5 != 0:
             self.split_bucket(index)
             self.add_contact(node)
         else:
             node_to_ask = bucket.head()
             addr = (node_to_ask.ip, node_to_ask.port)
+            logger.critical(f"node_to_ask {node_to_ask}, addr {addr}")
             with ServerSession(addr[0], addr[1]) as conn:
                 FileSystemProtocol.call_ping(conn, node_to_ask)
 
     def get_bucket_for(self, node: Node):
         """
         Get the index of the bucket that the given node would fall into.
         """
@@ -238,15 +240,16 @@
         k = k or self.ksize
         nodes: list[tuple[int, Node]] = []
         for neighbor in TableTraverser(self, node):
             if exclude:
                 logger.debug(
                     f"Comparing {neighbor.ip} {neighbor.port} and {exclude.ip} {exclude.port}"
                 )
-            not_excluded = exclude is None or not neighbor.same_home_as(exclude)
+            not_excluded = exclude is None or not neighbor.same_home_as(
+                exclude)
             logger.debug(f"not excluded {not_excluded}")
             if neighbor.id != node.id and not_excluded:
                 heapq.heappush(nodes, (node.distance_to(neighbor), neighbor))
             if len(nodes) == k:
                 break
 
         return [item[1] for item in heapq.nsmallest(k, nodes)]
```

### Comparing `kade_drive-0.5.1/kade_drive/core/storage.py` & `kade_drive-0.7.0/kade_drive/core/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from pathlib import Path
 import threading
 import base64
 import logging
 
 
 # Create a file handler
-file_handler = logging.FileHandler("log_file.log")
+# file_handler = logging.FileHandler("log_file.log")
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
-file_handler.setFormatter(formatter)
+# file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
+# logger.addHandler(file_handler)
 
 
 class PersistentStorage:
     """
     This class allows to persist files on disk using mongodb.
     The class acts as an OrderedDict that his keys are the hash of an
     specific file chunk and the value is the (ip, port) of the node that
@@ -55,19 +55,30 @@
 
         os.makedirs(self.metadata_path, exist_ok=True)
 
         os.makedirs(self.keys_path, exist_ok=True)
 
         os.makedirs(self.timestamp_path, exist_ok=True)
 
-    def update_timestamp(self, filename: str, republish_data=False):
+    def update_timestamp(self, filename: str, republish_data=False, is_write=False):
         self.ensure_dir_paths()
-        data = {"date": datetime.now(), "republish": republish_data}
+        data = {}
+        if os.path.exists(os.path.join(self.timestamp_path, str(filename))):
+            with open(os.path.join(self.timestamp_path, str(filename)), "rb") as f:
+                #  BUGGGG
+                data = pickle.load(f)
 
-        logger.debug(f"mira ruta {os.path.join(self.timestamp_path, str(filename))}")
+        data["date"] = datetime.now()
+        data["republish"] = republish_data
+
+        if is_write:
+            data['last_write'] = datetime.now()
+
+        logger.debug(
+            f"mira ruta {os.path.join(self.timestamp_path, str(filename))}")
         with open(os.path.join(self.timestamp_path, str(filename)), "wb") as f:
             pickle.dump(data, f)
 
     def update_republish(self, key: bytes):
         str_key = str(base64.urlsafe_b64encode(key))
         with open(os.path.join(self.timestamp_path, str_key), "rb") as f:
             data = pickle.load(f)
@@ -91,23 +102,27 @@
                             data = pickle.load(f)
 
                         if (datetime.now() - data["date"]).seconds > self.ttl:
                             logger.info(
                                 f"Removing file {file}, beacuse it has not been accessed in {self.ttl/60} minutes"
                             )
                             if Path(os.path.join(self.values_path, str(file))).exists():
-                                os.remove(os.path.join(self.values_path, str(file)))
+                                os.remove(os.path.join(
+                                    self.values_path, str(file)))
                             if Path(
                                 os.path.join(self.metadata_path, str(file))
                             ).exists():
-                                os.remove(os.path.join(self.metadata_path, str(file)))
+                                os.remove(os.path.join(
+                                    self.metadata_path, str(file)))
                             if Path(os.path.join(self.keys_path, str(file))).exists():
-                                os.remove(os.path.join(self.keys_path, str(file)))
+                                os.remove(os.path.join(
+                                    self.keys_path, str(file)))
 
-                            os.remove(os.path.join(self.timestamp_path, str(file)))
+                            os.remove(os.path.join(
+                                self.timestamp_path, str(file)))
             sleep(self.ttl)
 
     def get_value(self, str_key: str, update_timestamp=True, metadata=True):
         self.ensure_dir_paths()
         if metadata:
             path = os.path.join(self.metadata_path, str_key)
         else:
@@ -122,15 +137,15 @@
             logger.error(f"tried to get non existing data with key {str_key}")
             print("Tried to get data that is not in db")
         return result
 
     def set_value(self, key: bytes, value, metadata=True, republish_data=False):
         str_key = str(base64.urlsafe_b64encode(key))
         self.ensure_dir_paths()
-        self.update_timestamp(str_key, republish_data)
+        self.update_timestamp(str_key, republish_data, is_write=True)
         if metadata:
             path = os.path.join(self.metadata_path, str_key)
         else:
             path = os.path.join(self.values_path, str_key)
         with open(path, "wb") as f:
             try:
                 logger.debug("writting data  to file")
@@ -179,14 +194,25 @@
         else:
             path = Path(os.path.join(self.values_path, str_key))
             if not path.exists():
                 return False
 
         return True
 
+    def check_if_new_value_exists(self, key):
+        str_key = str(base64.urlsafe_b64encode(key))
+        path = Path(os.path.join(self.timestamp_path, str_key))
+        if not path.exists():
+            return False, None
+
+        with open(os.path.join(self.timestamp_path, str_key), "rb") as f:
+            data = pickle.load(f)
+
+        return True, data['last_write']
+
     def __getitem__(self, key: bytes):
         self.cull()
         str_key = str(base64.urlsafe_b64encode(key))
         result = self.get_value(str_key)
         if result is None:
             raise KeyError()
         return result
@@ -196,25 +222,24 @@
 
     def iter_older_than(self, seconds_old):
         self.ensure_dir_paths()
         for path, dir, files in os.walk(self.timestamp_path):
             for file in files:
                 if Path(os.path.join(self.timestamp_path, file)).exists():
                     with open(os.path.join(self.timestamp_path, file), "rb") as f:
-                        sleep(0.1)
                         data = pickle.load(f)
                     if (datetime.now() - data["date"]).seconds >= seconds_old or data[
                         "republish"
                     ]:
                         key, is_metadata = self.get_key_in_bytes(str(file))
                         value = self.get_value(
                             str(file), update_timestamp=False, metadata=is_metadata
                         )
                         assert value is not None
-                        yield key, value, is_metadata
+                        yield key, value, is_metadata, data['last_write']
 
     def keys(self):
         ikeys_files = os.listdir(os.path.join(self.keys_path))
         ikeys = []
         imetadata = []
         for key_name in ikeys_files:
             k, m = self.get_key_in_bytes(key_name)
@@ -234,9 +259,10 @@
             ikeys.append(k)
             imetadata.append(m)
 
         logger.debug("ikeys: %s", ikeys)
         ivalues: list[bytes] = []
 
         for i, ik in enumerate(ikeys):
-            ivalues.append(self.get(ik, update_timestamp=False, metadata=imetadata[i]))
+            ivalues.append(
+                self.get(ik, update_timestamp=False, metadata=imetadata[i]))
         return zip(ikeys, ivalues, imetadata)
```

### Comparing `kade_drive-0.5.1/kade_drive/server.py` & `kade_drive-0.7.0/kade_drive/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typer import Typer, Option
 import socket
-from core.network import Server
+from kade_drive.core.network import Server
 import threading
-from message_system.message_system import Message_System
-from core.utils import get_ips
-from core.config import Config
+from message_system.message_system import logger, MessageSystem
+from kade_drive.core.config import Config
 import logging
 
 # Create a file handler
 file_handler = logging.FileHandler("log_file.log")
 
 # Set the logging format
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
@@ -18,39 +17,40 @@
 # logging.basicConfig(level=logging.INFO,
 #                     format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
 # logging.getLogger("SERVER/8086").setLevel(logging.CRITICAL)
 # Create a logger instance
 logger = logging.getLogger(__name__)
 
 
-def start_server(host_ip=None, config: Config|None=None):
+def start_server(host_ip=None, config: Config | None = None):
     broadcast = None
     logger.debug(host_ip)
     bootstrap_nodes = None
 
     if host_ip is None:
-        ip_br = get_ips()[0]
+        ip_br = MessageSystem.get_ips()[0]
+        logger.debug(ip_br)
         broadcast = ip_br["broadcast"]
         host_ip = ip_br["addr"]
     logger.info(host_ip)
 
-    ms = Message_System(host_ip, broadcast)
+    ms = MessageSystem(host_ip, broadcast)
     hosts = []
 
     msg = ms.receive(service_name="dfs")
     logger.debug(msg)
     if msg:
         hosts.append(msg)
         logger.debug(f"Found {msg}")
         bootstrap_nodes = msg
     else:
         logger.info("No servers answered :(")
 
     if host_ip is None:
-        logger.warning(f"aaa {socket.get_hostname()}")
+        logger.warning(f"aaa {socket.gethostname()}")
         host_ip = socket.gethostbyname(socket.gethostname())
 
     if config is None:
         config = Config()
     Server.init(ip=host_ip.split(" ")[0], config=config)
 
     logger.info(f"broadcasting {Server.node.ip} {Server.node.port}")
@@ -65,29 +65,33 @@
     logger.info(f"Server started at {host_ip}")
 
 
 app = Typer()
 
 
 @app.command()
-def start(host_ip=Option(default=None), log_level=Option(default="INFO")):
-    if log_level == "INFO":
-        log_level = logging.INFO
-    if log_level == "DEBUG":
-        log_level = logging.DEBUG
-    if log_level == "WARNING":
-        log_level = logging.WARNING
+def start(host_ip=Option(default=None), log_level=Option(default="DEBUG")):
+    match log_level:
+        case 'INFO':
+            log_level = logging.INFO
+        case 'DEBUG':
+            log_level = logging.DEBUG
+        case 'WARNING':
+            log_level = logging.WARNING
+        case _:
+            log_level = logging.INFO
 
     logging.basicConfig(
-        level=log_level, format="%(asctime)s  - %(name)s - %(levelname)s - %(message)s"
+        level=log_level, format="%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
 
-    logging.getLogger("SERVER/8086").setLevel(logging.CRITICAL)
+    logging.getLogger("SERVER").setLevel(logging.CRITICAL+1)
     # Create a logger instance
     logger = logging.getLogger(__name__)
-
+    if not type(host_ip) == str:
+        host_ip = None
     logger.debug(host_ip)
     start_server(host_ip)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `kade_drive-0.5.1/kade_drive/test_store_file.py` & `kade_drive-0.7.0/kade_drive/test_store_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.datasets import load_diabetes
 import pandas as pd
 import pickle
-from client import ClientSession
+from kade_drive.client import ClientSession
 from time import sleep
 
 
 def test_store_df():
     X, y = load_diabetes(return_X_y=True)
 
     X = pd.DataFrame(X)
@@ -20,14 +20,14 @@
 
     client_session.put("dataset_diabetes", X_pickle)
 
     print("DONE, Getting")
     print()
     print()
     sleep(5)
-    value_getted = client_session.get("dataset_diabetes")
+    value_getted, conn = client_session.get("dataset_diabetes")
 
     print("value getted ", value_getted)
+    print('original value', X)
+    assert value_getted is not None
     assert X.equals(value_getted)
 
-
-test_store_df()
```

### Comparing `kade_drive-0.5.1/kade_drive/tests/conftest.py` & `kade_drive-0.7.0/kade_drive/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # import random
 # import hashlib
 # # pylint: disable=no-name-in-module
 # from struct import pack
 
 # import pytest
 
-# from core.network import Server
-# from core.node import Node
-# from core.routing import RoutingTable
+# from kade_drive.core.network import Server
+# from kade_drive.core.node import Node
+# from kade_drive.core.routing import RoutingTable
 
 
 # # @pytest.fixture()
 # # def event_loop():
 # #     return asyncio.get_event_loop()
```

### Comparing `kade_drive-0.5.1/kade_drive/tests/data_to_split.txt` & `kade_drive-0.7.0/kade_drive/tests/data_to_split.txt`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.1/kade_drive/tests/test_node.py` & `kade_drive-0.7.0/kade_drive/tests/test_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import hashlib
 
 
-from core.node import Node, NodeHeap
+from kade_drive.core.node import Node, NodeHeap
 
 
 class TestNode:
     def test_long_id(self):  # pylint: disable=no-self-use
         rid = hashlib.sha1(str(random.getrandbits(255)).encode()).digest()
         node = Node(rid)
         assert node.long_id == int(rid.hex(), 16)
```

### Comparing `kade_drive-0.5.1/kade_drive/tests/test_routing.py` & `kade_drive-0.7.0/kade_drive/tests/test_routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from random import shuffle
-from core.routing import KBucket, TableTraverser
+from kade_drive.core.routing import KBucket, TableTraverser
 
 
 class TestKBucket:
     def test_split(self, mknode):  # pylint: disable=no-self-use
         bucket = KBucket(0, 10, 5)
         bucket.add_node(mknode(intid=5))
         bucket.add_node(mknode(intid=6))
```

### Comparing `kade_drive-0.5.1/kade_drive/tests/test_splitdata.py` & `kade_drive-0.7.0/kade_drive/tests/test_splitdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle
 import pandas as pd
 from sklearn.datasets import load_diabetes
-from core.network import Server
+from kade_drive.core.network import Server
 
 
 def test_split_data():
     mytext = None
     with open("tests/data_to_split.txt", "rb") as txtfile:
         mytext = txtfile.read()
```

### Comparing `kade_drive-0.5.1/kade_drive/tests/test_storage.py` & `kade_drive-0.7.0/kade_drive/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.1/kade_drive/tests/test_utils.py` & `kade_drive-0.7.0/kade_drive/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hashlib
 
-from core.utils import digest, shared_prefix
+from kade_drive.core.utils import digest, shared_prefix
 
 
 class TestUtils:
     def test_digest(self):  # pylint: disable=no-self-use
         dig = hashlib.sha1(b"1").digest()
         assert dig == digest(1)
```

