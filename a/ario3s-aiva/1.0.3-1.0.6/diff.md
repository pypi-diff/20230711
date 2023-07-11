# Comparing `tmp/ario3s_aiva-1.0.3.tar.gz` & `tmp/ario3s_aiva-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ario3s_aiva-1.0.3.tar", max compression
+gzip compressed data, was "ario3s_aiva-1.0.6.tar", max compression
```

## Comparing `ario3s_aiva-1.0.3.tar` & `ario3s_aiva-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      632 2023-07-10 20:49:21.861730 ario3s_aiva-1.0.3/README.md
--rw-r--r--   0        0        0       22 2023-07-10 21:03:52.765495 ario3s_aiva-1.0.3/ario3s_aiva/__init__.py
--rw-r--r--   0        0        0       40 2023-01-14 09:52:31.824096 ario3s_aiva-1.0.3/ario3s_aiva/__main__.py
--rw-r--r--   0        0        0       37 2023-07-10 19:31:07.815125 ario3s_aiva-1.0.3/ario3s_aiva/commands/__init__.py
--rw-r--r--   0        0        0     1656 2023-07-10 20:39:01.251714 ario3s_aiva-1.0.3/ario3s_aiva/commands/change_server.py
--rw-r--r--   0        0        0      891 2023-07-10 19:29:33.646192 ario3s_aiva-1.0.3/ario3s_aiva/commands/connect.py
--rw-r--r--   0        0        0      555 2023-07-10 19:28:04.957168 ario3s_aiva-1.0.3/ario3s_aiva/commands/disconnect.py
--rw-r--r--   0        0        0      344 2023-07-10 19:28:13.973280 ario3s_aiva-1.0.3/ario3s_aiva/commands/list_servers.py
--rw-r--r--   0        0        0      660 2023-07-10 19:28:19.841351 ario3s_aiva-1.0.3/ario3s_aiva/commands/restart.py
--rw-r--r--   0        0        0      979 2023-07-10 19:28:26.745434 ario3s_aiva-1.0.3/ario3s_aiva/commands/status.py
--rw-r--r--   0        0        0      132 2023-07-10 18:58:36.624633 ario3s_aiva-1.0.3/ario3s_aiva/config.py
--rw-r--r--   0        0        0      668 2023-07-10 19:39:09.354250 ario3s_aiva-1.0.3/ario3s_aiva/main.py
--rw-r--r--   0        0        0        0 2023-07-10 18:53:18.528666 ario3s_aiva-1.0.3/ario3s_aiva/utils/__init__.py
--rw-r--r--   0        0        0     2617 2023-07-10 19:22:02.230868 ario3s_aiva-1.0.3/ario3s_aiva/utils/config_file.py
--rw-r--r--   0        0        0      696 2023-07-10 19:21:14.485689 ario3s_aiva-1.0.3/ario3s_aiva/utils/os_commands.py
--rw-r--r--   0        0        0     2245 2023-07-10 19:30:46.574926 ario3s_aiva-1.0.3/ario3s_aiva/utils/run_command.py
--rw-r--r--   0        0        0      693 2023-07-10 21:03:46.965044 ario3s_aiva-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 ario3s_aiva-1.0.3/setup.py
--rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 ario3s_aiva-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      632 2023-07-10 20:49:21.861730 ario3s_aiva-1.0.6/README.md
+-rw-r--r--   0        0        0       54 2023-07-11 10:23:05.298923 ario3s_aiva-1.0.6/ario3s_aiva/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-14 09:52:31.824096 ario3s_aiva-1.0.6/ario3s_aiva/__main__.py
+-rw-r--r--   0        0        0       37 2023-07-10 19:31:07.815125 ario3s_aiva-1.0.6/ario3s_aiva/commands/__init__.py
+-rw-r--r--   0        0        0     1656 2023-07-10 20:39:01.251714 ario3s_aiva-1.0.6/ario3s_aiva/commands/change_server.py
+-rw-r--r--   0        0        0      891 2023-07-10 19:29:33.646192 ario3s_aiva-1.0.6/ario3s_aiva/commands/connect.py
+-rw-r--r--   0        0        0      555 2023-07-10 19:28:04.957168 ario3s_aiva-1.0.6/ario3s_aiva/commands/disconnect.py
+-rw-r--r--   0        0        0      344 2023-07-10 19:28:13.973280 ario3s_aiva-1.0.6/ario3s_aiva/commands/list_servers.py
+-rw-r--r--   0        0        0      660 2023-07-10 19:28:19.841351 ario3s_aiva-1.0.6/ario3s_aiva/commands/restart.py
+-rw-r--r--   0        0        0      979 2023-07-10 19:28:26.745434 ario3s_aiva-1.0.6/ario3s_aiva/commands/status.py
+-rw-r--r--   0        0        0      132 2023-07-10 18:58:36.624633 ario3s_aiva-1.0.6/ario3s_aiva/config.py
+-rw-r--r--   0        0        0      668 2023-07-10 19:39:09.354250 ario3s_aiva-1.0.6/ario3s_aiva/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:53:18.528666 ario3s_aiva-1.0.6/ario3s_aiva/utils/__init__.py
+-rw-r--r--   0        0        0     2617 2023-07-10 19:22:02.230868 ario3s_aiva-1.0.6/ario3s_aiva/utils/config_file.py
+-rw-r--r--   0        0        0      696 2023-07-10 19:21:14.485689 ario3s_aiva-1.0.6/ario3s_aiva/utils/os_commands.py
+-rw-r--r--   0        0        0     2245 2023-07-10 19:30:46.574926 ario3s_aiva-1.0.6/ario3s_aiva/utils/run_command.py
+-rw-r--r--   0        0        0       22 2023-07-10 21:12:01.077253 ario3s_aiva-1.0.6/ario3s_aiva/version.py
+-rw-r--r--   0        0        0      739 2023-07-11 10:24:33.187553 ario3s_aiva-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 ario3s_aiva-1.0.6/setup.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 ario3s_aiva-1.0.6/PKG-INFO
```

### Comparing `ario3s_aiva-1.0.3/README.md` & `ario3s_aiva-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/commands/change_server.py` & `ario3s_aiva-1.0.6/ario3s_aiva/commands/change_server.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/commands/connect.py` & `ario3s_aiva-1.0.6/ario3s_aiva/commands/connect.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/commands/disconnect.py` & `ario3s_aiva-1.0.6/ario3s_aiva/commands/disconnect.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/commands/restart.py` & `ario3s_aiva-1.0.6/ario3s_aiva/commands/restart.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/commands/status.py` & `ario3s_aiva-1.0.6/ario3s_aiva/commands/status.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/main.py` & `ario3s_aiva-1.0.6/ario3s_aiva/main.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/utils/config_file.py` & `ario3s_aiva-1.0.6/ario3s_aiva/utils/config_file.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/utils/os_commands.py` & `ario3s_aiva-1.0.6/ario3s_aiva/utils/os_commands.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/ario3s_aiva/utils/run_command.py` & `ario3s_aiva-1.0.6/ario3s_aiva/utils/run_command.py`

 * *Files identical despite different names*

### Comparing `ario3s_aiva-1.0.3/pyproject.toml` & `ario3s_aiva-1.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ario3s-aiva"
-version = "1.0.3"
 description = "Manage dynamic ssh tunnel on localhost"
 authors = ["ario <cybera.3s@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ario3s_aiva"}]
+version = "0"
 
+[tool.poetry.urls]
+repository = "https://github.com/cybera3s/ario3s_aiva_cli"
 
-[project.urls]
-"Homepage" = "https://github.com/cybera3s/ario3s_aiva_cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tomli = "^2.0.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 toml = "^0.10.2"
 
@@ -25,8 +25,11 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aiva = "ario3s_aiva.main:app" 
 
 [tool.black]
-line-length = 79
+line-length = 79
+
+[tool.poetry-version-plugin]
+source = "init"
```

### Comparing `ario3s_aiva-1.0.3/setup.py` & `ario3s_aiva-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['toml>=0.10.2,<0.11.0', 'tomli>=2.0.1,<3.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['aiva = ario3s_aiva.main:app']}
 
 setup_kwargs = {
     'name': 'ario3s-aiva',
-    'version': '1.0.3',
+    'version': '1.0.6',
     'description': 'Manage dynamic ssh tunnel on localhost',
     'long_description': '# aiva cli tool\n\n<p>A tool to create SOCKS5 proxy on localhost</p>\n\n\n## Configuration\n<p>Default config file path is /home/USERNAME/.aiva.toml\n\n<b>Config file Format</b>\n```\n[default]\nusername = "<DEFAULT USERNAME>"\nlocal_port = <DEFAULT BIND PORT>\nserver_label = "<DEFAULT LABEL>"\n\n[server_<label>]\nip = <server-ip>\nport = <server-port>\n\n[server_<label>]\n...\n\n```\n</p>\n\n## Usage\n\nConnects to server using ssh\n```\naiva connect  \n```\n\nDisconnects from server\n```\naiva disconnect  \n```\n\nGet connection status\n```\naiva status [-d] \n```\n\nList available servers\n```\naiva list_servers\n```\n\nChange default server\n```\naiva change-server\n```',
     'author': 'ario',
     'author_email': 'cybera.3s@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ario3s_aiva-1.0.3/PKG-INFO` & `ario3s_aiva-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ario3s-aiva
-Version: 1.0.3
+Version: 1.0.6
 Summary: Manage dynamic ssh tunnel on localhost
 Author: ario
 Author-email: cybera.3s@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: repository, https://github.com/cybera3s/ario3s_aiva_cli
 Description-Content-Type: text/markdown
 
 # aiva cli tool
 
 <p>A tool to create SOCKS5 proxy on localhost</p>
```

