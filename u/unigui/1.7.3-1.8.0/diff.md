# Comparing `tmp/unigui-1.7.3.tar.gz` & `tmp/unigui-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.7.3.tar", last modified: Mon Jul 10 20:24:13 2023, max compression
+gzip compressed data, was "dist/unigui-1.8.0.tar", last modified: Tue Jul 11 21:52:33 2023, max compression
```

## Comparing `unigui-1.7.3.tar` & `unigui-1.8.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     9904 2023-07-10 20:13:51.000000 unigui-1.7.3/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     9136 2023-07-10 12:04:53.000000 unigui-1.7.3/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3573 2023-07-10 12:41:32.000000 unigui-1.7.3/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.7.3/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2396 2023-07-02 15:25:42.000000 unigui-1.7.3/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/css/vendor.49a52e8f.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/css/878.c6483fb6.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    45060 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/878.e76799d2.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/app.b39a06ae.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.7.3/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-10 20:23:44.000000 unigui-1.7.3/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19083 2023-07-10 20:24:13.000000 unigui-1.7.3/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-10 20:24:13.000000 unigui-1.7.3/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18778 2023-07-10 11:37:36.000000 unigui-1.7.3/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.7.3/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19083 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.7.3/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     9132 2023-07-11 20:55:41.000000 unigui-1.8.0/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3280 2023-07-11 18:46:47.000000 unigui-1.8.0/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)       99 2023-07-11 08:13:29.000000 unigui-1.8.0/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2449 2023-07-11 13:55:58.000000 unigui-1.8.0/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9608 2023-07-11 20:49:39.000000 unigui-1.8.0/unigui/user.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/css/223.f0f63b8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    44624 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/223.7924e6b0.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/app.fc1b2f39.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.0/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-11 21:47:23.000000 unigui-1.8.0/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19080 2023-07-11 21:52:33.000000 unigui-1.8.0/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-11 21:52:33.000000 unigui-1.8.0/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18775 2023-07-11 08:15:37.000000 unigui-1.8.0/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.0/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19080 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.0/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1202 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.7.3/unigui/manager.py` & `unigui-1.8.0/unigui/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-import os
 import importlib
 from .utils import *
-from . import utils
 import itertools
 from .guielements import *
 import sys
 import asyncio
 import requests
 from threading import Thread
 
-sign2method = {'=':'changed', '->':'update','?':'complete','+':'append', '-':'delete', '!':'editing', '#':'modify'}    
-
-#loop and thread is only for progress window functionality
-loop = asyncio.new_event_loop()
-def f(loop):
-    asyncio.set_event_loop(loop)
-    loop.run_forever() 
-
-t = Thread(target=f, args=(loop,))
-t.start()  
-
 class User:      
     def __init__(self):          
         self.screens = []        
         self.active_dialog = None
         self.screen_module = None                
         self.tool_buttons = []
         User.last_user = self
@@ -65,37 +52,36 @@
                         b = b.replace(bytes('8000',encoding='utf8'), bytes(str(utils.resource_port),encoding='utf8'))                
                     if utils.socket_port != 1234:
                         b = b.replace(bytes('1234',encoding='utf8'), bytes(str(utils.socket_port),encoding='utf8'))                
                     User.fixed_main = b.decode("utf-8") 
                     print(f"Fixed {file} created on ip {utils.socket_ip}, http port {utils.resource_port}, socket port {utils.socket_port}.")
                     break
 
+    def sync_send(self, obj):
+        asyncio.run_coroutine_threadsafe(self.send(obj), self.extra_loop)            
+
     def progress(self, str, *updates):
         """open or update progress window if str != null else close it  """     
         d = {'progress': str}
         if updates:
             d['update'] = None            
-            d['data'] = updates                 
-        asyncio.run_coroutine_threadsafe(self.send(d), loop)            
+            d['data'] = updates          
+        self.sync_send(d)               
 
     def load_module(self, file):
         screen_vars = {
             'icon' : None,
             'prepare' : None,
             'dispatch' : None,
             'blocks' : [],
             'header' : utils.appname,                        
             'toolbar' : [], 
             'order' : 0
-        }     
-        
-        name = file[0:-3]
-        screens_dir =  'screens'
-             
-        #if name not in modules:                    
+        }             
+        name = file[0:-3]        
         path = f'{screens_dir}/{file}'                
         spec = importlib.util.spec_from_file_location(name,path)
         module = importlib.util.module_from_spec(spec)        
         
         utils.clean_handlers()                                        
         module.user = self                               
         
@@ -107,42 +93,44 @@
         screen.handlers__ = utils.handlers__
         
         if not screen.toolbar:
             screen.toolbar = self.tool_buttons
                         
         screen.check()                         
         module.screen = screen
-
         return module
-                              
-    def load(self):   
-         
-        blocks_dir = 'blocks'        
-        screens_dir =  'screens'
-        
+
+    def clean_sys4next_user(self):
+        #remove user modules from sys for repeating loading for new users
+        if os.path.exists(blocks_dir):
+            for file in os.listdir(blocks_dir):
+                if file.endswith(".py") and file != '__init__.py':
+                    name = f'{blocks_dir}.{file[0:-3]}'
+                    if name in sys.modules:
+                        sys.modules[name].user = self
+                        del sys.modules[name]                          
+    def load(self):            
         for file in os.listdir(screens_dir):
             if file.endswith(".py") and file != '__init__.py':
                 module = self.load_module(file)                
                 self.screens.append(module)                
         
         self.screens.sort(key=lambda s: s.screen.order)
         main = self.screens[0]
         if 'prepare' in dir(main):
             main.prepare()
         self.screen_module = main
-        self.menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
+        self.update_menu()
+        self.clean_sys4next_user()                        
+
+    def update_menu(self):
+        menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
+        for s in self.screens:
+            s.screen.menu = menu
 
-        #remove user modules from sys for repeating loading for new users
-        for file in os.listdir(blocks_dir):
-            if file.endswith(".py") and file != '__init__.py':
-                name = f'{blocks_dir}.{file[0:-3]}'
-                if name in sys.modules:
-                    sys.modules[name].user = self
-                    del sys.modules[name]
-                
     @property
     def screen(self):        
         return  self.screen_module.screen 
 
     def set_screen(self,name):
         return self.process(['root', name])
 
@@ -225,36 +213,40 @@
             print(f'Unknown root command {s.name}')
         else:
             elem = self.find_element(arr)                        
             return self.process_element(elem, arr)        
         
     def process_element(self, elem, arr):        
         id = arr.pop() if len(arr) == 5 else 0
-        sign = arr[-2]
-        smeth = sign2method.get(sign)
+        smeth = arr[-2]        
         val = arr[-1]
-        if smeth:
-            handler = self.screen.handlers__.get((elem, smeth))
-            if handler:
-                result = handler(elem, val)                
-                return result
-            
-            handler = getattr(elem, smeth, False)                                
-            if handler:                
-                res = handler(elem, val)  
-                if id:                        
-                    res = Answer(res, None, id)                
-                return res
-            elif sign == '=':
-                if hasattr(elem,'value'): #exlude Buttons and others without 'value'
-                    elem.value = val                                        
-                return                
-            elif sign == '$': #update element params
-                for param in val:
-                    setattr(elem, param, val[param])                                        
-                return                
+        
+        handler = self.screen.handlers__.get((elem, smeth))
+        if handler:
+            result = handler(elem, val)                
+            return result
+        
+        handler = getattr(elem, smeth, False)                                
+        if handler:                
+            res = handler(elem, val)  
+            if id:                        
+                res = Answer(res, None, id)                
+            return res
+        elif smeth == 'changed':
+            if hasattr(elem,'value'): #exlude Buttons and others without 'value'
+                elem.value = val                                        
+            return                        
+
+        return Error(f'{elem} does not contain method for {smeth} event type!')
+
+#loop and thread is for progress window and async interactions
+loop = asyncio.new_event_loop()
+def f(loop):
+    asyncio.set_event_loop(loop)
+    loop.run_forever() 
 
-        if sign != '!': #editing can omit
-            return Error(f'{elem} does not contain method for {sign} event type!')
+async_thread = Thread(target=f, args=(loop,))
+async_thread.start()  
 
+User.extra_loop = loop
```

### Comparing `unigui-1.7.3/unigui/guielements.py` & `unigui-1.8.0/unigui/guielements.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     def __init__(self, *args, **kwargs):
         self.name = args[0]
         if len(args) > 1:
             self.changed = args[1]        
         for key in kwargs.keys():            
             self.add(key, kwargs[key])
 
-def CameraButton(name, handler,**kwargs):
+def CameraButton(name, *args,**kwargs):
     kwargs['type'] = 'camera'
-    return Button(name, handler, **kwargs)
+    return Button(name, *args, **kwargs)
 
 def UploadButton(name, handler,**kwargs):
     if 'type' not in kwargs:
         kwargs['type'] = 'gallery'
     if 'width' not in kwargs:
         kwargs['width'] = 250.0              
     if 'height' not in kwargs:
```

### Comparing `unigui-1.7.3/unigui/server.py` & `unigui-1.8.0/unigui/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,54 @@
 from aiohttp import web, WSMsgType
-from . import utils
-
-import os
-from .manager import * 
+from .user import *
+from config import port, pretty_print, socket_ip, socket_port, upload_dir
+from pathlib import Path
 
 async def post_handler(request):
-
     reader = await request.multipart()
-
     field = await reader.next()   
-    
     filename = upload_path(field.filename)  
     # You cannot rely on Content-Length if transfer is chunked.
     size = 0
     with open(filename, 'wb') as f:
         while True:
             chunk = await field.read_chunk()  # 8192 bytes by default.
             if not chunk:
                 break
             size += len(chunk)
             f.write(chunk)
 
     return web.Response(text=f'{filename} sized of {size} successfully stored')
 
-from config import port, user_dir, pretty_print, socket_ip, socket_port, upload_dir
-from pathlib import Path
-
-indent = 2 if pretty_print else 0
-
 def jsonString(obj):
-    return toJson(obj, indent, pretty_print)
+    return toJson(obj, 2 if pretty_print else 0, pretty_print)
 
-async def static_serve(request):
-    #if "Upgrade" in request.headers and request.headers["Upgrade"] == 'websocket':
-    #    return await websocket_handler(request)
+async def static_serve(request):    
     file_path = request.path
     if upload_dir not in  request.path:
-        file_path = f"{utils.webpath}{file_path}"  # rebase into static dir
+        file_path = f"{webpath}{file_path}"  # rebase into static dir
     file_path  = Path(file_path)
     
     if request.path == '/':
         file_path /= 'index.html'
         
-    if not file_path.exists():
-        return web.HTTPNotFound()
-     
-    return web.FileResponse(file_path) if request.path != User.fix_file else web.Response(text = User.fixed_main) 
+    return web.HTTPNotFound() if not file_path.exists() else (web.FileResponse(file_path)     
+         if request.path != User.fix_file else web.Response(text = User.fixed_main)) 
 
 async def websocket_handler(request):
-
     ws = web.WebSocketResponse()
     await ws.prepare(request)
-    
     user = User.UserType()
+
     async def send(res):
-        await ws.send_str(jsonString(user.prepare_result(res)))
-        
+        await ws.send_str(jsonString(user.prepare_result(res)))        
     user.send = send 
     user.load()
     
-    await ws.send_str(jsonString([user.menu,user.screen])) 
+    await ws.send_str(jsonString(user.screen)) 
 
     async for msg in ws:
         if msg.type == WSMsgType.TEXT:
             if msg.data == 'close':
                 await ws.close()
             else:
                 data = json.loads(msg.data)            
@@ -71,45 +56,41 @@
                 if result:                
                     await ws.send_str(jsonString(user.prepare_result(result)))
         elif msg.type == WSMsgType.ERROR:
             print('ws connection closed with exception %s' %
                 ws.exception())
 
     print('websocket connection closed')
-
     return ws       
 
 def start(appname, user_type = User, translate_path = None, http_handlers = []):
     
-    set_utils(appname,user_dir, port, upload_dir, translate_path, socket_ip, socket_port)    
+    set_utils(appname, port, upload_dir, translate_path, socket_ip, socket_port)    
     
     if upload_dir and not os.path.exists(upload_dir):
         os.makedirs(upload_dir)
 
     User.UserType = user_type
 
-    if utils.socket_ip != 'localhost' or utils.resource_port != 8000 or utils.socket_port != 1234:
+    if socket_ip != 'localhost' or resource_port != 8000 or socket_port != 1234:
         User.create_fixed_js()     
         http_handlers.append(web.get(User.fix_file, static_serve))
     else:
         User.fix_file = None
     
     http_handlers.insert(0, web.get('/ws', websocket_handler))
         
     for h in [web.get('/', static_serve), 
-        web.static('/js', f"{utils.webpath}/js"),
-        web.static('/fonts', f"{utils.webpath}/fonts"),
-        web.static('/css', f"{utils.webpath}/css"),
-        web.static('/icons', f"{utils.webpath}/icons"),
-        web.static(f'/{upload_dir}', f"/{utils.app_user_dir}/{upload_dir}"),
+        web.static('/js', f"{webpath}/js"),
+        web.static('/fonts', f"{webpath}/fonts"),
+        web.static('/css', f"{webpath}/css"),
+        web.static('/icons', f"{webpath}/icons"),
+        web.static(f'/{upload_dir}', f"/{app_user_dir}/{upload_dir}"),
         web.post('/', post_handler)]:
 
         http_handlers.append(h)
 
     print(f'Start {appname} server on {port} port..')    
-
     app = web.Application()
-    
-    app.add_routes(http_handlers)
-    
+    app.add_routes(http_handlers)    
     web.run_app(app,  port=port)
```

### Comparing `unigui-1.7.3/unigui/utils.py` & `unigui-1.8.0/unigui/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 resource_port = None
 appname = 'Unigui'
 app_user_dir = os.getcwd()
 upload_dir = 'upload'
 socket_ip = ''
 socket_port = 1234
+blocks_dir = 'blocks'        
+screens_dir =  'screens'        
 
 libpath = os.path.dirname(os.path.realpath(__file__))
 webpath = libpath + '/web' 
 
 def toJson(obj, indent, pretty_print):
     return json.dumps(json.loads(jsonpickle.encode(obj,unpicklable=False)), 
         indent = indent, sort_keys = pretty_print)
@@ -33,15 +35,15 @@
         path = path.split('?')[0]
     if path.startswith(f'/{upload_dir}/'):             
         return f'{app_user_dir}{path}'.replace('%20',' ')     
     return f'{webpath}{path}'.replace('%20',' ') 
 
 translate_path = translate_http_path
 
-def set_utils(appname_,user_dir_,port_,upload_dir_, translate_path_, socket_ip_, socket_port_):
+def set_utils(appname_,port_,upload_dir_, translate_path_, socket_ip_, socket_port_):
     global appname, resource_port, upload_dir, translate_path, socket_ip, socket_port
     appname = appname_
     resource_port = port_
     upload_dir = upload_dir_
     socket_ip = socket_ip_
     socket_port = socket_port_
```

### Comparing `unigui-1.7.3/unigui/web/favicon.ico` & `unigui-1.8.0/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.8.0/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/css/878.c6483fb6.css` & `unigui-1.8.0/unigui/web/css/223.f0f63b8f.css`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-8c264956]{display:flex;justify-content:center}.custom-caption[data-v-8c264956]{padding:5px!important}.web-camera-container[data-v-8c264956]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-8c264956]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-8c264956]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-8c264956]{opacity:1}.web-camera-container .camera-shoot[data-v-8c264956]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-8c264956]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-8c264956]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-8c264956]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-8c264956]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-8c264956]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-8c264956]{animation:preload-8c264956 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-8c264956]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-8c264956]:nth-child(3){animation-delay:.4s}@keyframes preload-8c264956{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-8c264956]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-2f472339]{display:flex;justify-content:center}.custom-caption[data-v-2f472339]{padding:5px!important}.web-camera-container[data-v-2f472339]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-2f472339]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-2f472339]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-2f472339]{opacity:1}.web-camera-container .camera-shoot[data-v-2f472339]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-2f472339]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-2f472339]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-2f472339]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-2f472339]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-2f472339]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-2f472339]{animation:preload-2f472339 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-2f472339]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-2f472339]:nth-child(3){animation-delay:.4s}@keyframes preload-2f472339{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-2f472339]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.7.3/unigui/web/icons/favicon-96x96.png` & `unigui-1.8.0/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/icons/favicon-16x16.png` & `unigui-1.8.0/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/icons/favicon-32x32.png` & `unigui-1.8.0/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/icons/favicon-128x128.png` & `unigui-1.8.0/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.8.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.8.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/js/430.591e9a73.js` & `unigui-1.8.0/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/js/878.e76799d2.js` & `unigui-1.8.0/unigui/web/js/223.7924e6b0.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [878], {
-        6878: (e, t, a) => {
+    [223], {
+        4223: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Jt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                     class: "q-pa-lg"
@@ -146,48 +146,48 @@
             }
             let j, S = 0;
 
             function z() {
                 for (let [e, t] of Object.entries(k)) t.styleSize = null
             }
 
-            function A(e, t, a, l = "?") {
+            function A(e, t, a, l = "complete") {
                 let s = ++S,
                     i = [e.pdata.name, e.data.name, l, t, s];
                 q(i), p[s] = a
             }
 
             function Z() {
                 b = {}, k = {}
             }
 
-            function M(e, t) {
+            function D(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function D(e) {
+            function M(e) {
                 if (e.multi)
                     for (let [t, a] of e.update.entries())
                         if (a.length > 1) {
                             a.reverse();
                             let l = a.join("@"),
                                 s = k[l];
-                            M(s, e.data[t])
+                            D(s, e.data[t])
                         } else {
                             let l = b[a[0]];
                             Object.assign(l.data, e.data[t])
                         }
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
                         t = k[e]
                     } else t = b[a[0]];
-                    M(t, e.data), 1 == a.length && (0, h.delay)(O, 200, t)
+                    D(t, e.data), 1 == a.length && (0, h.delay)(O, 200, t)
                 }
             }
 
             function $(e) {
                 typeof e.answer == String ? u.showError() : p[e.id](e.answer), delete p[e.id]
             }
 
@@ -208,16 +208,16 @@
                     }))
                 }))
             }
             let K = _.debounce(E, 200);
 
             function O(e) {
                 Array.isArray(e) && (e = null), j && (j.disconnect(), j = null), g && console.log("------------------recalc design");
-                const t = Q(e),
-                    a = W(e);
+                const t = W(e),
+                    a = Q(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = k[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = b[d];
                     for (let a of r.data.childs)
@@ -235,15 +235,15 @@
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function Q(e) {
+            function W(e) {
                 const t = u.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
@@ -301,15 +301,15 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function W(e) {
+            function Q(e) {
                 e = null;
                 const t = e ? [e] : u.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
@@ -510,69 +510,72 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 })
             }
             var ne = a(8880);
-            const de = e => ((0, l.dD)("data-v-8c264956"), e = e(), (0, l.Cn)(), e),
-                re = ["width", "height"],
-                ce = ["src"],
-                he = {
+            const de = e => ((0, l.dD)("data-v-2f472339"), e = e(), (0, l.Cn)(), e),
+                re = {
+                    key: 4
+                },
+                ce = ["width", "height"],
+                he = ["src"],
+                ue = {
                     key: 17,
                     class: "web-camera-container"
                 },
-                ue = {
+                pe = {
                     class: "camera-button"
                 },
-                pe = {
+                ge = {
                     key: 0
                 },
-                ge = {
+                me = {
                     key: 1
                 },
-                me = {
+                fe = {
                     class: "camera-loading"
                 },
-                fe = de((() => (0, l._)("ul", {
+                ye = de((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                ye = [fe],
-                we = ["height"],
+                we = [ye],
                 be = ["height"],
-                ke = {
+                ke = ["height"],
+                ve = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ve = de((() => (0, l._)("img", {
+                xe = de((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                xe = [ve],
-                Ce = {
+                Ce = [xe],
+                qe = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function qe(e, t, a, i, o, n) {
+            function _e(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
-                    g = (0, l.up)("q-btn-toggle"),
-                    m = (0, l.up)("utable"),
-                    f = (0, l.up)("linechart"),
-                    y = (0, l.up)("q-input"),
-                    w = (0, l.up)("q-tree"),
-                    b = (0, l.up)("q-scroll-area"),
-                    k = (0, l.up)("q-separator"),
-                    v = (0, l.up)("q-uploader"),
-                    x = (0, l.up)("cgraph"),
-                    C = (0, l.up)("q-btn"),
+                    g = (0, l.up)("q-btn"),
+                    m = (0, l.up)("q-btn-toggle"),
+                    f = (0, l.up)("utable"),
+                    y = (0, l.up)("linechart"),
+                    w = (0, l.up)("q-input"),
+                    b = (0, l.up)("q-tree"),
+                    k = (0, l.up)("q-scroll-area"),
+                    v = (0, l.up)("q-separator"),
+                    x = (0, l.up)("q-uploader"),
+                    C = (0, l.up)("cgraph"),
                     q = (0, l.up)("q-tooltip");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
                     onClick: (0, ne.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
@@ -625,55 +628,49 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, l.wg)(), (0, l.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.j4)(g, {
-                    key: 4,
-                    push: "",
-                    "no-caps": "",
-                    width: "400px",
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", re, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
+                    key: 0,
+                    ripple: !1,
+                    color: "secondary",
+                    disable: "",
+                    label: e.name,
+                    "no-caps": ""
+                }, null, 8, ["label"])) : (0, l.kq)("", !0), (0, l.Wm)(m, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
-                }, {
-                    default: (0, l.w5)((() => [e.showname ? ((0, l.wg)(), (0, l.j4)(c, {
-                        key: 0,
-                        color: "secondary"
-                    }, {
-                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.name), 1)])),
-                        _: 1
-                    })) : (0, l.kq)("", !0)])),
-                    _: 1
-                }, 8, ["modelValue", "options"])) : "table" == e.type ? ((0, l.wg)(), (0, l.j4)(m, {
+                }, null, 8, ["modelValue", "options"])])) : "table" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
                     key: 6,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
-                }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
+                }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
@@ -694,21 +691,21 @@
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
-                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
+                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
                     key: 10,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(w, {
+                    default: (0, l.w5)((() => [(0, l.Wm)(b, {
                         nodes: e.treeNodes,
                         selected: e.value,
                         "onUpdate:selected": t[8] || (t[8] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[9] || (t[9] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": "",
@@ -720,59 +717,59 @@
                     class: "textarea",
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
                     [ne.nr, e.value]
-                ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
+                ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
                     key: 12,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, ce)], 8, re)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                }, null, 8, he)], 8, ce)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     style: (0, s.j5)(e.elemSize),
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 15,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(C, {
                     key: 16,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", he, [(0, l._)("div", ue, [(0, l._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ue, [(0, l._)("div", pe, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", ge, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", pe, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", me, ye, 512), [
+                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", me, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ge, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", fe, we, 512), [
                     [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
@@ -780,48 +777,48 @@
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, we), [
+                }, null, 8, be), [
                     [ne.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, be), [
+                }, null, 8, ke), [
                     [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [ne.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", ke, [(0, l._)("button", {
+                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", ve, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, xe)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", Ce, [(0, l.Wm)(C, {
+                }, Ce)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(C, {
+                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 18,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
                     default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, l.kq)("", !0)])),
                     _: 1
-                }, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(C, {
+                }, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(g, {
                     key: 19,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
                     default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
@@ -830,23 +827,23 @@
                     }, {
                         default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, l.kq)("", !0)])),
                     _: 1
                 }, 8, ["icon", "onClick"]))
             }
-            const _e = {
+            const je = {
                     key: 0
                 },
-                je = {
+                Se = {
                     class: "row"
                 },
-                Se = ["onClick"];
+                ze = ["onClick"];
 
-            function ze(e, t, a, i, o, n) {
+            function Ae(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-tooltip"),
                     c = (0, l.up)("q-input"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
@@ -868,15 +865,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l._)("div", je, [(0, l.Wm)(c, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", je, [(0, l._)("div", Se, [(0, l.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, l.Nv)({
                         append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
@@ -1057,34 +1054,34 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, Se))])),
+                            }, (0, s.zw)(t.row[a.name]), 9, ze))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var Ae = a(1959);
+            var Ze = a(1959);
 
-            function Ze(e, t) {
+            function De(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
             const Me = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, Ae.BK)(e);
+                    } = (0, Ze.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
                                 o = i.length;
@@ -1098,17 +1095,17 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         o = i(),
-                        n = (0, Ae.iH)(o),
-                        d = (0, Ae.iH)(o),
-                        r = (0, Ae.iH)(!Array.isArray(t.value.value)),
+                        n = (0, Ze.iH)(o),
+                        d = (0, Ze.iH)(o),
+                        r = (0, Ze.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
                             q([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
@@ -1137,33 +1134,32 @@
                         this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
                             const l = e.iiid;
                             let s = this.data.rows;
-                            s[l][a] = e[t], this.sendMessage("#", [e[t],
+                            s[l][a] = e[t], this.sendMessage("modify", [e[t],
                                 [l, a]
                             ])
                         }
                     },
                     change(e) {
                         if (g && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
                             let a = this.data.rows;
-                            a[t][this.cedit] = e, this.sendMessage("#", [e, [t, this.cedit]])
+                            a[t][this.cedit] = e, this.sendMessage("modify", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
                         if ("Control" == e.key) return;
-                        g && console.log("keypress", e);
                         let t = !1;
                         switch (e.key) {
                             case "Enter":
-                                "update" in this.data && this.sendMessage("->", [this.rows[this.redit][this.data.headers[this.cedit]],
+                                "update" in this.data && this.sendMessage("update", [this.rows[this.redit][this.data.headers[this.cedit]],
                                     [this.redit, this.cedit]
                                 ]), t = !0;
                             case "ArrowRight":
                                 if (e.ctrlKey || t)
                                     for (let e = this.cedit + 1; e < this.data.rows[this.redit].length; e++) {
                                         let t = typeof this.data.rows[this.redit][e];
                                         if ("string" == t || "number" == t) {
@@ -1214,61 +1210,61 @@
                             a = this;
                         A(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return u.error(l);
                             g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
-                        }), "+")
+                        }), "append")
                     },
                     showSelected() {
                         let e = this.$refs.table;
                         if (this.selected.length) {
                             let t = e.computedRows.findIndex((e => e.iiid === this.selected[0].iiid));
                             e.scrollTo(t)
                         }
                     },
                     deselectAll() {
-                        this.selected = [], this.sendMessage("=", this.value)
+                        this.selected = [], this.sendMessage("changed", this.value)
                     },
                     chart() {
                         let e = this.data;
                         e.type = "linechart"
                     },
                     switchMode() {
                         this.singleMode = !this.singleMode, this.singleMode && this.selected.length > 1 && this.selected.splice(1)
                     },
                     switchEdit() {
-                        this.editMode = !this.editMode, this.sendMessage("!", this.editMode), this.editMode && !this.singleMode && this.switchMode()
+                        this.editMode = !this.editMode, this.editMode && !this.singleMode && this.switchMode()
                     },
                     delSelected() {
                         if (!this.selected.length) return void u.error("Rows are not selected!");
-                        this.sendMessage("-", this.value);
+                        this.sendMessage("delete", this.value);
                         let e = this.data.rows;
                         if (this.singleMode) e.splice(this.selected[0].iiid, 1);
                         else {
                             this.selected.length > 1 && this.selected.sort(((e, t) => t.iiid - e.iiid));
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!Ze(this.updated, this.selected)) {
+                        if (!De(this.updated, this.selected)) {
                             let e = this.selected.length;
-                            this.sendMessage("=", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
+                            this.sendMessage("changed", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
                     redit() {
-                        return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
+                        return this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
                         return 0 != this.data["edit"]
                     },
                     name() {
                         return "_" == this.data.name ? "" : this.data.name
                     },
@@ -1284,52 +1280,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var De = a(9267),
-                $e = a(4842),
-                Ve = a(8870),
-                Ee = a(2165),
-                Ke = a(8186),
-                Oe = a(2414),
+            var $e = a(9267),
+                Ve = a(4842),
+                Ee = a(8870),
+                Ke = a(2165),
+                Oe = a(8186),
+                We = a(2414),
                 Qe = a(3884),
-                We = a(5735),
-                He = a(7208);
-            const Ue = (0, U.Z)(Me, [
-                    ["render", ze]
+                He = a(5735),
+                Ue = a(7208);
+            const Ne = (0, U.Z)(Me, [
+                    ["render", Ae]
                 ]),
-                Ne = Ue;
+                Fe = Ne;
             R()(Me, "components", {
-                QTable: De.Z,
-                QInput: $e.Z,
+                QTable: $e.Z,
+                QInput: Ve.Z,
                 QIcon: P.Z,
-                QTooltip: Ve.Z,
-                QBtn: Ee.Z,
-                QTr: Ke.Z,
-                QTh: Oe.Z,
+                QTooltip: Ee.Z,
+                QBtn: Ke.Z,
+                QTr: Oe.Z,
+                QTh: We.Z,
                 QTd: Qe.Z,
-                QCheckbox: We.Z,
-                QSelect: He.Z
+                QCheckbox: He.Z,
+                QSelect: Ue.Z
             });
-            const Fe = ["nodes", "edges"];
+            const Pe = ["nodes", "edges"];
 
-            function Pe(e, t, a, i, o, n) {
+            function Te(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Fe)
+                }, null, 12, Pe)
             }
-            var Te = a(2393),
-                Ie = a.n(Te);
-            const Re = Ie().stylesheet().selector("node").css({
+            var Ie = a(2393),
+                Re = a.n(Ie);
+            const Le = Re().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1354,50 +1350,50 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray",
                     "font-size": "12px"
                 }),
-                Le = {
+                Be = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Be(e, t) {
+            function Ye(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Ye = (0, l.aZ)({
+            const Xe = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Re,
-                            layoutOptions: Le,
+                            style: Le,
+                            layoutOptions: Be,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: [],
                             shiftKey: !1
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Ie()({
+                        let e = Re()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1412,24 +1408,24 @@
                         e.on("tap", "node", (t => {
                             const a = t.target;
                             if (a.hasClass("selected")) {
                                 a.removeClass("selected");
                                 let e = a.id();
                                 l.selectedNodes = l.shiftKey ? l.selectedNodes.filter((t => t !== e)) : []
                             } else !l.shiftKey && l.selectedEdges.length > 0 && (e.$(".selected").removeClass("selected"), l.selectedEdges = []), a.addClass("selected"), l.selectedNodes.push(a.id());
-                            l.sendMessage("=", {
+                            l.sendMessage("changed", {
                                 nodes: l.selectedNodes,
                                 edges: l.selectedEdges
                             })
                         })), e.on("click", (function(t) {
                             let a = t.target;
                             if ("id" in a && (a === e || "edges" == t.target.group())) {
                                 l.shiftKey || e.edges().removeClass("highlighted");
                                 let t = a.id();
-                                l.selectedEdges.includes(t) ? (l.selectedEdges = l.shiftKey ? l.selectedEdges.filter((e => e != t)) : [], e.edges("[id='" + t + "']").removeClass("highlighted")) : (e.edges("[id='" + t + "']").addClass("highlighted"), l.shiftKey ? l.selectedEdges.push(t) : l.selectedEdges = [t]), l.sendMessage("=", {
+                                l.selectedEdges.includes(t) ? (l.selectedEdges = l.shiftKey ? l.selectedEdges.filter((e => e != t)) : [], e.edges("[id='" + t + "']").removeClass("highlighted")) : (e.edges("[id='" + t + "']").addClass("highlighted"), l.shiftKey ? l.selectedEdges.push(t) : l.selectedEdges = [t]), l.sendMessage("changed", {
                                     nodes: l.selectedNodes,
                                     edges: l.selectedEdges
                                 })
                             }
                         }))
                     },
                     computed: {
@@ -1517,18 +1513,17 @@
                             if (a) {
                                 t.length && a.$(".highlighted").removeClass("highlighted");
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
-                                console.log("wa gr");
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Ye(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Ye(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1545,43 +1540,43 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Xe = (0, U.Z)(Ye, [
-                    ["render", Pe]
+                Ge = (0, U.Z)(Xe, [
+                    ["render", Te]
                 ]),
-                Ge = Xe;
+                Je = Ge;
 
-            function Je(e, t, a, i, o, n) {
+            function et(e, t, a, i, o, n) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
                     option: o.options,
                     style: (0, s.j5)(a.styleSize),
                     autoresize: !0,
                     onClick: n.clicked
                 }, null, 8, ["option", "style", "onClick"])
             }
-            var et = a(5512),
-                tt = a(4447),
-                at = a(1006),
-                lt = a(3526),
-                st = a(763),
-                it = a(546),
-                ot = a(6902),
-                nt = a(2826),
-                dt = a(5256),
-                rt = a(3825),
-                ct = a(8825);
-            (0, st.D)([tt.N, at.N, lt.N]), (0, st.D)([it.N, ot.N, nt.N, dt.N, rt.N]);
-            let ht = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
-                ut = {
+            var tt = a(5512),
+                at = a(4447),
+                lt = a(1006),
+                st = a(3526),
+                it = a(763),
+                ot = a(546),
+                nt = a(6902),
+                dt = a(2826),
+                rt = a(5256),
+                ct = a(3825),
+                ht = a(8825);
+            (0, it.D)([at.N, lt.N, st.N]), (0, it.D)([ot.N, nt.N, dt.N, rt.N, ct.N]);
+            let ut = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
+                pt = {
                     responsive: !0,
                     maintainAspectRatio: !1,
                     legend: {
                         data: [],
                         bottom: 10
                     },
                     tooltip: {
@@ -1616,26 +1611,26 @@
                         end: 10
                     }, {
                         start: 0,
                         end: 10
                     }],
                     series: []
                 };
-            const pt = {
+            const gt = {
                     name: "linechart",
                     components: {
-                        VChart: et.ZP
+                        VChart: tt.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ct.Z)();
+                        const e = (0, ht.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: null
                         }
                     },
                     methods: {
@@ -1664,75 +1659,75 @@
                             let s = [];
                             for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
                                 name: t[l[o]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ht[o]
+                                    color: ut[o]
                                 },
                                 data: s[o]
                             }), this.options.legend.data.push(t[l[o]]));
                             this.options.xAxis.data = s[0];
                             let i = this.data.rows;
                             for (let o = 0; o < i.length; o++)
                                 for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
                             this.$refs.chart.setOption(this.options)
                         }
                     },
                     mounted() {
-                        this.options = (0, h.cloneDeep)(ut), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
+                        this.options = (0, h.cloneDeep)(pt), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
                     },
                     watch: {}
                 },
-                gt = (0, U.Z)(pt, [
-                    ["render", Je]
+                mt = (0, U.Z)(gt, [
+                    ["render", et]
                 ]),
-                mt = gt;
+                ft = mt;
 
-            function ft(e) {
+            function yt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const yt = (0, l.aZ)({
+            const wt = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Ne,
-                    cgraph: Ge,
-                    linechart: mt
+                    utable: Fe,
+                    cgraph: Je,
+                    linechart: ft
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
                         q([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
-                        "update" in this.data && this.sendMessage("->", this.value)
+                        "update" in this.data && this.sendMessage("update", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("=", e.files[t - 1].name), K())
+                        t && (this.sendMessage("changed", e.files[t - 1].name), K())
                     },
                     sendValue() {
-                        this.sendMessage("=", this.value)
+                        this.sendMessage("changed", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
-                        console.log(e), this.value = e
+                        this.value = e
                     },
                     complete(e, t, a) {
                         this.value = e, A(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
@@ -1768,15 +1763,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
@@ -1788,15 +1783,15 @@
                             top: l.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
-                    k[this.fullname] = this, g && console.log("mounted", this.fullname)
+                    k[this.fullname] = this
                 },
                 data() {
                     return {
                         value: this.data.value,
                         styleSize: w(this.data),
                         options: [],
                         expandedKeys: [],
@@ -1897,61 +1892,61 @@
                     pdata: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     value(e, t) {
-                        "tree" == this.type && this.data.options[e] == t && this.expandedKeys.indexOf(t) < 0 && this.expandedKeys.push(t), e !== this.updated && (g && console.log("value changed", e, t), this.sendValue(), this.updated = e)
+                        "tree" == this.type && this.data.options[e] == t && this.expandedKeys.indexOf(t) < 0 && this.expandedKeys.push(t), e !== this.updated && (this.sendValue(), this.updated = e)
                     },
                     selection(e) {
-                        g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
+                        Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.styleSize || (this.styleSize = w(this.data), g && console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
+                        this.styleSize || (this.styleSize = w(this.data)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var wt = a(4027),
-                bt = a(9721),
-                kt = a(8886),
-                vt = a(8761),
-                xt = a(1232),
-                Ct = a(5551),
-                qt = a(5869),
-                _t = a(1745);
-            const jt = (0, U.Z)(yt, [
-                    ["render", qe],
-                    ["__scopeId", "data-v-8c264956"]
+            var bt = a(4027),
+                kt = a(9721),
+                vt = a(8886),
+                xt = a(8761),
+                Ct = a(1232),
+                qt = a(5551),
+                _t = a(5869),
+                jt = a(1745);
+            const St = (0, U.Z)(wt, [
+                    ["render", _e],
+                    ["__scopeId", "data-v-2f472339"]
                 ]),
-                St = jt;
-            R()(yt, "components", {
-                QImg: wt.Z,
+                zt = St;
+            R()(wt, "components", {
+                QImg: bt.Z,
                 QIcon: P.Z,
-                QSelect: He.Z,
-                QBadge: bt.Z,
-                QCheckbox: We.Z,
-                QToggle: kt.Z,
-                QBtnToggle: vt.Z,
-                QInput: $e.Z,
-                QScrollArea: xt.Z,
-                QTree: Ct.Z,
-                QSeparator: qt.Z,
-                QUploader: _t.Z,
-                QBtn: Ee.Z,
-                QTooltip: Ve.Z
+                QSelect: Ue.Z,
+                QBadge: kt.Z,
+                QCheckbox: He.Z,
+                QToggle: vt.Z,
+                QBtn: Ke.Z,
+                QBtnToggle: xt.Z,
+                QInput: Ve.Z,
+                QScrollArea: Ct.Z,
+                QTree: qt.Z,
+                QSeparator: _t.Z,
+                QUploader: jt.Z,
+                QTooltip: Ee.Z
             });
-            const zt = (0, l.aZ)({
+            const At = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: St
+                    element: zt
                 },
                 data() {
                     return {
                         styleSize: y,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -2018,25 +2013,25 @@
                 },
                 watch: {
                     data(e) {
                         g && console.log("data update", this.name), this.styleSize = y, b[this.name] = this, this.expanding && (k[this.fullname] = this)
                     }
                 }
             });
-            var At = a(151);
-            const Zt = (0, U.Z)(zt, [
+            var Zt = a(151);
+            const Dt = (0, U.Z)(At, [
                     ["render", oe]
                 ]),
-                Mt = Zt;
-            R()(zt, "components", {
-                QCard: At.Z,
+                Mt = Dt;
+            R()(At, "components", {
+                QCard: Zt.Z,
                 QIcon: P.Z,
-                QScrollArea: xt.Z
+                QScrollArea: Ct.Z
             });
-            const Dt = (0, l.aZ)({
+            const $t = (0, l.aZ)({
                     name: "zone",
                     components: {
                         block: Mt
                     },
                     props: {
                         data: Object
                     },
@@ -2046,23 +2041,23 @@
                                 requestAnimationFrame((() => {
                                     O()
                                 }))
                             }))
                         }))
                     }
                 }),
-                $t = (0, U.Z)(Dt, [
+                Vt = (0, U.Z)($t, [
                     ["render", J]
                 ]),
-                Vt = $t,
-                Et = {
+                Et = Vt,
+                Kt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Kt(e, t, a, i, o, n) {
+            function Ot(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -2078,26 +2073,26 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Et, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Kt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const Ot = {
+            const Wt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
                     block: Mt
                 },
@@ -2120,27 +2115,26 @@
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
             var Qt = a(5926),
-                Wt = a(2025);
-            const Ht = (0, U.Z)(Ot, [
-                    ["render", Kt]
+                Ht = a(2025);
+            const Ut = (0, U.Z)(Wt, [
+                    ["render", Ot]
                 ]),
-                Ut = Ht;
-            R()(Ot, "components", {
+                Nt = Ut;
+            R()(Wt, "components", {
                 QDialog: Qt.Z,
-                QCard: At.Z,
+                QCard: Zt.Z,
                 QItemLabel: T.Z,
-                QSpace: Wt.Z,
-                QBtn: Ee.Z
+                QSpace: Ht.Z,
+                QBtn: Ke.Z
             });
-            var Nt = !0;
             let Ft = null;
             const Pt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
@@ -2153,16 +2147,16 @@
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
                     menubar: B,
-                    zone: Vt,
-                    element: St
+                    zone: Et,
+                    element: zt
                 },
                 created() {
                     C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
@@ -2178,15 +2172,15 @@
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ut
+                                component: Nt
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -2223,34 +2217,33 @@
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (Nt) Nt = !1, this.menu = e[0].map((e => ({
+                        if ("screen" == e.type) this.screen.name != e.name && z(), Z(), this.screen = e, console.log(e), this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
-                        }))), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
-                        else if ("screen" == e.type) this.screen.name != e.name && z(), Z(), this.screen = e;
+                        }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ut, t.componentProps = {
+                            t.component = Nt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if (e.hasOwnProperty("answer")) $(e);
                         else {
-                            e.update && D(e);
+                            e.update && M(e);
                             let t = !1;
                             for (let a of v) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
                         Ft && !e.progress && this.notify(null, "progress")
                     }
                 },
@@ -2269,15 +2262,15 @@
                     ["render", n]
                 ]),
                 Jt = Gt;
             R()(Pt, "components", {
                 QLayout: Tt.Z,
                 QHeader: It.Z,
                 QToolbar: Rt.Z,
-                QBtn: Ee.Z,
+                QBtn: Ke.Z,
                 QItemLabel: T.Z,
                 QTabs: Lt.Z,
                 QTab: Bt.Z,
                 QPageContainer: Yt.Z,
                 QPage: Xt.Z
             })
         }
```

### Comparing `unigui-1.7.3/unigui/web/js/app.b39a06ae.js` & `unigui-1.8.0/unigui/web/js/app.fc1b2f39.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -14,23 +14,23 @@
                     const s = (0, a.up)("router-view");
                     return (0, a.wg)(), (0, a.iD)("div", i, [(0, a.Wm)(s)])
                 }
                 const s = (0, a.aZ)({
                     name: "App"
                 });
                 var u = r(4260);
-                const d = (0, u.Z)(s, [
+                const c = (0, u.Z)(s, [
                         ["render", l]
                     ]),
-                    c = d;
+                    d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(878)]).then(r.bind(r, 6878)),
+                        component: () => Promise.all([r.e(736), r.e(223)]).then(r.bind(r, 4223)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -46,15 +46,15 @@
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
                 async function g(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
-                        n = e(c);
+                        n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
                 var b = r(6417),
                     y = r(5597);
@@ -126,27 +126,27 @@
         return e[n].call(a.exports, a, a.exports, r), a.loaded = !0, a.exports
     }
     r.m = e, (() => {
         var e = [];
         r.O = (t, n, o, a) => {
             if (!n) {
                 var i = 1 / 0;
-                for (d = 0; d < e.length; d++) {
-                    for (var [n, o, a] = e[d], l = !0, s = 0; s < n.length; s++)(!1 & a || i >= a) && Object.keys(r.O).every((e => r.O[e](n[s]))) ? n.splice(s--, 1) : (l = !1, a < i && (i = a));
+                for (c = 0; c < e.length; c++) {
+                    for (var [n, o, a] = e[c], l = !0, s = 0; s < n.length; s++)(!1 & a || i >= a) && Object.keys(r.O).every((e => r.O[e](n[s]))) ? n.splice(s--, 1) : (l = !1, a < i && (i = a));
                     if (l) {
-                        e.splice(d--, 1);
+                        e.splice(c--, 1);
                         var u = o();
                         void 0 !== u && (t = u)
                     }
                 }
                 return t
             }
             a = a || 0;
-            for (var d = e.length; d > 0 && e[d - 1][2] > a; d--) e[d] = e[d - 1];
-            e[d] = [n, o, a]
+            for (var c = e.length; c > 0 && e[c - 1][2] > a; c--) e[c] = e[c - 1];
+            e[c] = [n, o, a]
         }
     })(), (() => {
         r.n = e => {
             var t = e && e.__esModule ? () => e["default"] : () => e;
             return r.d(t, {
                 a: t
             }), t
@@ -159,25 +159,25 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            430: "591e9a73",
-            878: "e76799d2"
+            223: "7924e6b0",
+            430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            736: "49a52e8f",
-            878: "c6483fb6"
+            223: "f0f63b8f",
+            736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -190,18 +190,18 @@
         var e = {},
             t = "uniqua:";
         r.l = (n, o, a, i) => {
             if (e[n]) e[n].push(o);
             else {
                 var l, s;
                 if (void 0 !== a)
-                    for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                        var c = u[d];
-                        if (c.getAttribute("src") == n || c.getAttribute("data-webpack") == t + a) {
-                            l = c;
+                    for (var u = document.getElementsByTagName("script"), c = 0; c < u.length; c++) {
+                        var d = u[c];
+                        if (d.getAttribute("src") == n || d.getAttribute("data-webpack") == t + a) {
+                            l = d;
                             break
                         }
                     }
                 l || (s = !0, l = document.createElement("script"), l.charset = "utf-8", l.timeout = 120, r.nc && l.setAttribute("nonce", r.nc), l.setAttribute("data-webpack", t + a), l.src = n), e[n] = [o];
                 var p = (t, r) => {
                         l.onerror = l.onload = null, clearTimeout(f);
                         var o = e[n];
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                878: 1
+                223: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
@@ -296,18 +296,18 @@
                 }
         }, r.O.j = t => 0 === e[t];
         var t = (t, n) => {
                 var o, a, [i, l, s] = n,
                     u = 0;
                 if (i.some((t => 0 !== e[t]))) {
                     for (o in l) r.o(l, o) && (r.m[o] = l[o]);
-                    if (s) var d = s(r)
+                    if (s) var c = s(r)
                 }
                 for (t && t(n); u < i.length; u++) a = i[u], r.o(e, a) && e[a] && e[a][0](), e[i[u]] = 0;
-                return r.O(d)
+                return r.O(c)
             },
             n = globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || [];
         n.forEach(t.bind(null, 0)), n.push = t.bind(null, n.push.bind(n))
     })();
     var n = r.O(void 0, [736], (() => r(653)));
     n = r.O(n)
 })();
```

### Comparing `unigui-1.7.3/unigui/web/js/193.283445be.js` & `unigui-1.8.0/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.8.0/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/unigui/web/index.html` & `unigui-1.8.0/unigui/web/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.b39a06ae.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.fc1b2f39.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.7.3/LICENSE` & `unigui-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.7.3/setup.py` & `unigui-1.8.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.7.3',      
+      version='1.8.0',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.7.3/PKG-INFO` & `unigui-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.7.3
+Version: 1.8.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -406,14 +406,14 @@
 unigui.start('Hello app', user_type = Hello_user)
 ```
 In screens and blocks sources we can access the user by 'user' variable
 ```
 print(isinstance(user, Hello_user))
 ```
 
-More info about User class methods you can find in manager.py in the souce dir.
+More info about User class methods you can find in user.py in the souce dir.
 
 Examples are in tests folder.
 
 Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.7.3/README.md` & `unigui-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -394,12 +394,12 @@
 unigui.start('Hello app', user_type = Hello_user)
 ```
 In screens and blocks sources we can access the user by 'user' variable
 ```
 print(isinstance(user, Hello_user))
 ```
 
-More info about User class methods you can find in manager.py in the souce dir.
+More info about User class methods you can find in user.py in the souce dir.
 
 Examples are in tests folder.
 
 Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.7.3/unigui.egg-info/PKG-INFO` & `unigui-1.8.0/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.7.3
+Version: 1.8.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -406,14 +406,14 @@
 unigui.start('Hello app', user_type = Hello_user)
 ```
 In screens and blocks sources we can access the user by 'user' variable
 ```
 print(isinstance(user, Hello_user))
 ```
 
-More info about User class methods you can find in manager.py in the souce dir.
+More info about User class methods you can find in user.py in the souce dir.
 
 Examples are in tests folder.
 
 Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.7.3/unigui.egg-info/SOURCES.txt` & `unigui-1.8.0/unigui.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 unigui/__init__.py
 unigui/guielements.py
-unigui/manager.py
 unigui/server.py
+unigui/user.py
 unigui/utils.py
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/878.c6483fb6.css
+unigui/web/css/223.f0f63b8f.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -27,11 +27,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
+unigui/web/js/223.7924e6b0.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/878.e76799d2.js
-unigui/web/js/app.b39a06ae.js
+unigui/web/js/app.fc1b2f39.js
 unigui/web/js/vendor.3e8714c2.js
```

