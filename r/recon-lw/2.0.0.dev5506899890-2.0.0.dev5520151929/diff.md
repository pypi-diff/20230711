# Comparing `tmp/recon_lw-2.0.0.dev5506899890.tar.gz` & `tmp/recon_lw-2.0.0.dev5520151929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5506899890.tar", last modified: Mon Jul 10 10:20:32 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5520151929.tar", last modified: Tue Jul 11 12:52:01 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5506899890.tar` & `recon_lw-2.0.0.dev5520151929.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-10 10:20:14.000000 recon_lw-2.0.0.dev5506899890/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35229 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-11 12:51:37.000000 recon_lw-2.0.0.dev5520151929/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4277 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35229 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 12:52:01.000000 recon_lw-2.0.0.dev5520151929/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-11 12:51:09.000000 recon_lw-2.0.0.dev5520151929/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/StateSequenceGenerator.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._state_cache = {}
         self._streams = {}
 
         self._create_event = create_event
         self._send_events = send_events
         self._horizon_delay_seconds = horizon_delay_seconds
         self._custom_settings = custom_settings
-        self._debug = False
+        self._debug = True
 
     def process_objects_batch(self, batch: list) -> None:
         current_ts = None
         #add to sequence streams
         for o in batch:
             stream, seq, ts = self._stream_sequence_timestamp_extract(o)
             if stream is not None:
@@ -37,15 +37,15 @@
                 current_ts = ts
                 self._streams[stream].add_object(seq, ts, o)
                 
         #flush old records
         self.process_streams(current_ts)
     
     def process_streams(self, current_ts):
-        for stream_cache in self._streams.values():
+        for stream, stream_cache in self._streams.items():
             next_chunk = stream_cache.get_next_chunk(current_ts)
             processed = 0
             arranged = {}
             chains = {}
             for o in next_chunk:
                 key , ts, new_key = self._object_key_ts_extract(o)
                 if key is not None:
@@ -56,15 +56,15 @@
                     if key in chains:
                         chained_key = chains[key]                        
                     if new_key is not None and new_key != key:
                         chains[new_key] = chained_key
                     if key not in arranged[ts_key]:
                         arranged[ts_key][chained_key] = [(o, key, new_key)]
                     else:
-                        arranged[ts_key][chained_key].append(o, key, new_key)
+                        arranged[ts_key][chained_key].append((o, key, new_key))
                 processed += 1
 
             tss = list(arranged.keys())
             tss.sort()
             for ts_key in tss:
                 for chain_key, o_lst in arranged[ts_key].items():
                     if chain_key not in self._state_cache:
@@ -74,13 +74,22 @@
                     for o, key, new_key in o_lst:
                         updates_states.append((o,copy.deepcopy(current_state)))
                         self._state_update(o, current_state, self._create_event, self._send_events)
                     if len(o_lst) > 0:
                         last_new_key = o_lst[-1][2]
                         if last_new_key is not None and last_new_key != chain_key:
                             self._state_cache[last_new_key] = self._state_cache.pop(chain_key)
+                        if self._debug:
+                            body = {"ts_key" : ts_key, "chain_key": chain_key, "last_new_key": last_new_key, "stream": stream}
+                            body["all_keys"] = {item[1] for item in o_lst}
+                            body["all_new_keys"] = {item[2] for item in o_lst}
+                            body["o_list"] = o_lst
+                            ev = self._create_event("SSGDebug", "SSGDebug", True, body)
+                            self._send_events([ev])
+
                     self._report_images(updates_states, self._create_event, self._send_events)
+        
             stream_cache.clear_processed_chunk(processed)
 
 
     def flush_all(self) -> None:
         self.process_streams(None)
```

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5520151929/recon_lw/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5520151929/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/setup.py` & `recon_lw-2.0.0.dev5520151929/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5506899890/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5520151929/test/test_recon_ob.py`

 * *Files identical despite different names*

