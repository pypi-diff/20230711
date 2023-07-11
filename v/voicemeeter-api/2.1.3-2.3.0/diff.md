# Comparing `tmp/voicemeeter_api-2.1.3.tar.gz` & `tmp/voicemeeter_api-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.1.3.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.3.0.tar", max compression
```

## Comparing `voicemeeter_api-2.1.3.tar` & `voicemeeter_api-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.1.3/LICENSE
--rw-r--r--   0        0        0     1111 2023-07-09 00:45:16.686090 voicemeeter_api-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    17394 2023-07-01 19:24:29.927689 voicemeeter_api-2.1.3/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.1.3/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.1.3/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter_api-2.1.3/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.1.3/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.1.3/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.1.3/voicemeeterlib/device.py
--rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter_api-2.1.3/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.1.3/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.1.3/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.1.3/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.1.3/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.1.3/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.1.3/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.1.3/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-01 18:51:25.725768 voicemeeter_api-2.1.3/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.1.3/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    11192 2023-07-09 00:42:36.890657 voicemeeter_api-2.1.3/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.1.3/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.1.3/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter_api-2.1.3/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.1.3/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.1.3/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17226 1970-01-01 00:00:00.000000 voicemeeter_api-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1102 2023-07-11 17:25:08.856740 voicemeeter_api-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18140 2023-07-11 17:21:40.302191 voicemeeter_api-2.3.0/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.0/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.3.0/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.0/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.0/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.0/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.0/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.0/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.0/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.0/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.0/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.0/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.3.0/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.3.0/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.0/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.0/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.0/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12109 2023-07-11 16:45:26.140521 voicemeeter_api-2.3.0/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.3.0/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.0/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2978 2023-07-10 02:00:50.034407 voicemeeter_api-2.3.0/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.3.0/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.3.0/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17953 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.0/PKG-INFO
```

### Comparing `voicemeeter_api-2.1.3/LICENSE` & `voicemeeter_api-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/pyproject.toml` & `voicemeeter_api-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.1.3"
+version = "2.3.0"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
-packages = [
-    { include = "voicemeeterlib" },
-]
+packages = [{ include = "voicemeeterlib" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```

### Comparing `voicemeeter_api-2.1.3/README.md` & `voicemeeter_api-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -697,23 +697,42 @@
 
 ## Config Files
 
 `vm.apply_config(configname)`
 
 You may load config files in TOML format.
 Three example configs have been included with the package. Remember to save
-current settings before loading a user config. To set one you may do:
+current settings before loading a user config. To load one you may do:
 
 ```python
 import voicemeeterlib
 with voicemeeterlib.api('banana') as vm:
     vm.apply_config('example')
 ```
 
-will load a user config file at configs/banana/example.toml for Voicemeeter Banana.
+Your configs may be located in one of the following paths:
+-   \<current working directory\> / "configs" / kind_id
+-   \<user home directory\> / ".config" / "voicemeeter" / kind_id
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
 
 ## Events
 
 By default, NO events are listened for. Use events kwargs to enable specific event types.
 
 example:
```

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/bus.py` & `voicemeeter_api-2.3.0/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.3.0/voicemeeterlib/cbindings.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class CBindings(metaclass=ABCMeta):
     """
     C bindings defined here.
 
     Maps expected ctype argument and res types for each binding.
     """
 
-    logger_cbindings = logger.getChild("Cbindings")
+    logger_cbindings = logger.getChild("CBindings")
 
     vm_login = libc.VBVMR_Login
     vm_login.restype = LONG
     vm_login.argtypes = None
 
     vm_logout = libc.VBVMR_Logout
     vm_logout.restype = LONG
@@ -112,14 +112,14 @@
     vm_get_midi_message.argtypes = [ct.POINTER(CHAR * 1024), LONG]
 
     def call(self, func, *args, ok=(0,), ok_exp=None):
         try:
             res = func(*args)
             if ok_exp is None:
                 if res not in ok:
-                    raise CAPIError(f"{func.__name__} returned {res}")
-            elif not ok_exp(res):
-                raise CAPIError(f"{func.__name__} returned {res}")
+                    raise CAPIError(func.__name__, res)
+            elif not ok_exp(res) and res not in ok:
+                raise CAPIError(func.__name__, res)
             return res
         except CAPIError as e:
-            self.logger_cbindings.exception(f"{type(e).__name__}: {e}")
+            self.logger_cbindings.exception(str(e))
             raise
```

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/command.py` & `voicemeeter_api-2.3.0/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/config.py` & `voicemeeter_api-2.3.0/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/device.py` & `voicemeeter_api-2.3.0/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/event.py` & `voicemeeter_api-2.3.0/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/factory.py` & `voicemeeter_api-2.3.0/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/inst.py` & `voicemeeter_api-2.3.0/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/iremote.py` & `voicemeeter_api-2.3.0/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/kinds.py` & `voicemeeter_api-2.3.0/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.3.0/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/meta.py` & `voicemeeter_api-2.3.0/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/misc.py` & `voicemeeter_api-2.3.0/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/recorder.py` & `voicemeeter_api-2.3.0/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/remote.py` & `voicemeeter_api-2.3.0/voicemeeterlib/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,20 @@
     @property
     def mdirty(self) -> bool:
         """True iff MB parameters have been updated."""
         try:
             return self.call(self.vm_mdirty, ok=(0, 1)) == 1
         except AttributeError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
+            ERR_MSG = (
+                "no bind for VBVMR_MacroButton_IsDirty.",
+                "are you using an old version of the API?",
+            )
             raise CAPIError(
-                "no bind for VBVMR_MacroButton_IsDirty. are you using an old version of the API?"
+                "VBVMR_MacroButton_IsDirty", -9, msg=" ".join(ERR_MSG)
             ) from e
 
     @property
     def ldirty(self) -> bool:
         """True iff levels have been updated."""
         self._strip_buf, self._bus_buf = self._get_levels()
         return not (
@@ -129,16 +133,18 @@
             and self.cache.get("bus_level") == self._bus_buf
         )
 
     def clear_dirty(self) -> NoReturn:
         try:
             while self.pdirty or self.mdirty:
                 pass
-        except CAPIError:
-            self.logger.error("no bind for mdirty, clearing pdirty only")
+        except CAPIError as e:
+            if not (e.fn_name == "VBVMR_MacroButton_IsDirty" and e.code == -9):
+                raise
+            self.logger.error(f"{e} clearing pdirty only.")
             while self.pdirty:
                 pass
 
     @polling
     def get(self, param: str, is_string: Optional[bool] = False) -> Union[str, float]:
         """Gets a string or float parameter"""
         if is_string:
@@ -170,28 +176,36 @@
                 self.vm_get_buttonstatus,
                 ct.c_long(id),
                 ct.byref(state),
                 ct.c_long(mode),
             )
         except AttributeError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
+            ERR_MSG = (
+                "no bind for VBVMR_MacroButton_GetStatus.",
+                "are you using an old version of the API?",
+            )
             raise CAPIError(
-                "no bind for VBVMR_MacroButton_GetStatus. are you using an old version of the API?"
+                "VBVMR_MacroButton_GetStatus", -9, msg=" ".join(ERR_MSG)
             ) from e
         return int(state.value)
 
     def set_buttonstatus(self, id: int, state: int, mode: int) -> NoReturn:
         """Sets a macrobutton parameter. Caches value"""
         c_state = ct.c_float(float(state))
         try:
             self.call(self.vm_set_buttonstatus, ct.c_long(id), c_state, ct.c_long(mode))
         except AttributeError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
+            ERR_MSG = (
+                "no bind for VBVMR_MacroButton_SetStatus.",
+                "are you using an old version of the API?",
+            )
             raise CAPIError(
-                "no bind for VBVMR_MacroButton_SetStatus. are you using an old version of the API?"
+                "VBVMR_MacroButton_SetStatus", -9, msg=" ".join(ERR_MSG)
             ) from e
         self.cache[f"mb_{id}_{mode}"] = int(c_state.value)
 
     def get_num_devices(self, direction: str = None) -> int:
         """Retrieves number of physical devices connected"""
         if direction not in ("in", "out"):
             raise VMError("Expected a direction: in or out")
@@ -236,15 +250,21 @@
                 for i in range(8 * (self.kind.phys_out + self.kind.virt_out))
             ),
         )
 
     def get_midi_message(self):
         n = ct.c_long(1024)
         buf = ct.create_string_buffer(1024)
-        res = self.vm_get_midi_message(ct.byref(buf), n, ok_exp=lambda r: r >= 0)
+        res = self.call(
+            self.vm_get_midi_message,
+            ct.byref(buf),
+            n,
+            ok=(-5, -6),  # no data received from midi device
+            ok_exp=lambda r: r >= 0,
+        )
         if res > 0:
             vals = tuple(
                 grouper(3, (int.from_bytes(buf[i], "little") for i in range(res)))
             )
             for msg in vals:
                 ch, pitch, vel = msg
                 if not self.midi._channel or self.midi._channel != ch:
@@ -277,24 +297,32 @@
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
-            raise VMError(("\n").join(error_msg)) from e
+            self.logger.error(("\n").join(ERR_MSG))
+            raise VMError(("\n").join(ERR_MSG)) from e
+
+        if "extends" in config:
+            extended = config.pop("extends")
+            config = self.configs[extended] | config
+            self.logger.debug(
+                f"profile '{name}' extends '{extended}', profiles merged.."
+            )
+        self.apply(config)
+        self.logger.info(f"Profile '{name}' applied!")
 
     def logout(self) -> NoReturn:
         """Wait for dirty parameters to clear, then logout of the API"""
         self.clear_dirty()
         time.sleep(0.1)
         self.call(self.vm_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
```

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/strip.py` & `voicemeeter_api-2.3.0/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/subject.py` & `voicemeeter_api-2.3.0/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/updater.py` & `voicemeeter_api-2.3.0/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/util.py` & `voicemeeter_api-2.3.0/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/voicemeeterlib/vban.py` & `voicemeeter_api-2.3.0/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.3/PKG-INFO` & `voicemeeter_api-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.1.3
+Version: 2.3.0
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -714,23 +714,42 @@
 
 ## Config Files
 
 `vm.apply_config(configname)`
 
 You may load config files in TOML format.
 Three example configs have been included with the package. Remember to save
-current settings before loading a user config. To set one you may do:
+current settings before loading a user config. To load one you may do:
 
 ```python
 import voicemeeterlib
 with voicemeeterlib.api('banana') as vm:
     vm.apply_config('example')
 ```
 
-will load a user config file at configs/banana/example.toml for Voicemeeter Banana.
+Your configs may be located in one of the following paths:
+-   \<current working directory\> / "configs" / kind_id
+-   \<user home directory\> / ".config" / "voicemeeter" / kind_id
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
 
 ## Events
 
 By default, NO events are listened for. Use events kwargs to enable specific event types.
 
 example:
```

