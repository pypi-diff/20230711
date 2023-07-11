# Comparing `tmp/nodered.py-0.2.6.tar.gz` & `tmp/nodered.py-0.2.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.6.tar", last modified: Mon Jul 10 09:13:53 2023, max compression
+gzip compressed data, was "nodered.py-0.2.6.post1.tar", last modified: Tue Jul 11 11:51:53 2023, max compression
```

## Comparing `nodered.py-0.2.6.tar` & `nodered.py-0.2.6.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.580000 nodered.py-0.2.6/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.6/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2575 2023-07-10 09:13:53.640000 nodered.py-0.2.6/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2259 2023-07-10 09:05:46.000000 nodered.py-0.2.6/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.580000 nodered.py-0.2.6/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2575 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.6/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.580000 nodered.py-0.2.6/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-10 09:12:12.000000 nodered.py-0.2.6/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    18790 2023-07-10 09:11:19.000000 nodered.py-0.2.6/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.6/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.600000 nodered.py-0.2.6/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.6/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.6/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.600000 nodered.py-0.2.6/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.6/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.6/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.6/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.600000 nodered.py-0.2.6/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.6/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.6/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4998 2023-07-10 01:49:09.000000 nodered.py-0.2.6/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.6/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-10 09:13:53.640000 nodered.py-0.2.6/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.6/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 11:51:53.180000 nodered.py-0.2.6.post1/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.6.post1/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2581 2023-07-11 11:51:53.290000 nodered.py-0.2.6.post1/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2259 2023-07-10 09:05:46.000000 nodered.py-0.2.6.post1/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 11:51:53.180000 nodered.py-0.2.6.post1/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2581 2023-07-11 11:51:53.000000 nodered.py-0.2.6.post1/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-11 11:51:53.000000 nodered.py-0.2.6.post1/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-11 11:51:53.000000 nodered.py-0.2.6.post1/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-11 11:51:53.000000 nodered.py-0.2.6.post1/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-11 11:51:53.000000 nodered.py-0.2.6.post1/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.6.post1/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 11:51:53.180000 nodered.py-0.2.6.post1/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      480 2023-07-11 11:51:00.000000 nodered.py-0.2.6.post1/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    19081 2023-07-11 11:47:47.000000 nodered.py-0.2.6.post1/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.6.post1/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 11:51:53.210000 nodered.py-0.2.6.post1/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.6.post1/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.6.post1/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 11:51:53.210000 nodered.py-0.2.6.post1/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.6.post1/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.6.post1/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.6.post1/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 11:51:53.210000 nodered.py-0.2.6.post1/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.6.post1/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.6.post1/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5788 2023-07-11 11:51:18.000000 nodered.py-0.2.6.post1/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.6.post1/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-11 11:51:53.290000 nodered.py-0.2.6.post1/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.6.post1/setup.py
```

### Comparing `nodered.py-0.2.6/LICENSE` & `nodered.py-0.2.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/PKG-INFO` & `nodered.py-0.2.6.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.6
+Version: 0.2.6.post1
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6 Summary: make python
-function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
-Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6.post1 Summary: make
+python function to Node-RED node Home-page: https://github.com/oyajiDev/
+NodeRED.py Author: oyajiDev Author-email: this.dev.somehit@gmail.com License:
+MIT license Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
```

### Comparing `nodered.py-0.2.6/README.md` & `nodered.py-0.2.6.post1/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.6.post1/nodered.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.6
+Version: 0.2.6.post1
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6 Summary: make python
-function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
-Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6.post1 Summary: make
+python function to Node-RED node Home-page: https://github.com/oyajiDev/
+NodeRED.py Author: oyajiDev Author-email: this.dev.somehit@gmail.com License:
+MIT license Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
```

### Comparing `nodered.py-0.2.6/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.6.post1/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/_nodered.py` & `nodered.py-0.2.6.post1/noderedpy/_nodered.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,24 @@
             Node(
                 name, category,
                 version, description, author, keywords,
                 icon, properties, node_func
             )
         )
 
+    # write output
+    def __write_output(self, output_file:str, res:dict):
+        try:
+            with open(output_file, "w", encoding = "utf-8") as ofw:
+                json.dump(res, ofw, indent = 4)
+        except:
+            os.remove(output_file)
+            res["req"]["body"] = {}
+            self.__write_output(output_file, res)
+
     # check input and run node
     def __check_input_from_node(self):
         input_file, output_file = os.path.join(self.__cache_dir, "input.json"), os.path.join(self.__cache_dir, "output.json")
 
         while True:
             if os.path.exists(input_file):
                 # read input file
@@ -234,16 +244,18 @@
                         os.remove(input_file)
                         break
                     except json.JSONDecodeError:
                         pass
 
                 node = list(filter(lambda n: n.name == input_data["name"], RED.registered_nodes))[0]
 
-                with open(output_file, "w", encoding = "utf-8") as ofw:
-                    json.dump(node.run(input_data["props"], input_data["msg"]), ofw, indent = 4)
+                self.__write_output(
+                    output_file,
+                    node.run(input_data["props"], input_data["msg"])
+                )
 
     def start(self, callback:MethodType = None, debug:bool = True, start_browser:bool = True):
         """
         Start Node-RED server
 
         Parameters
         ----------
@@ -441,9 +453,8 @@
             resp = self.__node_func(self.__communicator, props, msg)
             print("============================= ended\n")
 
             resp.update({ "state": "success", "name": self.name })
 
             return resp
         except:
-            print("============================= error\n")
-            return { "state": "fail", "message": traceback.format_exc() }
+            return { "state": "fail", "name": self.name, "message": traceback.format_exc() }
```

### Comparing `nodered.py-0.2.6/noderedpy/_property.py` & `nodered.py-0.2.6.post1/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/assets/python-logo.png` & `nodered.py-0.2.6.post1/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/decorator.py` & `nodered.py-0.2.6.post1/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.6.post1/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/templates/__init__.py` & `nodered.py-0.2.6.post1/noderedpy/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/templates/template.html` & `nodered.py-0.2.6.post1/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6/noderedpy/templates/template.js` & `nodered.py-0.2.6.post1/noderedpy/templates/template.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,17 @@
 const fs = require("fs"),
     path = require("path");
 
 let messageCache = {};
 
+function $sleep(ms) {
+    const wakeUpTime = Date.now() + ms;
+    while (Date.now() < wakeUpTime) {}
+}
+
 module.exports = function(RED) {
     function fnNode(config) {
         var node = this;
         RED.nodes.createNode(this, config);
 
         this.status({
             fill: "blue",
@@ -18,19 +23,32 @@
             delete message._msgid;
 
             var reqToSend = null;
             if (message.req != undefined && typeof(message.req) == "object") {
                 messageCache.req = message.req;
 
                 reqToSend = {
-                    payload: message.req.payload,
-                    body: message.req.body,
-                    cookie: message.req.cookie,
                     header: {}
                 };
+                try {
+                    reqToSend.payload = JSON.parse(message.req.payload);
+                } catch {
+                    reqToSend.payload = message.req.payload;
+                }
+                try {
+                    reqToSend.body = JSON.parse(message.req.body);
+                } catch {
+                    reqToSend.body = message.req.body;
+                }
+                try {
+                    reqToSend.cookie = JSON.parse(message.req.cookie);
+                } catch {
+                    reqToSend.cookie = message.req.cookie;
+                }
+
                 for (var idx = 0; idx < message.req.rawHeaders.length / 2; idx++) {
                     reqToSend.header[message.req.rawHeaders[idx * 2]] = message.req.rawHeaders[idx * 2 + 1].replaceAll('"', "'");
                 }
 
                 message.req = reqToSend;
             }
             if (message.res != undefined && typeof(message.res) == "object") {
@@ -102,14 +120,15 @@
                     try {
                         resp = JSON.parse(fs.readFileSync(outFile));
                         if (resp.name == "{$node_name}") {
                             fs.unlinkSync(outFile);
                             break;
                         }
                     } catch {
+                        // $sleep(1000);
                         continue;
                     }
                 }
             }
 
             // get result ans parse
             try {
@@ -128,23 +147,25 @@
                     node.send(resp);
                     node.status({
                         fill: "green",
                         shape: "dot",
                         text: "Finished"
                     });
                 } else {
-                    node.error(resp.message);
+                    node.error("\n" + resp.message);
+                    console.log("============================= error\n");
                     node.status({
                         fill: "red",
                         shape: "dot",
                         text: "Stopped, see debug panel"
                     });
                 }
             } catch (err) {
-                node.error(err.message);
+                node.error("\n" + err.message);
+                console.log("============================= error\n");
                 node.status({
                     fill: "red",
                     shape: "dot",
                     text: "Stopped, see debug panel"
                 });
             }
         });
```

### Comparing `nodered.py-0.2.6/setup.py` & `nodered.py-0.2.6.post1/setup.py`

 * *Files identical despite different names*

