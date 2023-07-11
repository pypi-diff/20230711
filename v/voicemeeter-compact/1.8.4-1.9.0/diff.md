# Comparing `tmp/voicemeeter_compact-1.8.4.tar.gz` & `tmp/voicemeeter_compact-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_compact-1.8.4.tar", max compression
+gzip compressed data, was "voicemeeter_compact-1.9.0.tar", max compression
```

## Comparing `voicemeeter_compact-1.8.4.tar` & `voicemeeter_compact-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.8.4/LICENSE
--rw-r--r--   0        0        0      730 2023-07-07 23:22:00.757305 voicemeeter_compact-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter_compact-1.8.4/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.8.4/vmcompact/__init__.py
--rw-r--r--   0        0        0     4685 2023-07-07 21:33:25.991940 voicemeeter_compact-1.8.4/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.8.4/vmcompact/banner.py
--rw-r--r--   0        0        0    23309 2023-07-05 22:29:08.031736 voicemeeter_compact-1.8.4/vmcompact/builders.py
--rw-r--r--   0        0        0    10867 2023-07-05 23:06:46.459871 voicemeeter_compact-1.8.4/vmcompact/channels.py
--rw-r--r--   0        0        0     9634 2023-07-05 22:31:26.458658 voicemeeter_compact-1.8.4/vmcompact/config.py
--rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.8.4/vmcompact/configurations.py
--rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.8.4/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.8.4/vmcompact/errors.py
--rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter_compact-1.8.4/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.8.4/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    16815 2023-07-07 17:15:19.541901 voicemeeter_compact-1.8.4/vmcompact/menu.py
--rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.8.4/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.8.4/vmcompact/subject.py
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.9.0/LICENSE
+-rw-r--r--   0        0        0      730 2023-07-10 19:52:01.330626 voicemeeter_compact-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6125 2023-07-10 03:18:55.019093 voicemeeter_compact-1.9.0/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.9.0/vmcompact/__init__.py
+-rw-r--r--   0        0        0     6246 2023-07-11 07:31:35.433343 voicemeeter_compact-1.9.0/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.9.0/vmcompact/banner.py
+-rw-r--r--   0        0        0    23962 2023-07-10 23:26:02.030414 voicemeeter_compact-1.9.0/vmcompact/builders.py
+-rw-r--r--   0        0        0    11135 2023-07-10 23:59:51.207793 voicemeeter_compact-1.9.0/vmcompact/channels.py
+-rw-r--r--   0        0        0     9852 2023-07-10 23:14:22.369555 voicemeeter_compact-1.9.0/vmcompact/config.py
+-rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.9.0/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.9.0/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.9.0/vmcompact/errors.py
+-rw-r--r--   0        0        0     9178 2023-07-10 23:25:00.326724 voicemeeter_compact-1.9.0/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.9.0/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    16901 2023-07-10 22:04:53.242069 voicemeeter_compact-1.9.0/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.9.0/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.9.0/vmcompact/subject.py
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.9.0/PKG-INFO
```

### Comparing `voicemeeter_compact-1.8.4/LICENSE` & `voicemeeter_compact-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/pyproject.toml` & `voicemeeter_compact-1.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.8.4"
+version = "1.9.0"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
 include = ["vmcompact/img/cat.ico"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sv-ttk = "^2.5.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
-voicemeeter-api = "^2.0.2"
-vban-cmd = "^2.0.0"
+voicemeeter-api = "^2.1.2"
+vban-cmd = "^2.2.0"
 
 [tool.poetry.dev-dependencies]
 black = { version = "^22.6.0", allow-prereleases = true }
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `voicemeeter_compact-1.8.4/README.md` & `voicemeeter_compact-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,36 +30,36 @@
 
 ```python
 import voicemeeterlib
 import vmcompact
 
 
 def main():
-    # pass the kind_id and the vm object to the app
-    with voicemeeterlib.api(kind_id) as vm:
-        app = vmcompact.connect(kind_id, vm)
+    # choose the kind of Voicemeeter (Local connection)
+    KIND_ID = "banana"
+
+    # pass the KIND_ID and the vm object to the app
+    with voicemeeterlib.api(KIND_ID) as vm:
+        app = vmcompact.connect(KIND_ID, vm)
         app.mainloop()
 
 
 if __name__ == "__main__":
-    # choose the kind of Voicemeeter (Local connection)
-    kind_id = "banana"
-
     main()
 ```
 
 It's important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.
 
 ![Image of unlabelled app](./doc_imgs/nolabels.png)
 
 If the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).
 
-### kind_id
+### KIND_ID
 
-Set the kind of Voicemeeter, kind_id may be:
+Set the kind of Voicemeeter, KIND_ID may be:
 
 -   `basic`
 -   `banana`
 -   `potato`
 
 ## TOML Files
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/app.py` & `voicemeeter_compact-1.9.0/vmcompact/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import tkinter as tk
 from functools import cached_property
 from pathlib import Path
-from tkinter import ttk
+from tkinter import messagebox, ttk
 from typing import NamedTuple
 
+import voicemeeterlib
+
 from .builders import MainFrameBuilder
 from .configurations import loader
-from .data import _base_values, _configuration, _kinds_all
+from .data import _base_values, _configuration, _kinds_all, get_configuration
 from .errors import VMCompactError
 from .menu import Menus
 from .subject import Subject
 
 logger = logging.getLogger(__name__)
 
 
@@ -44,29 +46,25 @@
         self._vmr.init_thread()
         icon_path = Path(__file__).parent.resolve() / "img" / "cat.ico"
         if icon_path.is_file():
             self.iconbitmap(str(icon_path))
         self.minsize(275, False)
         self.subject = Subject()
         self._configs = None
-        self["menu"] = Menus(self, vmr)
+        self.menu = self["menu"] = Menus(self, vmr)
         self.styletable = ttk.Style()
         if _configuration.config:
             vmr.apply_config(_configuration.config)
 
         self.build_app()
 
         self.drag_id = ""
         self.bind("<Configure>", self.dragging)
 
-    def start_updates(self):
-        self.logger.debug("updates started")
-        _base_values.run_update = True
-        if self._vmr.gui.launched_by_api:
-            self.on_pdirty()
+        self.after(1, self.healthcheck_step)
 
     def __str__(self):
         return f"{type(self).__name__}App"
 
     @property
     def target(self):
         """returns the current interface"""
@@ -144,14 +142,50 @@
         _base_values.dragging = False
 
     @cached_property
     def userconfigs(self):
         self._configs = loader(self.kind.name, self.target)
         return self._configs
 
+    def start_updates(self):
+        self.logger.debug("updates started")
+        _base_values.run_update = True
+        if self._vmr.gui.launched_by_api:
+            self.on_pdirty()
+
+    def healthcheck_step(self):
+        if not _base_values.vban_connected:
+            try:
+                self._vmr.pdirty
+            except voicemeeterlib.error.CAPIError:
+                resp = messagebox.askyesno(message="Restart Voicemeeter GUI?")
+                if resp:
+                    self.logger.debug(
+                        "healthcheck failed, rebuilding the app after GUI restart."
+                    )
+                    self._vmr.end_thread()
+                    self._vmr.run_voicemeeter(self._vmr.kind.name)
+                    _base_values.run_update = False
+                    self._vmr.init_thread()
+                    self.after(8000, self.start_updates)
+                    self._destroy_top_level_frames()
+                    self.build_app(self._vmr.kind)
+                    vban_config = get_configuration("vban")
+                    for i, _ in enumerate(vban_config):
+                        target = getattr(self.menu, f"menu_vban_{i+1}")
+                        target.entryconfig(0, state="normal")
+                        target.entryconfig(1, state="disabled")
+                    [
+                        self.menu.menu_vban.entryconfig(j, state="normal")
+                        for j, _ in enumerate(self.menu.menu_vban.winfo_children())
+                    ]
+                else:
+                    self.destroy()
+        self.after(250, self.healthcheck_step)
+
 
 _apps = {kind.name: App.make(kind) for kind in _kinds_all}
 
 
 def connect(kind_id: str, vmr) -> App:
     """return App of the kind requested"""
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/banner.py` & `voicemeeter_compact-1.9.0/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/vmcompact/builders.py` & `voicemeeter_compact-1.9.0/vmcompact/builders.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,29 +245,35 @@
             command=self.labelframe.scale_callback,
             length=_configuration.channel_height,
         )
         self.scale.grid(column=1, row=0)
         self.scale.bind("<Double-Button-1>", self.labelframe.reset_gain)
         self.scale.bind("<Button-1>", self.labelframe.scale_press)
         self.scale.bind("<ButtonRelease-1>", self.labelframe.scale_release)
-        self.scale.bind("<MouseWheel>", self.labelframe._on_mousewheel)
+        self.scale.bind(
+            "<MouseWheel>",
+            partial(
+                self.labelframe.pause_updates,
+                self.labelframe._on_mousewheel,
+            ),
+        )
 
     def add_gain_label(self):
         self.labelframe.gain_label = ttk.Label(
             self.labelframe,
             textvariable=self.labelframe.gainlabel,
         )
         self.labelframe.gain_label.grid(column=0, row=1, columnspan=2)
 
     def add_mute_button(self):
         """Adds a mute button widget to a single label frame"""
         self.button_mute = ttk.Checkbutton(
             self.labelframe,
             text="MUTE",
-            command=partial(self.labelframe.toggle_mute, "mute"),
+            command=partial(self.labelframe.pause_updates, self.labelframe.toggle_mute),
             style=f"{'Toggle.TButton' if _configuration.themes_enabled else f'{self.identifier}Mute{self.index}.TButton'}",
             variable=self.labelframe.mute,
         )
         self.button_mute.grid(column=0, row=2, columnspan=2)
 
     def add_conf_button(self):
         self.button_conf = ttk.Checkbutton(
@@ -279,15 +285,15 @@
         )
         self.button_conf.grid(column=0, row=3, columnspan=2)
 
     def add_on_button(self):
         self.button_on = ttk.Checkbutton(
             self.labelframe,
             text="ON",
-            command=self.labelframe.set_on,
+            command=partial(self.labelframe.pause_updates, self.labelframe.set_on),
             style=f"{'Toggle.TButton' if _configuration.themes_enabled else f'{self.identifier}On{self.index}.TButton'}",
             variable=self.labelframe.on,
         )
         self.button_on.grid(column=0, row=2, columnspan=2)
 
     def teardown(self):
         self.labelframe.grid_remove()
@@ -482,15 +488,17 @@
         aud_scale.grid(column=1, row=0)
 
     def create_a_buttons(self):
         self.configframe.a_buttons = [
             ttk.Checkbutton(
                 self.configframe,
                 text=param,
-                command=partial(self.configframe.toggle_a, param),
+                command=partial(
+                    self.configframe.pause_updates, self.configframe.toggle_a, param
+                ),
                 style=f"{'Toggle.TButton' if _configuration.themes_enabled else f'{param}.TButton'}",
                 variable=self.configframe.phys_out_params_vars[
                     self.configframe.phys_out_params.index(param)
                 ],
             )
             for param in self.configframe.phys_out_params
         ]
@@ -503,15 +511,17 @@
         ]
 
     def create_b_buttons(self):
         self.configframe.b_buttons = [
             ttk.Checkbutton(
                 self.configframe,
                 text=param,
-                command=partial(self.configframe.toggle_b, param),
+                command=partial(
+                    self.configframe.pause_updates, self.configframe.toggle_b, param
+                ),
                 style=f"{'Toggle.TButton' if _configuration.themes_enabled else f'{param}.TButton'}",
                 variable=self.configframe.virt_out_params_vars[
                     self.configframe.virt_out_params.index(param)
                 ],
             )
             for param in self.configframe.virt_out_params
         ]
@@ -524,15 +534,17 @@
         ]
 
     def create_param_buttons(self):
         param_buttons = [
             ttk.Checkbutton(
                 self.configframe,
                 text=param,
-                command=partial(self.configframe.toggle_p, param),
+                command=partial(
+                    self.configframe.pause_updates, self.configframe.toggle_p, param
+                ),
                 style=f"{'Toggle.TButton' if _configuration.themes_enabled else f'{param}.TButton'}",
                 variable=self.configframe.param_vars[i],
             )
             for i, param in enumerate(self.configframe.params)
         ]
         [
             button.grid(
@@ -574,26 +586,34 @@
         self.configframe.busmode_button = ttk.Button(
             self.configframe, textvariable=self.configframe.bus_mode_label_text
         )
         self.configframe.busmode_button.grid(
             column=0, row=0, columnspan=2, sticky=(tk.W)
         )
         self.configframe.busmode_button.bind(
-            "<Button-1>", self.configframe.rotate_bus_modes_right
+            "<Button-1>",
+            partial(
+                self.configframe.pause_updates, self.configframe.rotate_bus_modes_right
+            ),
         )
         self.configframe.busmode_button.bind(
-            "<Button-3>", self.configframe.rotate_bus_modes_left
+            "<Button-3>",
+            partial(
+                self.configframe.pause_updates, self.configframe.rotate_bus_modes_left
+            ),
         )
 
     def create_param_buttons(self):
         param_buttons = [
             ttk.Checkbutton(
                 self.configframe,
                 text=param,
-                command=partial(self.configframe.toggle_p, param),
+                command=partial(
+                    self.configframe.pause_updates, self.configframe.toggle_p, param
+                ),
                 style=f"{'Toggle.TButton' if _configuration.themes_enabled else f'{param}.TButton'}",
                 variable=self.configframe.param_vars[i],
             )
             for i, param in enumerate(self.configframe.params)
         ]
         [
             button.grid(
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/channels.py` & `voicemeeter_compact-1.9.0/vmcompact/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,33 +84,43 @@
         self.after(1, self.add_events)
 
     def add_events(self):
         self.parent.target.event.add("pdirty")
         self.parent.target.event.add("ldirty")
         self.after(500, self.resume_updates)
 
+    def pause_updates(self, func, *args):
+        """function wrapper, adds a 50ms delay on updates"""
+        _base_values.run_update = False
+
+        func(*args)
+
+        self.after(50, self.resume_updates)
+
     def resume_updates(self):
         _base_values.run_update = True
 
     def _on_mousewheel(self, event):
-        _base_values.run_update = False
         self.gain.set(
-            self.gain.get()
-            + (
-                _configuration.mwscroll_step
-                if event.delta > 0
-                else -_configuration.mwscroll_step
+            round(
+                self.gain.get()
+                + (
+                    _configuration.mwscroll_step
+                    if event.delta > 0
+                    else -_configuration.mwscroll_step
+                ),
+                1,
             )
         )
         if self.gain.get() > 12:
             self.gain.set(12)
         elif self.gain.get() < -60:
             self.gain.set(-60)
         self.setter("gain", self.gain.get())
-        self.after(1, self.resume_updates)
+        self.gainlabel.set(round(self.gain.get(), 1))
 
     def open_config(self):
         if self.conf.get():
             self.configbuilder.create_configframe(self.identifier, self.index, self.id)
         else:
             self.parent.parent.config_frame.teardown()
         if not _configuration.themes_enabled:
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/config.py` & `voicemeeter_compact-1.9.0/vmcompact/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,22 @@
         self.after(1, self.add_events)
 
     def add_events(self):
         self.parent.target.event.add("pdirty")
         self.parent.target.event.add("ldirty")
         self.after(350, self.resume_updates)
 
+    def pause_updates(self, func, *args):
+        """function wrapper, adds a 50ms delay on updates"""
+        _base_values.run_update = False
+
+        func(*args)
+
+        self.after(50, self.resume_updates)
+
     def resume_updates(self):
         _base_values.run_update = True
 
     def scale_enter(self, param, *args):
         val = self.slider_vars[self.slider_params.index(param)].get()
         self.parent.nav_frame.info_text.set(round(val, 1))
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/configurations.py` & `voicemeeter_compact-1.9.0/vmcompact/configurations.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/vmcompact/data.py` & `voicemeeter_compact-1.9.0/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/vmcompact/gainlayer.py` & `voicemeeter_compact-1.9.0/vmcompact/gainlayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,22 @@
         self.after(1, self.add_events)
 
     def add_events(self):
         self.parent.target.event.add("pdirty")
         self.parent.target.event.add("ldirty")
         self.after(500, self.resume_updates)
 
+    def pause_updates(self, func, *args):
+        """function wrapper, adds a 50ms delay on updates"""
+        _base_values.run_update = False
+
+        func(*args)
+
+        self.after(50, self.resume_updates)
+
     def resume_updates(self):
         _base_values.run_update = True
 
     def _on_mousewheel(self, event):
         _base_values.run_update = False
         self.gain.set(
             self.gain.get()
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/img/cat.ico` & `voicemeeter_compact-1.9.0/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/vmcompact/menu.py` & `voicemeeter_compact-1.9.0/vmcompact/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,18 @@
     def enable_vban_menus(self):
         [
             self.menu_vban.entryconfig(j, state="normal")
             for j, _ in enumerate(self.menu_vban.winfo_children())
         ]
 
     def action_invoke_voicemeeter(self, cmd):
-        getattr(self.target.command, cmd)()
+        if fn := getattr(self.target.command, cmd):
+            fn()
+        if cmd == "shutdown":
+            self.parent.destroy()
 
     def action_set_voicemeeter(self, cmd, val=True):
         if cmd == "lock":
             self._lock.set(val)
             self._unlock.set(not self._lock.get())
         setattr(self.target.command, cmd, val)
 
@@ -394,15 +397,15 @@
         self.parent._destroy_top_level_frames()
         _base_values.vban_connected = False
         # logout of vban interface
         self.vmr.init_thread()
         self.vban.logout()
         # build new app frames according to a kind
         kind = kind_get(self.vmr.type)
-        self.parent.build_app(kind, None)
+        self.parent.build_app(kind)
         target_menu = getattr(self, f"menu_vban_{i+1}")
         target_menu.entryconfig(0, state="normal")
         target_menu.entryconfig(1, state="disabled")
         self.menu_layout.entryconfig(
             0, state=f"{'normal' if kind.name == 'potato' else 'disabled'}"
         )
         # ensure the configs are reloaded into memory
```

### Comparing `voicemeeter_compact-1.8.4/vmcompact/navigation.py` & `voicemeeter_compact-1.9.0/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/vmcompact/subject.py` & `voicemeeter_compact-1.9.0/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.4/PKG-INFO` & `voicemeeter_compact-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.8.4
+Version: 1.9.0
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sv-ttk (>=2.5.1,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: vban-cmd (>=2.0.0,<3.0.0)
-Requires-Dist: voicemeeter-api (>=2.0.2,<3.0.0)
+Requires-Dist: vban-cmd (>=2.2.0,<3.0.0)
+Requires-Dist: voicemeeter-api (>=2.1.2,<3.0.0)
 Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-compact
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![OS: Windows](https://img.shields.io/badge/os-windows-red)
@@ -50,36 +50,36 @@
 
 ```python
 import voicemeeterlib
 import vmcompact
 
 
 def main():
-    # pass the kind_id and the vm object to the app
-    with voicemeeterlib.api(kind_id) as vm:
-        app = vmcompact.connect(kind_id, vm)
+    # choose the kind of Voicemeeter (Local connection)
+    KIND_ID = "banana"
+
+    # pass the KIND_ID and the vm object to the app
+    with voicemeeterlib.api(KIND_ID) as vm:
+        app = vmcompact.connect(KIND_ID, vm)
         app.mainloop()
 
 
 if __name__ == "__main__":
-    # choose the kind of Voicemeeter (Local connection)
-    kind_id = "banana"
-
     main()
 ```
 
 It's important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.
 
 ![Image of unlabelled app](./doc_imgs/nolabels.png)
 
 If the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).
 
-### kind_id
+### KIND_ID
 
-Set the kind of Voicemeeter, kind_id may be:
+Set the kind of Voicemeeter, KIND_ID may be:
 
 -   `basic`
 -   `banana`
 -   `potato`
 
 ## TOML Files
```

