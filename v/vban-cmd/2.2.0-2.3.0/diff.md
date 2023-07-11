# Comparing `tmp/vban_cmd-2.2.0.tar.gz` & `tmp/vban_cmd-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.2.0.tar", max compression
+gzip compressed data, was "vban_cmd-2.3.0.tar", max compression
```

## Comparing `vban_cmd-2.2.0.tar` & `vban_cmd-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.2.0/LICENSE
--rw-r--r--   0        0        0      951 2023-07-08 06:34:03.457702 vban_cmd-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    11605 2023-07-05 13:04:56.374532 vban_cmd-2.2.0/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.2.0/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.2.0/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.2.0/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban_cmd-2.2.0/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.2.0/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.2.0/vban_cmd/event.py
--rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.2.0/vban_cmd/factory.py
--rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.2.0/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.2.0/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.2.0/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.2.0/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.2.0/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.2.0/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.2.0/vban_cmd/subject.py
--rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.2.0/vban_cmd/util.py
--rw-r--r--   0        0        0     4320 2023-07-08 06:27:12.206963 vban_cmd-2.2.0/vban_cmd/vban.py
--rw-r--r--   0        0        0     6915 2023-07-08 07:08:39.810087 vban_cmd-2.2.0/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.2.0/vban_cmd/worker.py
--rw-r--r--   0        0        0    11763 1970-01-01 00:00:00.000000 vban_cmd-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.0/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-11 17:25:21.228891 vban_cmd-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12527 2023-07-11 18:49:38.369576 vban_cmd-2.3.0/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.0/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.0/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.0/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.0/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.0/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.0/vban_cmd/event.py
+-rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.0/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.3.0/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.3.0/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.3.0/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.0/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.3.0/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.0/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.0/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.3.0/vban_cmd/util.py
+-rw-r--r--   0        0        0     4320 2023-07-08 06:27:12.206963 vban_cmd-2.3.0/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7280 2023-07-11 17:55:51.111211 vban_cmd-2.3.0/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.3.0/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12664 1970-01-01 00:00:00.000000 vban_cmd-2.3.0/PKG-INFO
```

### Comparing `vban_cmd-2.2.0/LICENSE` & `vban_cmd-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/pyproject.toml` & `vban_cmd-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.2.0"
+version = "2.3.0"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.2.0/README.md` & `vban_cmd-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ```toml
 [connection]
 ip = "gamepc.local"
 port = 6980
 streamname = "Command1"
 ```
 
-It should be placed next to your `__main__.py` file.
+It should be placed in \<user home directory\> / "Documents" / "Voicemeeter" / "configs"
 
 Alternatively you may pass `ip`, `port`, `streamname` as keyword arguments.
 
 #### `__main__.py`
 
 Simplest use case, use a context manager to request a VbanCmd class of a kind.
 
@@ -355,34 +355,55 @@
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
-vban.strip[0].apply(mute: true, gain: 3.2, A1: true)
-vban.bus[0].apply(A1: true)
+vban.strip[0].apply({"mute": True, "gain": 3.2, "A1": True})
+vban.vban.outstream[0].apply({"on": True, "name": "streamname", "bit": 24})
 ```
 
 ## Config Files
 
 `vban.apply_config(<configname>)`
 
 You may load config files in TOML format.
 Three example configs have been included with the package. Remember to save
-current settings before loading a user config. To set one you may do:
+current settings before loading a user config. To load one you may do:
 
 ```python
 import vban_cmd
 with vban_cmd.api('banana') as vban:
     vban.apply_config('example')
 ```
 
 will load a config file at configs/banana/example.toml for Voicemeeter Banana.
 
+Your configs may be located in one of the following paths:
+-   \<current working directory\> / "configs" / kind_id
+-   \<user home directory\> / ".config" / "vban-cmd" / kind_id
+-   \<user home directory\> / "Documents" / "Voicemeeter" / "configs" / kind_id
+
+If a config with the same name is located in multiple locations, only the first one found is loaded into memory, in the above order.
+
+#### `config extends`
+
+You may also load a config that extends another config with overrides or additional parameters.
+
+You just need to define a key `extends` in the config TOML, that names the config to be extended.
+
+Three example 'extender' configs are included with the repo. You may load them with:
+
+```python
+import voicemeeterlib
+with voicemeeterlib.api('banana') as vm:
+    vm.apply_config('extender')
+```
+
 ## Events
 
 Level updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.
 
 example:
 
 ```python
```

### Comparing `vban_cmd-2.2.0/vban_cmd/bus.py` & `vban_cmd-2.3.0/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/command.py` & `vban_cmd-2.3.0/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/config.py` & `vban_cmd-2.3.0/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/event.py` & `vban_cmd-2.3.0/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/factory.py` & `vban_cmd-2.3.0/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/iremote.py` & `vban_cmd-2.3.0/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/kinds.py` & `vban_cmd-2.3.0/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/macrobutton.py` & `vban_cmd-2.3.0/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/meta.py` & `vban_cmd-2.3.0/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/packet.py` & `vban_cmd-2.3.0/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/strip.py` & `vban_cmd-2.3.0/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/subject.py` & `vban_cmd-2.3.0/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/util.py` & `vban_cmd-2.3.0/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/vban.py` & `vban_cmd-2.3.0/vban_cmd/vban.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/vban_cmd/vbancmd.py` & `vban_cmd-2.3.0/vban_cmd/vbancmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,30 +60,30 @@
             import tomllib
         except ModuleNotFoundError:
             import tomli as tomllib
 
         def get_filepath():
             filepaths = [
                 Path.cwd() / "vban.toml",
+                Path.cwd() / "configs" / "vban.toml",
                 Path.home() / ".config" / "vban-cmd" / "vban.toml",
-                Path.home() / "Documents" / "Voicemeeter" / "vban.toml",
+                Path.home() / "Documents" / "Voicemeeter" / "configs" / "vban.toml",
             ]
             for filepath in filepaths:
                 if filepath.exists():
                     return filepath
 
         if filepath := get_filepath():
             with open(filepath, "rb") as f:
                 conn = tomllib.load(f)
                 assert (
-                    "ip" in conn["connection"]
-                ), "please provide ip, by kwarg or config"
+                    "connection" in conn and "ip" in conn["connection"]
+                ), "expected [connection][ip] in vban config"
             return conn["connection"]
-        else:
-            raise VBANCMDError("no ip provided and no vban.toml located.")
+        raise VBANCMDError("no ip provided and no vban.toml located.")
 
     def __enter__(self):
         self.login()
         return self
 
     def login(self):
         """Starts the subscriber and updater threads (unless in outbound mode)"""
@@ -97,15 +97,15 @@
             queue = Queue()
             self.updater = Updater(self, queue)
             self.updater.start()
             self.producer = Producer(self, queue)
             self.producer.start()
 
         self.logger.info(
-            "Successfully logged into {kind} with ip='{ip}', port={port}, streamname='{streamname}'".format(
+            "Successfully logged into VBANCMD {kind} with ip='{ip}', port={port}, streamname='{streamname}'".format(
                 **self.__dict__
             )
         )
 
     def _set_rt(self, cmd: str, val: Union[str, float]):
         """Sends a string request command over a network."""
         self.socks[Socket.request].sendto(
@@ -185,24 +185,32 @@
                 return getattr(getattr(self, obj), f"{m2}stream")[index]
             raise ValueError(obj)
 
         [param(key).apply(datum).then_wait() for key, datum in data.items()]
 
     def apply_config(self, name):
         """applies a config from memory"""
-        error_msg = (
+        ERR_MSG = (
             f"No config with name '{name}' is loaded into memory",
             f"Known configs: {list(self.configs.keys())}",
         )
         try:
-            self.apply(self.configs[name])
-            self.logger.info(f"Profile '{name}' applied!")
+            config = self.configs[name].copy()
         except KeyError as e:
-            self.logger.error(("\n").join(error_msg))
-            raise VBANCMDError(("\n").join(error_msg)) from e
+            self.logger.error(("\n").join(ERR_MSG))
+            raise VBANCMDError(("\n").join(ERR_MSG)) from e
+
+        if "extends" in config:
+            extended = config.pop("extends")
+            config = self.configs[extended] | config
+            self.logger.debug(
+                f"profile '{name}' extends '{extended}', profiles merged.."
+            )
+        self.apply(config)
+        self.logger.info(f"Profile '{name}' applied!")
 
     def logout(self):
         self.running = False
         time.sleep(0.2)
         [sock.close() for sock in self.socks]
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
```

### Comparing `vban_cmd-2.2.0/vban_cmd/worker.py` & `vban_cmd-2.3.0/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.2.0/PKG-INFO` & `vban_cmd-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -57,15 +57,15 @@
 ```toml
 [connection]
 ip = "gamepc.local"
 port = 6980
 streamname = "Command1"
 ```
 
-It should be placed next to your `__main__.py` file.
+It should be placed in \<user home directory\> / "Documents" / "Voicemeeter" / "configs"
 
 Alternatively you may pass `ip`, `port`, `streamname` as keyword arguments.
 
 #### `__main__.py`
 
 Simplest use case, use a context manager to request a VbanCmd class of a kind.
 
@@ -372,34 +372,55 @@
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
-vban.strip[0].apply(mute: true, gain: 3.2, A1: true)
-vban.bus[0].apply(A1: true)
+vban.strip[0].apply({"mute": True, "gain": 3.2, "A1": True})
+vban.vban.outstream[0].apply({"on": True, "name": "streamname", "bit": 24})
 ```
 
 ## Config Files
 
 `vban.apply_config(<configname>)`
 
 You may load config files in TOML format.
 Three example configs have been included with the package. Remember to save
-current settings before loading a user config. To set one you may do:
+current settings before loading a user config. To load one you may do:
 
 ```python
 import vban_cmd
 with vban_cmd.api('banana') as vban:
     vban.apply_config('example')
 ```
 
 will load a config file at configs/banana/example.toml for Voicemeeter Banana.
 
+Your configs may be located in one of the following paths:
+-   \<current working directory\> / "configs" / kind_id
+-   \<user home directory\> / ".config" / "vban-cmd" / kind_id
+-   \<user home directory\> / "Documents" / "Voicemeeter" / "configs" / kind_id
+
+If a config with the same name is located in multiple locations, only the first one found is loaded into memory, in the above order.
+
+#### `config extends`
+
+You may also load a config that extends another config with overrides or additional parameters.
+
+You just need to define a key `extends` in the config TOML, that names the config to be extended.
+
+Three example 'extender' configs are included with the repo. You may load them with:
+
+```python
+import voicemeeterlib
+with voicemeeterlib.api('banana') as vm:
+    vm.apply_config('extender')
+```
+
 ## Events
 
 Level updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.
 
 example:
 
 ```python
```

