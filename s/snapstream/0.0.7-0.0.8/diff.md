# Comparing `tmp/snapstream-0.0.7.tar.gz` & `tmp/snapstream-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.7.tar", max compression
+gzip compressed data, was "snapstream-0.0.8.tar", max compression
```

## Comparing `snapstream-0.0.7.tar` & `snapstream-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-06-22 20:32:31.360191 snapstream-0.0.7/LICENSE
--rw-r--r--   0        0        0     2536 2023-06-22 20:32:31.360191 snapstream-0.0.7/README.md
--rw-r--r--   0        0        0     2034 2023-06-22 20:32:44.784464 snapstream-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2277 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/__init__.py
--rw-r--r--   0        0        0     7897 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/__main__.py
--rw-r--r--   0        0        0     9781 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/caching.py
--rw-r--r--   0        0        0     2812 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/codecs.py
--rw-r--r--   0        0        0    10774 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/core.py
--rw-r--r--   0        0        0     3255 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-11 14:39:54.304796 snapstream-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2536 2023-07-11 14:39:54.304796 snapstream-0.0.8/README.md
+-rw-r--r--   0        0        0     2034 2023-07-11 14:40:07.508956 snapstream-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2277 2023-07-11 14:39:54.308796 snapstream-0.0.8/snapstream/__init__.py
+-rw-r--r--   0        0        0     8371 2023-07-11 14:39:54.308796 snapstream-0.0.8/snapstream/__main__.py
+-rw-r--r--   0        0        0     9781 2023-07-11 14:39:54.308796 snapstream-0.0.8/snapstream/caching.py
+-rw-r--r--   0        0        0     2812 2023-07-11 14:39:54.312796 snapstream-0.0.8/snapstream/codecs.py
+-rw-r--r--   0        0        0    11057 2023-07-11 14:39:54.312796 snapstream-0.0.8/snapstream/core.py
+-rw-r--r--   0        0        0     3255 2023-07-11 14:39:54.312796 snapstream-0.0.8/snapstream/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.8/PKG-INFO
```

### Comparing `snapstream-0.0.7/LICENSE` & `snapstream-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.7/README.md` & `snapstream-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.7/pyproject.toml` & `snapstream-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.7"
+version = "0.0.8"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 documentation = "https://snapstream.readthedocs.io"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
```

### Comparing `snapstream-0.0.7/snapstream/__init__.py` & `snapstream-0.0.8/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.7/snapstream/__main__.py` & `snapstream-0.0.8/snapstream/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 def get_args(args=argv[1:]) -> Namespace:
     """Get user arguments."""
     parser = ArgumentParser('snapstream')
     subparsers = parser.add_subparsers(dest='action', required=True)
     parser.add_argument('--config-path', type=str, default=DEFAULT_CONFIG_PATH,
                         help='file containing topic/cache configurations')
-    parser.add_argument('--secrets-base-path', type=str, default='',
+    parser.add_argument('--secrets-base-path', type=str, default='/etc/secrets',
                         help='folder containing secret files')
 
     topic = subparsers.add_parser('topic', help='read messages from Topic')
     topic.add_argument('name', type=str,
                        help='topicname')
     topic.add_argument('-s', '--schema', type=str,
                        help='path to avro schema file')
@@ -56,30 +56,32 @@
                        help='list of columns to extract from message (if dict), ex: "time,date,pk"')
     cache.add_argument('--stats', action='store_true',
                        help='print additional database statistics')
 
     return parser.parse_args(args)
 
 
-def default_topic_entry(name: str, prep: Callable) -> dict:
+def default_topic_entry(args: Namespace, prep: Callable) -> dict:
     """Create default topic entry."""
     return {
         'type': 'Topic',
-        'name': prep(name),
+        'name': prep(args.name),
         'conf': {
             'bootstrap.servers': 'localhost:29091',
-        }
+        },
+        'schema_path': args.schema,
+        'secrets_base_path': args.secrets_base_path
     }
 
 
-def default_cache_entry(path: str, prep: Callable) -> dict:
+def default_cache_entry(args: Namespace, prep: Callable) -> dict:
     """Create default topic entry."""
     return {
         'type': 'Cache',
-        'path': prep(path),
+        'path': prep(args.path),
         'conf': {}
     }
 
 
 def get_config_entry(config_path: str, args: Namespace) -> dict:
     """Update config file."""
     try:
@@ -107,16 +109,16 @@
         for _ in config
         if _.get(prop) == prep(key)
     }.get(key):
         return entry
 
     # If not found, create entry
     entry = (
-        default_topic_entry(args.name, prep) if args.action == 'topic'
-        else default_cache_entry(args.path, prep) if args.action == 'cache'
+        default_topic_entry(args, prep) if args.action == 'topic'
+        else default_cache_entry(args, prep) if args.action == 'cache'
         else {}
     )
     config.append(entry)
     with open(config_path, 'w') as f:
         dump(config, f, indent=4)
     return entry
 
@@ -138,46 +140,54 @@
     if regex and key:
         return bool(search(regex, key))
     if regex and not key:
         raise RuntimeError('Can\'t filter topic without keys.')
     return True
 
 
-def inspect_topic(conf: dict, args: Namespace):
+def inspect_topic(entry: dict, args: Namespace):
     """Read messages from topic."""
+    conf = entry['conf']
     if 'group.id' not in conf:
         conf['group.id'] = '$Default'
     if 'group.instance.id' not in conf:
         conf['group.instance.id'] = '$Default'
 
-    schema = AvroCodec(args.schema) if args.schema else None
+    start_time = dt.now(tz=timezone.utc)
+    schema_path = args.schema or entry.get('schema_path')
+    schema = AvroCodec(args.schema) if schema_path else None
     key_filter = curry(regex_filter)(args.key_filter)
     val_filter = curry(regex_filter)(args.val_filter)
 
     for msg in Topic(args.name, conf, args.offset, schema):
-        timestamp = (
-            dt
-            .fromtimestamp(msg.timestamp()[-1] / 1000, tz=timezone.utc)
-            .isoformat()
-            if msg.timestamp() else ''
-        )
+        if msg.timestamp():
+            timestamp = (
+                dt
+                .fromtimestamp(msg.timestamp()[-1] / 1000, tz=timezone.utc)
+            )
+            timestamp_str = timestamp.isoformat()
+        else:
+            timestamp, timestamp_str = None, ''
         key = msg.key().decode() if msg.key() is not None else ''
         offset = msg.offset()
         val = msg.value()
         if key_filter(str(key)) and val_filter(str(val)):  # pyright: ignore
             print()
-            print('>>> timestamp:', timestamp)
+            if timestamp and timestamp < start_time:
+                print('>>> timestamp:', timestamp_str, '(catching up)')
+            else:
+                print('>>> timestamp:', timestamp_str)
             print('>>> offset:', offset)
             print('>>> key:', key)
             print(val) if not args.columns else print({
                 k: v for k, v in val.items() if k in args.columns.split(',')
             })
 
 
-def inspect_cache(conf: dict, args: Namespace):
+def inspect_cache(entry: dict, args: Namespace):
     """Read records from cache."""
     if not path.isdir(args.path):
         raise OSError(f'Folder doesn\'t exist: {args.path}')
     cache = Cache(
         args.path,
         access_type=AccessType.read_only(),
     )
@@ -215,14 +225,14 @@
         entry = get_config_entry(config_path, args)
         entry = replace_variable_references(entry, args)
 
         # Call appropriate function with config and args
         {
             'topic': inspect_topic,
             'cache': inspect_cache,
-        }[args.action](entry['conf'], args)
+        }[args.action](entry, args)
     except KeyboardInterrupt:
         print('\nYou stopped the program.')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `snapstream-0.0.7/snapstream/caching.py` & `snapstream-0.0.8/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.7/snapstream/codecs.py` & `snapstream-0.0.8/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.7/snapstream/core.py` & `snapstream-0.0.8/snapstream/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,19 @@
     ) == 'false'
 
     while True:
         msg = c.poll(poll_timeout)
         if msg is None:
             continue
         if err := msg.error():
-            if raise_error:
+            if raise_error or err.fatal() or not err.retriable():
                 raise KafkaException(err)
+            else:
+                logger.error(msg.error())
+                continue
         if codec:
             decoded_val = codec.decode(msg.value())
             msg.set_value(decoded_val)
 
         yield msg
 
         if manual_commit:
@@ -262,15 +265,16 @@
         conf: dict = {},
         offset: Optional[int] = None,
         codec: Optional[ICodec] = None,
         flush_timeout: float = -1.0,
         poll_timeout: float = 1.0,
         pusher=_producer_handler,
         poller=_consumer_handler,
-        dry: bool = False
+        dry: bool = False,
+        raise_error: bool = False
     ) -> None:
         """Pass topic related configuration."""
         c = Conf()
         self.name = name
         self.conf = {**c.conf, **conf}
         self.starting_offset = offset
         self.flush_timeout = flush_timeout
@@ -278,14 +282,15 @@
         self.consumer = None
         self.producer = None
         self._producer_ctx = None
         self.pusher = pusher
         self.poller = poller
         self.codec = codec
         self.dry = dry
+        self.raise_error = raise_error
 
     def admin(self):
         """Get admin client."""
         return AdminClient(self.conf)
 
     def create_topic(self, *args, **kwargs) -> None:
         """Create topic."""
@@ -299,15 +304,16 @@
                     logger.warning(e)
                 else:
                     logger.error(e)
                     raise
 
     def __iter__(self) -> Iterator[Any]:
         """Consume from topic."""
-        c = get_consumer(self.name, self.conf, self.starting_offset, self.codec, self.poll_timeout, self.poller)
+        c = get_consumer(self.name, self.conf, self.starting_offset, self.codec,
+                         self.poll_timeout, self.poller, self.raise_error)
         with c as consumer:
             for msg in consumer:
                 yield msg
 
     def __next__(self) -> Any:
         """Consume next message from topic."""
         self.consumer = self.consumer or self.__iter__()
@@ -322,15 +328,16 @@
             None,
             i + 1 if i >= 0 else None
         ) if isinstance(i, int) else (
             i.start,
             i.step,
             i.stop
         )
-        c = get_consumer(self.name, self.conf, start, self.codec, self.poll_timeout, self.poller)
+        c = get_consumer(self.name, self.conf, start, self.codec,
+                         self.poll_timeout, self.poller, self.raise_error)
         with c as consumer:
             for msg in consumer:
                 if stop and msg.offset() >= stop:
                     return
                 if step and (msg.offset() - max(0, start)) % step != 0:
                     continue
                 yield msg
```

### Comparing `snapstream-0.0.7/snapstream/utils.py` & `snapstream-0.0.8/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.7/PKG-INFO` & `snapstream-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.7
+Version: 0.0.8
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

