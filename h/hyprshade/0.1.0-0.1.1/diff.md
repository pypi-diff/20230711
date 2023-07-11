# Comparing `tmp/hyprshade-0.1.0.tar.gz` & `tmp/hyprshade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.1.0.tar", max compression
+gzip compressed data, was "hyprshade-0.1.1.tar", max compression
```

## Comparing `hyprshade-0.1.0.tar` & `hyprshade-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.1.0/LICENSE
--rw-r--r--   0        0        0       44 2023-07-05 23:37:20.434170 hyprshade-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-06 21:56:49.771001 hyprshade-0.1.0/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.1.0/hyprshade/__main__.py
--rw-r--r--   0        0        0     2491 2023-07-10 07:17:12.226451 hyprshade-0.1.0/hyprshade/cli.py
--rw-r--r--   0        0        0     3452 2023-07-10 00:00:56.619373 hyprshade-0.1.0/hyprshade/config.py
--rw-r--r--   0        0        0      884 2023-07-07 02:02:57.355772 hyprshade-0.1.0/hyprshade/helpers.py
--rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.1.0/hyprshade/utils.py
--rw-r--r--   0        0        0     1002 2023-07-10 07:49:59.648421 hyprshade-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 hyprshade-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.1.1/LICENSE
+-rw-r--r--   0        0        0       44 2023-07-05 23:37:20.434170 hyprshade-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 23:35:03.452541 hyprshade-0.1.1/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.1.1/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2577 2023-07-11 02:45:55.459709 hyprshade-0.1.1/hyprshade/cli.py
+-rw-r--r--   0        0        0     3553 2023-07-11 02:52:15.538679 hyprshade-0.1.1/hyprshade/config.py
+-rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.1.1/hyprshade/helpers.py
+-rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.1.1/hyprshade/utils.py
+-rw-r--r--   0        0        0     1002 2023-07-11 02:51:45.314681 hyprshade-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 hyprshade-0.1.1/PKG-INFO
```

### Comparing `hyprshade-0.1.0/LICENSE` & `hyprshade-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.0/hyprshade/cli.py` & `hyprshade-0.1.1/hyprshade/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,79 +7,79 @@
 import typer
 
 from hyprshade.helpers import get_shader_path, get_shaders_dir
 from hyprshade.utils import systemd_user_config_home
 
 EMPTY_STR: Final = "[[EMPTY]]"
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True)
 
 
 @app.command()
 def ls() -> int:
     """List available screen shaders"""
 
     shaders_dir = get_shaders_dir()
     for shader in os.listdir(shaders_dir):
         shader = path.splitext(shader)[0]
         print(shader)
     return 0
 
 
 @app.command()
-def on(shader: str) -> int:
+def on(shader_name_or_path: str) -> int:
     """Turn on screen shader"""
 
-    shader_path = get_shader_path(shader)
+    shader_path = get_shader_path(shader_name_or_path)
     code = os.system(f"hyprctl keyword decoration:screen_shader '{shader_path}'")
     return code
 
 
 @app.command()
 def off() -> int:
     """Turn off screen shader"""
 
     code = os.system(f"hyprctl keyword decoration:screen_shader '{EMPTY_STR}'")
     return code
 
 
 @app.command()
-def toggle(shader: str) -> int:
+def toggle(shader_name_or_path: str) -> int:
     """Toggle screen shader"""
 
     import json
     from json import JSONDecodeError
 
     current_shader: str | None = None
     try:
         o = json.load(os.popen("hyprctl -j getoption decoration:screen_shader"))
         current_shader = str(o["str"]).strip()
     except JSONDecodeError:
         print("Failed to get current screen shader", file=sys.stderr)
         return 1
 
     if path.isfile(current_shader) and path.samefile(
-        get_shader_path(shader), current_shader
+        get_shader_path(shader_name_or_path), current_shader
     ):
         off()
         return 0
 
-    return on(shader)
+    return on(shader_name_or_path)
 
 
 @app.command()
 def auto() -> int:
     from hyprshade.config import Config
 
     t = datetime.now().time()
     schedule = Config().to_schedule()
-    shade = schedule.contained(t)
+    shade = schedule.find_shade(t)
+
     if shade is not None:
         return on(shade)
-
     return off()
 
 
 @app.command()
 def install() -> int:
     from hyprshade.config import Config
```

### Comparing `hyprshade-0.1.0/hyprshade/config.py` & `hyprshade-0.1.1/hyprshade/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,39 +53,40 @@
             f'ScheduleEntry("{self.name}", start_time={self.start_time}, '
             f"end_time={self.end_time})"
         )
 
 
 class Schedule:
     entries: list[ScheduleEntry]
-    default_shade: str | None
+    default_shade_name: str | None
 
     def __init__(self, config_dict: ConfigDict):
         default_shade, other_shades = partition_shades(config_dict["shades"])
         sorted_shades = sorted(other_shades, key=lambda s: s["start_time"])
         self.entries = list(map(ScheduleEntry, sorted_shades))
-        self.default_shade = default_shade and default_shade["name"]
+        self.default_shade_name = default_shade and default_shade["name"]
 
-    def contained(self, t: time) -> str | None:
-        for entry, next_entry in self._pairwise_entries():
-            start_time = entry.start_time
-            end_time = entry.end_time or next_entry.start_time
+    def find_shade(self, t: time) -> str | None:
+        for entry_name, start_time, end_time in self._resolved_entries():
             if is_time_between(t, start_time, end_time):
-                return entry.name
+                return entry_name
 
-        return self.default_shade
+        return self.default_shade_name
 
     def on_calendar_entries(self) -> Iterable[time]:
         for entry in self.entries:
             yield entry.start_time
             if entry.end_time is not None:
                 yield entry.end_time
 
-    def _pairwise_entries(self):
-        return pairwise(chain(self.entries, [self.entries[0]]))
+    def _resolved_entries(self):
+        for entry, next_entry in pairwise(chain(self.entries, [self.entries[0]])):
+            start_time = entry.start_time
+            end_time = entry.end_time or next_entry.start_time
+            yield entry.name, start_time, end_time
 
 
 class Config:
     """Parses config.toml into a dict"""
 
     _config_dict: ConfigDict
```

### Comparing `hyprshade-0.1.0/hyprshade/helpers.py` & `hyprshade-0.1.1/hyprshade/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,23 @@
     config_home = hypr_config_home()
     shaders_dir = path.join(config_home, "shaders")
     if not path.isdir(shaders_dir):
         raise FileNotFoundError(f"Shaders directory {shaders_dir} does not exist")
     return path.join(config_home, "shaders")
 
 
-def get_shader_path(shader: str) -> str:
-    shader_path = shader
+def get_shader_path(shader_name_or_path: str) -> str:
+    shader_path = shader_name_or_path
     if not path.isfile(shader_path):
         shaders_dir = get_shaders_dir()
-        shader_path = path.join(shaders_dir, glsl_ext(shader))
+        shader_path = path.join(shaders_dir, glsl_ext(shader_name_or_path))
         if not path.isfile(shader_path):
             raise FileNotFoundError(
-                f"Shader {shader} does not exist; check contents of {shaders_dir}"
+                f"Shader {shader_name_or_path} does not exist; "
+                f"check contents of {shaders_dir}"
             )
     return shader_path
 
 
 def glsl_ext(pathname: str) -> str:
     if pathname.endswith(".glsl"):
         return pathname
```

### Comparing `hyprshade-0.1.0/hyprshade/utils.py` & `hyprshade-0.1.1/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.0/pyproject.toml` & `hyprshade-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 
 [tool.poetry.dependencies]
```

