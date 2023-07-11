# Comparing `tmp/asterisk-plus-agent-3.0.1.tar.gz` & `tmp/asterisk-plus-agent-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asterisk-plus-agent-3.0.1.tar", last modified: Mon Jul 10 09:02:51 2023, max compression
+gzip compressed data, was "asterisk-plus-agent-3.0.2.tar", last modified: Tue Jul 11 11:52:14 2023, max compression
```

## Comparing `asterisk-plus-agent-3.0.1.tar` & `asterisk-plus-agent-3.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:02:51.406228 asterisk-plus-agent-3.0.1/
--rw-r--r--   0 root         (0) root         (0)      973 2023-07-10 09:02:51.402228 asterisk-plus-agent-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-28 18:31:50.000000 asterisk-plus-agent-3.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:02:51.402228 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      973 2023-07-10 09:02:51.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-10 09:02:51.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:02:51.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 09:02:51.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:01:15.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 09:02:51.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-10 09:02:51.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    23266 2023-07-10 08:58:30.000000 asterisk-plus-agent-3.0.1/asterisk_plus_agent.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:02:51.406228 asterisk-plus-agent-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-28 18:27:32.000000 asterisk-plus-agent-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:52:14.795134 asterisk-plus-agent-3.0.2/
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-11 11:52:14.791134 asterisk-plus-agent-3.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-28 18:31:50.000000 asterisk-plus-agent-3.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:52:14.791134 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-11 11:52:14.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-11 11:52:14.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 11:52:14.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-11 11:52:14.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:01:15.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-11 11:52:14.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-11 11:52:14.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    23327 2023-07-11 11:49:26.000000 asterisk-plus-agent-3.0.2/asterisk_plus_agent.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 11:52:14.795134 asterisk-plus-agent-3.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-28 18:27:32.000000 asterisk-plus-agent-3.0.2/setup.py
```

### Comparing `asterisk-plus-agent-3.0.1/PKG-INFO` & `asterisk-plus-agent-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asterisk-plus-agent
-Version: 3.0.1
+Version: 3.0.2
 Summary: Asterisk Plus PBX Agent
 Home-page: https://odoopbx.com
 Author: Odooist
 Author-email: odooist@gmail.com
 License: Odoo Enterprise Edition License v1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `asterisk-plus-agent-3.0.1/asterisk_plus_agent.egg-info/PKG-INFO` & `asterisk-plus-agent-3.0.2/asterisk_plus_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asterisk-plus-agent
-Version: 3.0.1
+Version: 3.0.2
 Summary: Asterisk Plus PBX Agent
 Home-page: https://odoopbx.com
 Author: Odooist
 Author-email: odooist@gmail.com
 License: Odoo Enterprise Edition License v1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `asterisk-plus-agent-3.0.1/asterisk_plus_agent.py` & `asterisk-plus-agent-3.0.2/asterisk_plus_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from aio_odoorpc import AsyncOdooRPC
 import aiorun
 import httpx
 from panoramisk import Manager, Message
 import wave
 import lameenc
 
-__version__ = '3.0.1'
+__version__ = '3.0.2'
 
 
 if os.environ.get('SENTRY_DSN'):
     import sentry_sdk
     sentry_sdk.init(
         dsn=os.environ['SENTRY_DSN'],
         traces_sample_rate=1.0)    
@@ -65,48 +65,51 @@
     config = {}
 
 
 ############### SYSTEM #################################
 
     def __init__(self, config_path):
         self.config_path = config_path
+        self.config = {}
 
     def get_source(self):
         script_path = inspect.getfile(inspect.currentframe())
         source_code = open(script_path, 'rb').read()
         data = base64.b64encode(source_code).decode()
         return data
 
     async def load_config(self):
+        local_config = {}
+        agent_config = {}
         if not os.path.exists(self.config_path):
             raise Exception('Config file %s does not exist!' % self.config_path)
         with open(self.config_path) as f:
-            self.config = yaml.load(f, Loader=yaml.FullLoader)
-            if not self.config:
+            local_config = yaml.load(f, Loader=yaml.FullLoader)
+            if not local_config:
                 raise Exception('Config file %s is empty or broken!' % self.config_path)
         r = None
         try:
             # Next load config from the billing            
             async with httpx.AsyncClient() as client:                
                 r = await client.post(
-                    urljoin(self.config['api_url'], 'app/asterisk_plus/config'),
+                    urljoin(local_config['api_url'], 'app/asterisk_plus/config'),
                     json={
                         'source_code': self.get_source(),
                     },
                     headers={
-                        'x-api-key': self.config['api_key'],
-                        'x-instance-uid': self.config['instance_uid']})
+                        'x-api-key': local_config['api_key'],
+                        'x-instance-uid': local_config['instance_uid']})
                 r.raise_for_status()
                 agent_config = r.json()
                 # Check versions
                 major_version = float('.'.join(__version__.split('.')[:2]))
                 if float(agent_config['asterisk_plus_version']) != major_version:
                     logger.warning('Asterisk Plus module version is %s, but your Agent version is %s, upgrade the Agent!',
                         agent_config['asterisk_plus_version'], __version__)
-                # Finally overwrite with local values                
+                self.config.update(local_config)
                 self.config.update(agent_config)
                 logger.debug(json.dumps(self.config, indent=2))
                 logger.info('Config loaded.')
         except Exception as e:
             logger.error('Init config: %s', r and r.text or e)
             await asyncio.sleep(10*365*24*60*60)
```

### Comparing `asterisk-plus-agent-3.0.1/setup.py` & `asterisk-plus-agent-3.0.2/setup.py`

 * *Files identical despite different names*

