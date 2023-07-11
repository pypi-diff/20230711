# Comparing `tmp/real-time-tf-0.1.1.tar.gz` & `tmp/real-time-tf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real-time-tf-0.1.1.tar", last modified: Sun Jul  9 15:14:39 2023, max compression
+gzip compressed data, was "real-time-tf-0.1.2.tar", last modified: Tue Jul 11 17:43:55 2023, max compression
```

## Comparing `real-time-tf-0.1.1.tar` & `real-time-tf-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:14:39.001421 real-time-tf-0.1.1/
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1514 2023-07-09 15:08:42.000000 real-time-tf-0.1.1/LICENSE
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1704 2023-07-09 15:14:39.001534 real-time-tf-0.1.1/PKG-INFO
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1317 2023-07-09 14:31:17.000000 real-time-tf-0.1.1/README.md
-drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:14:38.999666 real-time-tf-0.1.1/real_time_tf.egg-info/
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1704 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/PKG-INFO
--rw-r--r--   0 diganta.eth   (501) staff       (20)      360 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/SOURCES.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)        1 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/dependency_links.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)       61 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/entry_points.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)       29 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/requires.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)       12 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/top_level.txt
-drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:14:39.001024 real-time-tf-0.1.1/realtime_tf/
--rw-r--r--   0 diganta.eth   (501) staff       (20)       33 2023-07-09 15:02:30.000000 real-time-tf-0.1.1/realtime_tf/__init__.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)       58 2023-07-09 14:24:52.000000 real-time-tf-0.1.1/realtime_tf/constants.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)     5392 2023-07-09 15:03:05.000000 real-time-tf-0.1.1/realtime_tf/realtime_tf.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)     3013 2023-07-09 14:24:25.000000 real-time-tf-0.1.1/realtime_tf/time_frequency.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)       79 2023-07-09 15:14:39.001930 real-time-tf-0.1.1/setup.cfg
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1151 2023-07-09 15:14:36.000000 real-time-tf-0.1.1/setup.py
+drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-11 17:43:55.261024 real-time-tf-0.1.2/
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1514 2023-07-09 15:08:42.000000 real-time-tf-0.1.2/LICENSE
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1782 2023-07-11 17:43:55.261115 real-time-tf-0.1.2/PKG-INFO
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1395 2023-07-10 06:38:49.000000 real-time-tf-0.1.2/README.md
+drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-11 17:43:55.259336 real-time-tf-0.1.2/real_time_tf.egg-info/
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1782 2023-07-11 17:43:55.000000 real-time-tf-0.1.2/real_time_tf.egg-info/PKG-INFO
+-rw-r--r--   0 diganta.eth   (501) staff       (20)      360 2023-07-11 17:43:55.000000 real-time-tf-0.1.2/real_time_tf.egg-info/SOURCES.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)        1 2023-07-11 17:43:55.000000 real-time-tf-0.1.2/real_time_tf.egg-info/dependency_links.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       61 2023-07-11 17:43:55.000000 real-time-tf-0.1.2/real_time_tf.egg-info/entry_points.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       29 2023-07-11 17:43:55.000000 real-time-tf-0.1.2/real_time_tf.egg-info/requires.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       12 2023-07-11 17:43:55.000000 real-time-tf-0.1.2/real_time_tf.egg-info/top_level.txt
+drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-11 17:43:55.260698 real-time-tf-0.1.2/realtime_tf/
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       33 2023-07-09 15:02:30.000000 real-time-tf-0.1.2/realtime_tf/__init__.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       58 2023-07-09 14:24:52.000000 real-time-tf-0.1.2/realtime_tf/constants.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     5449 2023-07-10 14:51:01.000000 real-time-tf-0.1.2/realtime_tf/realtime_tf.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     3013 2023-07-09 14:24:25.000000 real-time-tf-0.1.2/realtime_tf/time_frequency.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       79 2023-07-11 17:43:55.261449 real-time-tf-0.1.2/setup.cfg
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1151 2023-07-10 14:51:48.000000 real-time-tf-0.1.2/setup.py
```

### Comparing `real-time-tf-0.1.1/LICENSE` & `real-time-tf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `real-time-tf-0.1.1/PKG-INFO` & `real-time-tf-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-time-tf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Real time time frequency plotting of EEG data from the Muse headset.
 Home-page: https://github.com/dxganta/real-time-tf
 Author: Diganta Kalita
 Author-email: digantakalita.ai@gmail.com
 License: BSD (3-clause)
 Keywords: muse time-frequency eeg fft neuroscience
 Description-Content-Type: text/markdown
@@ -26,14 +26,20 @@
 
 First install [muselsl](https://github.com/alexandrebarachant/muse-lsl), connect to your muse headset and start a muse stream using <br>
 
 ```
 muselsl stream
 ```
 
+Then install the realtime_tf package using
+
+```
+pip install real-time-tf
+```
+
 Keep the muselsl stream running and in a separate terminal run
 
 ```
 realtime_tf
 ```
 
 to visualize the realtime time frequency plot of the streamed eeg data from your muse headset.
```

### Comparing `real-time-tf-0.1.1/README.md` & `real-time-tf-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
 First install [muselsl](https://github.com/alexandrebarachant/muse-lsl), connect to your muse headset and start a muse stream using <br>
 
 ```
 muselsl stream
 ```
 
+Then install the realtime_tf package using
+
+```
+pip install real-time-tf
+```
+
 Keep the muselsl stream running and in a separate terminal run
 
 ```
 realtime_tf
 ```
 
 to visualize the realtime time frequency plot of the streamed eeg data from your muse headset.
```

### Comparing `real-time-tf-0.1.1/real_time_tf.egg-info/PKG-INFO` & `real-time-tf-0.1.2/real_time_tf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-time-tf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Real time time frequency plotting of EEG data from the Muse headset.
 Home-page: https://github.com/dxganta/real-time-tf
 Author: Diganta Kalita
 Author-email: digantakalita.ai@gmail.com
 License: BSD (3-clause)
 Keywords: muse time-frequency eeg fft neuroscience
 Description-Content-Type: text/markdown
@@ -26,14 +26,20 @@
 
 First install [muselsl](https://github.com/alexandrebarachant/muse-lsl), connect to your muse headset and start a muse stream using <br>
 
 ```
 muselsl stream
 ```
 
+Then install the realtime_tf package using
+
+```
+pip install real-time-tf
+```
+
 Keep the muselsl stream running and in a separate terminal run
 
 ```
 realtime_tf
 ```
 
 to visualize the realtime time frequency plot of the streamed eeg data from your muse headset.
```

### Comparing `real-time-tf-0.1.1/realtime_tf/realtime_tf.py` & `real-time-tf-0.1.2/realtime_tf/realtime_tf.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 
                 if counter < update_time_window * srate:
                     temp_data.popleft()
                     temp_data.append(sample)
                     counter += 1
                 else:
                     
-                    data = np.array(temp_data)[:,:4].T
+                    data = np.array(temp_data)[:,:len(channel_labels)].T
                     self.plot_data(data, cmwX, nKern, frex, show_time_window, channel, loops )
                     
                     counter = 0
                     loops += update_time_window
 
         except KeyboardInterrupt:
             print('Stopping data collection.')
@@ -81,15 +81,15 @@
     def _filter_channel(self, tf , channel):
         '''
             tf must be of shape channels x time
 
             returns tf array and title
         '''
         if channel != 'avg':
-            assert int(channel) < 4, 'Channel numbers range from 0 to 3. Please input a valid number'
+            assert int(channel) < len(channel_labels), f'Channel numbers range from 0 to {len(channel_labels)}. Please input a valid number'
         
         match channel:            
             case 'avg':
                 return np.mean(tf, axis=0), 'Average Power Spectrum over all channels'
             case _ :
                 return tf[int(channel), :], f'Power Spectrum across channel {channel_labels[int(channel)]}'
```

### Comparing `real-time-tf-0.1.1/realtime_tf/time_frequency.py` & `real-time-tf-0.1.2/realtime_tf/time_frequency.py`

 * *Files identical despite different names*

### Comparing `real-time-tf-0.1.1/setup.py` & `real-time-tf-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="real-time-tf",
-    version="0.1.1",
+    version="0.1.2",
     description="Real time time frequency plotting of EEG data from the Muse headset.",
     keywords="muse time-frequency eeg fft neuroscience",
     url="https://github.com/dxganta/real-time-tf",
     author="Diganta Kalita",
     author_email="digantakalita.ai@gmail.com",
     license="BSD (3-clause)",
     packages=find_packages(),
```

