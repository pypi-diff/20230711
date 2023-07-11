# Comparing `tmp/GMMA-1.2.0.tar.gz` & `tmp/GMMA-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GMMA-1.2.0.tar", last modified: Thu Jun 15 20:08:14 2023, max compression
+gzip compressed data, was "GMMA-1.2.1.tar", last modified: Tue Jul 11 00:18:14 2023, max compression
```

## Comparing `GMMA-1.2.0.tar` & `GMMA-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.421778 GMMA-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.417778 GMMA-1.2.0/GMMA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 20:08:02.000000 GMMA-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:08:14.421778 GMMA-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.421778 GMMA-1.2.0/gamma/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/_bayesian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/_gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/seismic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    17019 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:08:14.421778 GMMA-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 20:08:02.000000 GMMA-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.421778 GMMA-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-15 20:08:02.000000 GMMA-1.2.0/tests/test_seismoc_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.759226 GMMA-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.755226 GMMA-1.2.1/GMMA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 00:18:04.000000 GMMA-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 00:18:14.759226 GMMA-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.759226 GMMA-1.2.1/gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/_bayesian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/_gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/seismic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 00:18:14.759226 GMMA-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 00:18:04.000000 GMMA-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.759226 GMMA-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-11 00:18:05.000000 GMMA-1.2.1/tests/test_seismoc_ops.py
```

### Comparing `GMMA-1.2.0/LICENSE` & `GMMA-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.0/gamma/_base.py` & `GMMA-1.2.1/gamma/_base.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.0/gamma/_bayesian_mixture.py` & `GMMA-1.2.1/gamma/_bayesian_mixture.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.0/gamma/_gaussian_mixture.py` & `GMMA-1.2.1/gamma/_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.0/gamma/app.py` & `GMMA-1.2.1/gamma/app.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.0/gamma/seismic_ops.py` & `GMMA-1.2.1/gamma/seismic_ops.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.0/gamma/utils.py` & `GMMA-1.2.1/gamma/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # to_seconds = lambda t: datetime.strptime(t, "%Y-%m-%dT%H:%M:%S.%f").timestamp()
 # from_seconds = lambda t: [datetime.utcfromtimestamp(x).strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] for x in t]
 
 
 def convert_picks_csv(picks, stations, config):
     # t = picks["timestamp"].apply(lambda x: x.timestamp()).to_numpy()
     if type(picks["timestamp"].iloc[0]) is str:
-        picks.loc[:,"timestamp"] = picks["timestamp"].apply(lambda x: datetime.fromisoformat(x))
+        picks.loc[:, "timestamp"] = picks["timestamp"].apply(lambda x: datetime.fromisoformat(x))
     t = (
         picks["timestamp"]
         .apply(lambda x: x.tz_convert("UTC").timestamp() if x.tzinfo is not None else x.tz_localize("UTC").timestamp())
         .to_numpy()
     )
     # t = picks["timestamp"].apply(lambda x: x.timestamp()).to_numpy()
     timestamp0 = np.min(t)
@@ -52,14 +52,17 @@
 
 
 def association(picks, stations, config, event_idx0=0, method="BGMM", **kwargs):
     data, locs, phase_type, phase_weight, pick_idx, pick_station_id, timestamp0 = convert_picks_csv(
         picks, stations, config
     )
 
+    if len(data) < config["min_picks_per_eq"]:
+        return [], []
+
     vel = config["vel"] if "vel" in config else {"p": 6.0, "s": 6.0 / 1.73}
     if ("eikonal" not in config) or (config["eikonal"] is None):
         config["eikonal"] = None
     else:
         config["eikonal"] = initialize_eikonal(config["eikonal"])
 
     if ("use_dbscan" in config) and config["use_dbscan"]:
@@ -71,21 +74,20 @@
         unique_labels = set(labels)
         unique_labels = unique_labels.difference([-1])
     else:
         labels = np.zeros(len(data))
         unique_labels = [0]
 
     if "ncpu" not in config:
-        config["ncpu"] = max(1, min(len(unique_labels)//4, mp.cpu_count() - 1))
+        config["ncpu"] = max(1, min(len(unique_labels) // 4, mp.cpu_count() - 1))
 
-    if (config["ncpu"] == 1):
+    if config["ncpu"] == 1:
         print(f"Associating {len(data)} picks with {config['ncpu']} CPUs")
         event_idx = 0
-        events = []
-        assignment = []
+        events, assignment = [], []
         for unique_label in list(unique_labels):
             events_, assignment_ = associate(
                 unique_label,
                 labels,
                 data,
                 locs,
                 phase_type,
@@ -106,28 +108,28 @@
         lock = manager.Lock()
         # event_idx0 - 1 as event_idx is increased before use
         event_idx = manager.Value("i", event_idx0 - 1)
 
         print(f"Associating {len(unique_labels)} clusters with {config['ncpu']} CPUs")
 
         # the following sort and shuffle is to make sure jobs are distributed evenly
-        counter=Counter(labels)
+        counter = Counter(labels)
         unique_labels = sorted(unique_labels, key=lambda x: counter[x], reverse=True)
         np.random.shuffle(unique_labels)
 
         # the default chunk_size is len(unique_labels)//(config["ncpu"]*4), which makes some jobs very heavy
-        chunk_size = max(len(unique_labels)//(config["ncpu"]*20), 1)
-        
+        chunk_size = max(len(unique_labels) // (config["ncpu"] * 20), 1)
+
         # Check for OS to start a child process in multiprocessing
         # https://superfastpython.com/multiprocessing-context-in-python/
         if platform.system().lower() in ["darwin", "windows"]:
             context = "spawn"
         else:
             context = "fork"
-        
+
         with mp.get_context(context).Pool(config["ncpu"]) as p:
             results = p.starmap(
                 associate,
                 [
                     [
                         k,
                         labels,
@@ -146,20 +148,21 @@
                     ]
                     for k in unique_labels
                 ],
                 chunksize=chunk_size,
             )
             # resuts is a list of tuples, each tuple contains two lists events and assignment
             # here we flatten the list of tuples into two lists
-            events, assignment = [],[]
+            events, assignment = [], []
             for each_events, each_assignment in results:
                 events.extend(each_events)
                 assignment.extend(each_assignment)
 
-    return events, assignment # , event_idx.value
+    return events, assignment  # , event_idx.value
+
 
 def associate(
     k,
     labels,
     data,
     locs,
     phase_type,
@@ -170,21 +173,21 @@
     timestamp0,
     vel,
     method,
     event_idx,
     lock=None,
 ):
     print(".", end="")
-    
-    data_=data[labels==k]
-    locs_=locs[labels==k]
-    phase_type_=phase_type[labels==k]
-    phase_weight_=phase_weight[labels==k]
-    pick_idx_=pick_idx[labels==k]
-    pick_station_id_=pick_station_id[labels==k]
+
+    data_ = data[labels == k]
+    locs_ = locs[labels == k]
+    phase_type_ = phase_type[labels == k]
+    phase_weight_ = phase_weight[labels == k]
+    pick_idx_ = pick_idx[labels == k]
+    pick_station_id_ = pick_station_id[labels == k]
 
     max_num_event = max(Counter(pick_station_id_).values())
 
     if len(pick_idx_) < max(3, config["min_picks_per_eq"]):
         return [], []
 
     time_range = max(data_[:, 0].max() - data_[:, 0].min(), 1)
@@ -372,29 +375,39 @@
     if (np.prod(initial_points) * max_num_event * config["oversample_factor"]) > len(data_):
         initial_points = [1, 1, 1]
 
     x_init = np.linspace(config["x(km)"][0], config["x(km)"][1], initial_points[0] + 2)[1:-1]
     y_init = np.linspace(config["y(km)"][0], config["y(km)"][1], initial_points[1] + 2)[1:-1]
     z_init = np.linspace(config["z(km)"][0], config["z(km)"][1], initial_points[2] + 2)[1:-1]
     # z_init = np.linspace(config["z(km)"][0], config["z(km)"][1], initial_points[2]) + 1.0
+
+    ## manually set initial points
+    if "x_init" in config:
+        x_init = np.array(config["x_init"])
+    if "y_init" in config:
+        y_init = np.array(config["y_init"])
+    if "z_init" in config:
+        z_init = np.array(config["z_init"])
+
     x_init = np.broadcast_to(x_init[:, np.newaxis, np.newaxis], initial_points).reshape(-1)
     y_init = np.broadcast_to(y_init[np.newaxis, :, np.newaxis], initial_points).reshape(-1)
     z_init = np.broadcast_to(z_init[np.newaxis, np.newaxis, :], initial_points).reshape(-1)
 
     ## I found it helpful to add a point at the center of the area
     if (initial_points[0] == 2) and (initial_points[1] == 2):
         x_init = np.append(x_init, np.mean(config["x(km)"]))
         y_init = np.append(y_init, np.mean(config["y(km)"]))
         z_init = np.append(z_init, 0)
+
     num_xyz_init = len(x_init)
 
     # num_sta = len(np.unique(locs_, axis=0))
     # num_t_init = max(np.round(len(data_) / num_sta / num_xyz_init * config["oversample_factor"]), 1)
     # num_t_init = min(int(num_t_init), max(len(data_) // num_xyz_init, 1))
-    num_t_init = min(max_num_event * config["oversample_factor"], max(len(data_) // num_xyz_init, 1))
+    num_t_init = min(max(int(max_num_event * config["oversample_factor"]), 1), max(len(data_) // num_xyz_init, 1))
     t_init = np.sort(data_[:, 0])[:: max(len(data_) // num_t_init, 1)][:num_t_init]
     # t_init = np.linspace(
     #         data_[:, 0].min() - 0.1 * time_range,
     #         data_[:, 0].max() + 0.1 * time_range,
     #         num_t_init)
 
     x_init = np.broadcast_to(x_init[:, np.newaxis], (num_xyz_init, num_t_init)).reshape(-1)
@@ -410,29 +423,8 @@
         centers_init = np.vstack([x_init, t_init]).T
     else:
         raise (ValueError("Unsupported dims"))
 
     if config["use_amplitude"]:
         centers_init = np.hstack([centers_init, 1.0 * np.ones((len(centers_init), 1))])  # init magnitude to 1.0
 
-    # import matplotlib.pyplot as plt
-    # plt.figure()
-    # plt.scatter(x_init, y_init)
-    # plt.savefig("initial_points_xy.png")
-    # plt.figure()
-    # plt.scatter(x_init, z_init)
-    # plt.savefig("initial_points_xz.png")
-    # plt.figure()
-    # plt.scatter(y_init, z_init)
-    # plt.savefig("initial_points_yz.png")
-
-    # plt.figure()
-    # plt.scatter(t_init, x_init)
-    # plt.savefig("initial_points_tx.png")
-    # plt.figure()
-    # plt.scatter(t_init, y_init)
-    # plt.savefig("initial_points_ty.png")
-    # plt.figure()
-    # plt.scatter(t_init, z_init)
-    # plt.savefig("initial_points_tz.png")
-
     return centers_init
```

### Comparing `GMMA-1.2.0/tests/test_seismoc_ops.py` & `GMMA-1.2.1/tests/test_seismoc_ops.py`

 * *Files identical despite different names*

