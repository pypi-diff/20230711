# Comparing `tmp/recon_lw-2.0.0.dev5521630734.tar.gz` & `tmp/recon_lw-2.0.0.dev5521865947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5521630734.tar", last modified: Tue Jul 11 15:04:54 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5521865947.tar", last modified: Tue Jul 11 15:26:18 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5521630734.tar` & `recon_lw-2.0.0.dev5521865947.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-11 15:04:33.000000 recon_lw-2.0.0.dev5521630734/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35229 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:04:54.000000 recon_lw-2.0.0.dev5521630734/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-11 15:04:10.000000 recon_lw-2.0.0.dev5521630734/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-11 15:25:56.000000 recon_lw-2.0.0.dev5521865947/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35229 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:26:18.000000 recon_lw-2.0.0.dev5521865947/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-11 15:25:30.000000 recon_lw-2.0.0.dev5521865947/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/StateSequenceGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     current_state = self._state_cache[first_key]
                     updates_states = []
                     for o, key, new_key in o_lst:
                         updates_states.append((o,copy.deepcopy(current_state)))
                         self._state_update(o, current_state, self._create_event, self._send_events)
                     last_new_key = o_lst[-1][2]
                     if last_new_key is not None and last_new_key != chain_key:
-                        self._state_cache[last_new_key] = self._state_cache.pop(chain_key)
+                        self._state_cache[last_new_key] = self._state_cache.pop(first_key)
                     if self._debug:
                         body = {"ts_key" : ts_key, "chain_key": chain_key, "last_new_key": last_new_key, "stream": stream}
                         body["all_keys"] = {item[1] for item in o_lst}
                         body["all_new_keys"] = {item[2] for item in o_lst}
                         body["o_list"] = o_lst
                         ev = self._create_event("SSGDebug", "SSGDebug", True, body)
                         self._send_events([ev])
```

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5521865947/recon_lw/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5521865947/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/setup.py` & `recon_lw-2.0.0.dev5521865947/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5521630734/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5521865947/test/test_recon_ob.py`

 * *Files identical despite different names*

