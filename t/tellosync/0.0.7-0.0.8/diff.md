# Comparing `tmp/tellosync-0.0.7.tar.gz` & `tmp/tellosync-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellosync-0.0.7.tar", last modified: Thu Jun 29 13:27:00 2023, max compression
+gzip compressed data, was "tellosync-0.0.8.tar", last modified: Tue Jul 11 13:01:06 2023, max compression
```

## Comparing `tellosync-0.0.7.tar` & `tellosync-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:27:00.675646 tellosync-0.0.7/
--rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2619 2023-06-29 13:27:00.674521 tellosync-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2041 2023-06-29 02:55:12.000000 tellosync-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 13:27:00.675646 tellosync-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-06-29 13:26:53.000000 tellosync-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:27:00.608807 tellosync-0.0.7/tellosync/
--rw-rw-rw-   0        0        0      275 2023-06-29 13:26:55.000000 tellosync-0.0.7/tellosync/__init__.py
--rw-rw-rw-   0        0        0     2227 2023-06-27 11:55:49.000000 tellosync-0.0.7/tellosync/stats.py
--rw-rw-rw-   0        0        0     1072 2023-06-29 02:03:12.000000 tellosync-0.0.7/tellosync/synchro.py
--rw-rw-rw-   0        0        0     8878 2023-06-29 13:17:50.000000 tellosync-0.0.7/tellosync/tello.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:27:00.669396 tellosync-0.0.7/tellosync.egg-info/
--rw-rw-rw-   0        0        0     2619 2023-06-29 13:27:00.000000 tellosync-0.0.7/tellosync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-29 13:27:00.000000 tellosync-0.0.7/tellosync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:27:00.000000 tellosync-0.0.7/tellosync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-29 13:27:00.000000 tellosync-0.0.7/tellosync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 13:27:00.000000 tellosync-0.0.7/tellosync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 13:01:06.351236 tellosync-0.0.8/
+-rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2619 2023-07-11 13:01:06.343237 tellosync-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2041 2023-07-10 16:40:19.000000 tellosync-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:01:06.351236 tellosync-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-11 13:01:00.000000 tellosync-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:01:06.303367 tellosync-0.0.8/tellosync/
+-rw-rw-rw-   0        0        0      275 2023-07-11 13:00:58.000000 tellosync-0.0.8/tellosync/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-07-10 16:48:37.000000 tellosync-0.0.8/tellosync/stats.py
+-rw-rw-rw-   0        0        0     1072 2023-06-29 02:03:12.000000 tellosync-0.0.8/tellosync/synchro.py
+-rw-rw-rw-   0        0        0     8453 2023-07-11 13:00:14.000000 tellosync-0.0.8/tellosync/tello.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:01:06.343237 tellosync-0.0.8/tellosync.egg-info/
+-rw-rw-rw-   0        0        0     2619 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/top_level.txt
```

### Comparing `tellosync-0.0.7/LICENSE` & `tellosync-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.7/PKG-INFO` & `tellosync-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.7
+Version: 0.0.8
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tellosync-0.0.7/README.md` & `tellosync-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.7/setup.py` & `tellosync-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tellosync',
-    version='0.0.7',
+    version='0.0.8',
     author='Ezra Fielding, Vincent Wu',
     author_email='ezra.fielding@gmail.com, vwu1888@gmail.com',
     description='An easy framework to support DJI Tello scripting in Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vwu1888/easyTello',
     packages=setuptools.find_packages(),
```

### Comparing `tellosync-0.0.7/tellosync/stats.py` & `tellosync-0.0.8/tellosync/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,20 @@
 
     def temp_response(self):
         raw_temp = self.response.split('~')
         temp = (self.int_response(raw_temp[0]) + self.int_response(raw_temp[1]))/2
         return temp
 
     def get_response(self):
-        if 'attitude?' in self.command:
-            return self.attitude_response()
-        elif 'acceleration?' in self.command:
-            return self.acceleration_response()
-        elif 'temp?' in self.command:
-            return self.temp_response()
-        elif 'baro?' in self.command or 'speed?' in self.command:
-            return self.float_response(self.response)
-        elif '?' not in self.command:
-            return self.get_raw_response()
-        else:
-            return self.int_response(self.response)
+        return self.get_raw_response()
+        # if 'attitude?' in self.command:
+        #     return self.attitude_response()
+        # elif 'acceleration?' in self.command:
+        #     return self.acceleration_response()
+        # elif 'temp?' in self.command:
+        #     return self.temp_response()
+        # elif 'baro?' in self.command or 'speed?' in self.command:
+        #     return self.float_response(self.response)
+        # elif '?' not in self.command:
+        #     return self.get_raw_response()
+        # else:
+        #     return self.int_response(self.response)
```

### Comparing `tellosync-0.0.7/tellosync/synchro.py` & `tellosync-0.0.8/tellosync/synchro.py`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.7/tellosync/tello.py` & `tellosync-0.0.8/tellosync/tello.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if isSynced:
             self.synchro = Synchro(port)
             self.isSynced = self.synchro.open()
 
         # Setting Tello to command mode
         self.command()
 
-    def send_command(self, command: str, delay: float=0.0, query: bool=False, tries: int=0):
+    def send_command(self, command: str, delay: float=0.0, tries: int=0):
         # New log entry created for the outbound command
         self.log.append(Stats(command, len(self.log)))
         currentStats = self.log[-1]
 
         if delay > 0:
             self.wait(delay)
 
@@ -59,27 +59,25 @@
             now = time.time()
             difference = now - start
             if difference > self.MAX_TIME_OUT:
                 currentStats.add_response('Connection timed out!')
                 break
 
         # Prints out Tello response (if 'debug' is True)
-        if self.debug is True and not query:
+        if self.debug is True:
             print(f'Response: {currentStats.get_response()}')
 
-        # sourcery skip: merge-nested-ifs
-        if tries < 3 and currentStats.got_response():
-            if currentStats.get_raw_response() == "error No valid imu" or currentStats.get_raw_response == "error Not joystick":
-                self.socket.sendto("stop".encode('utf-8'), self.tello_address)
-                time.sleep(1.0)
+        if currentStats.get_raw_response() == "error No valid imu" or currentStats.get_raw_response == "error Not joystick":
+            self.socket.sendto("stop".encode('utf-8'), self.tello_address)
+            time.sleep(1.0)
 
         if delay < 0:
             self.wait(abs(delay))
 
-        time.sleep(1.0)
+        time.sleep(0.5)
         self.wait_for_sync()
 
     def _keep_alive(self):
         # Sending command to Tello
         print("Keeping connection alive")
         self.socket.sendto("stop".encode('utf-8'), self.tello_address)
 
@@ -88,14 +86,19 @@
             # Checking for Tello response, throws socket error
             try:
                 self.response, ip = self.socket.recvfrom(1024)
                 self.log[-1].add_response(self.response.decode('utf-8'))
             except socket.error as exc:
                 print(f'Socket error: {exc}')
 
+            try:
+                self.log[-1].add_response(self.response.decode('utf-8'))
+            except UnicodeDecodeError as e:
+                self.log[-1].add_response("Response: utf-8 decode error")
+
     def _video_thread(self):
         # Creating stream capture object
         cap = cv2.VideoCapture(f'udp://{self.tello_ip}:11111')
         # Runs while 'stream_state' is True
         while self.stream_state:
             ret, self.last_frame = cap.read()
             cv2.imshow('DJI Tello', self.last_frame)
@@ -150,16 +153,16 @@
     
     def takeoff(self, delay: float=0.0):
         self.send_command('takeoff', delay)
 
     def land(self, delay: float=0.0):
         if self.isSynced:
             self.synchro.finished()
+            self.synchro.close()
         self.send_command('land', delay)
-        self.synchro.close()
 
     def streamon(self):
         self.send_command('streamon')
         self.stream_state = True
         self.video_thread = threading.Thread(target=self._video_thread)
         self.video_thread.daemon = True
         self.video_thread.start()
@@ -216,45 +219,35 @@
         self.send_command(f'rc {a} {b} {c} {d}')
 
     def set_wifi(self, ssid: str, passwrd: str):
         self.send_command(f'wifi {ssid} {passwrd}')
 
     # Read Commands
     def get_speed(self):
-        self.send_command('speed?', True)
-        return self.log[-1].get_response()
+        self.send_command('speed?')
 
     def get_battery(self):
-        self.send_command('battery?', True)
-        return self.log[-1].get_response()
+        self.send_command('battery?')
 
     def get_time(self):
-        self.send_command('time?', True)
-        return self.log[-1].get_response()
+        self.send_command('time?')
 
     def get_height(self):
-        self.send_command('height?', True)
-        return self.log[-1].get_response()
+        self.send_command('height?')
     
     def get_temp(self):
-        self.send_command('temp?', True)
-        return self.log[-1].get_response()
+        self.send_command('temp?')
 
     def get_attitude(self):
-        self.send_command('attitude?', True)
-        return self.log[-1].get_response()
+        self.send_command('attitude?')
 
     def get_baro(self):
-        self.send_command('baro?', True)
-        return self.log[-1].get_response()
+        self.send_command('baro?')
 
     def get_acceleration(self):
-        self.send_command('acceleration?', True)
-        return self.log[-1].get_response()
+        self.send_command('acceleration?')
     
     def get_tof(self):
-        self.send_command('tof?', True)
-        return self.log[-1].get_response()
+        self.send_command('tof?')
 
     def get_wifi(self):
-        self.send_command('wifi?', True)
-        return self.log[-1].get_response()
+        self.send_command('wifi?')
```

### Comparing `tellosync-0.0.7/tellosync.egg-info/PKG-INFO` & `tellosync-0.0.8/tellosync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.7
+Version: 0.0.8
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

