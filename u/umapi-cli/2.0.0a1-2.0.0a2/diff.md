# Comparing `tmp/umapi_cli-2.0.0a1.tar.gz` & `tmp/umapi_cli-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umapi_cli-2.0.0a1.tar", max compression
+gzip compressed data, was "umapi_cli-2.0.0a2.tar", max compression
```

## Comparing `umapi_cli-2.0.0a1.tar` & `umapi_cli-2.0.0a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11335 2023-06-21 15:28:39.518313 umapi_cli-2.0.0a1/LICENSE
--rw-r--r--   0        0        0      610 2023-06-28 05:25:03.616226 umapi_cli-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      603 2023-06-21 16:29:58.311507 umapi_cli-2.0.0a1/umapi_cli/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-29 00:01:19.698699 umapi_cli-2.0.0a1/umapi_cli/action_queue.py
--rw-r--r--   0        0        0    16523 2023-06-28 23:29:41.029748 umapi_cli-2.0.0a1/umapi_cli/cli.py
--rw-r--r--   0        0        0     1318 2023-06-21 16:29:28.366519 umapi_cli-2.0.0a1/umapi_cli/client.py
--rw-r--r--   0        0        0     1253 2023-06-21 16:29:35.143777 umapi_cli-2.0.0a1/umapi_cli/config.py
--rw-r--r--   0        0        0     5834 2023-06-28 23:07:34.517123 umapi_cli-2.0.0a1/umapi_cli/formatter.py
--rw-r--r--   0        0        0     1298 2023-06-21 16:29:14.623535 umapi_cli-2.0.0a1/umapi_cli/log.py
--rw-r--r--   0        0        0      628 2023-06-21 16:29:08.563818 umapi_cli-2.0.0a1/umapi_cli/version.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 umapi_cli-2.0.0a1/setup.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 umapi_cli-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-06-21 15:28:39.518313 umapi_cli-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0    24216 2023-06-29 22:55:29.426631 umapi_cli-2.0.0a2/README.md
+-rw-r--r--   0        0        0      705 2023-06-30 05:28:16.965493 umapi_cli-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-21 16:29:58.311507 umapi_cli-2.0.0a2/umapi_cli/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-29 00:01:19.698699 umapi_cli-2.0.0a2/umapi_cli/action_queue.py
+-rw-r--r--   0        0        0    16607 2023-06-30 04:10:34.672428 umapi_cli-2.0.0a2/umapi_cli/cli.py
+-rw-r--r--   0        0        0     1318 2023-06-21 16:29:28.366519 umapi_cli-2.0.0a2/umapi_cli/client.py
+-rw-r--r--   0        0        0     1253 2023-06-21 16:29:35.143777 umapi_cli-2.0.0a2/umapi_cli/config.py
+-rw-r--r--   0        0        0     5834 2023-06-28 23:07:34.517123 umapi_cli-2.0.0a2/umapi_cli/formatter.py
+-rw-r--r--   0        0        0     1298 2023-06-21 16:29:14.623535 umapi_cli-2.0.0a2/umapi_cli/log.py
+-rw-r--r--   0        0        0      628 2023-06-30 04:26:09.885809 umapi_cli-2.0.0a2/umapi_cli/version.py
+-rw-r--r--   0        0        0    24970 1970-01-01 00:00:00.000000 umapi_cli-2.0.0a2/PKG-INFO
```

### Comparing `umapi_cli-2.0.0a1/LICENSE` & `umapi_cli-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/pyproject.toml` & `umapi_cli-2.0.0a2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [tool.poetry]
 name = "umapi-cli"
-version = "2.0.0a1"
+version = "2.0.0a2"
 description = "User Management API CLI Tool"
 authors = ["Andrew Dorton <adorton@adobe.com>"]
+license = "Apache 2.0"
+readme = "README.md"
+repository = "https://github.com/adobe/umapi-cli/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.0"
 umapi-client = "^3.0"
 python-dotenv = "^1.0.0"
 schema = "^0.7.5"
```

### Comparing `umapi_cli-2.0.0a1/umapi_cli/__init__.py` & `umapi_cli-2.0.0a2/umapi_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/umapi_cli/action_queue.py` & `umapi_cli-2.0.0a2/umapi_cli/action_queue.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/umapi_cli/cli.py` & `umapi_cli-2.0.0a2/umapi_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 @click.version_option(app_version, '--version', message='%(prog)s %(version)s')
 @click.pass_context
 def app(ctx, env_file, test_mode, v):
     log.init(v)
     if env_file is not None:
         dotenv.load_dotenv(env_file)
     else:
-        dotenv.load_dotenv()
+        env_file = dotenv.find_dotenv(usecwd=True)
+        if env_file:
+            dotenv.load_dotenv(env_file)
     ctx.ensure_object(dict)
     conf = config.get_options()
     ctx.obj['conn'] = client.create_conn(conf, test_mode)
 
 
 @app.command()
 @click.help_option('-h', '--help')
```

### Comparing `umapi_cli-2.0.0a1/umapi_cli/client.py` & `umapi_cli-2.0.0a2/umapi_cli/client.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/umapi_cli/config.py` & `umapi_cli-2.0.0a2/umapi_cli/config.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/umapi_cli/formatter.py` & `umapi_cli-2.0.0a2/umapi_cli/formatter.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/umapi_cli/log.py` & `umapi_cli-2.0.0a2/umapi_cli/log.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a1/umapi_cli/version.py` & `umapi_cli-2.0.0a2/umapi_cli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-__version__ = "2.0.0a1"
+__version__ = "2.0.0a2"
```

