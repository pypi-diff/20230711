# Comparing `tmp/q1pulse-0.8.7.tar.gz` & `tmp/q1pulse-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1pulse-0.8.7.tar", last modified: Fri Jun 30 12:43:52 2023, max compression
+gzip compressed data, was "dist\q1pulse-0.8.8.tar", last modified: Tue Jul 11 15:27:33 2023, max compression
```

## Comparing `q1pulse-0.8.7.tar` & `q1pulse-0.8.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/
--rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.7/LICENSE
--rw-rw-rw-   0        0        0      193 2023-06-30 12:43:52.000000 q1pulse-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/
--rw-rw-rw-   0        0        0      139 2023-06-30 12:43:30.000000 q1pulse-0.8.7/q1pulse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/assembler/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/assembler/__init__.py
--rw-rw-rw-   0        0        0    28695 2023-02-08 14:26:47.000000 q1pulse-0.8.7/q1pulse/assembler/generator.py
--rw-rw-rw-   0        0        0     1813 2021-12-15 13:49:20.000000 q1pulse-0.8.7/q1pulse/assembler/generator_data.py
--rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.7/q1pulse/assembler/instruction_queue.py
--rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.7/q1pulse/assembler/registers.py
--rw-rw-rw-   0        0        0    11312 2023-06-30 12:40:00.000000 q1pulse-0.8.7/q1pulse/instrument.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/lang/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/lang/__init__.py
--rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.7/q1pulse/lang/base.py
--rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.7/q1pulse/lang/exceptions.py
--rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.7/q1pulse/lang/expression.py
--rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.7/q1pulse/lang/flow_statements.py
--rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.7/q1pulse/lang/generator.py
--rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.7/q1pulse/lang/loops.py
--rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.7/q1pulse/lang/math_expressions.py
--rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.7/q1pulse/lang/register.py
--rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.7/q1pulse/lang/register_statements.py
--rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.7/q1pulse/lang/registers.py
--rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.7/q1pulse/lang/sequence.py
--rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.7/q1pulse/lang/simulator_statements.py
--rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.7/q1pulse/lang/timed_statements.py
--rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.7/q1pulse/lang/timeline.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/modules/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/modules/__init__.py
--rw-rw-rw-   0        0        0     8732 2023-06-30 11:37:00.000000 q1pulse-0.8.7/q1pulse/modules/modules.py
--rw-rw-rw-   0        0        0     2924 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/modules/sequencer_states.py
--rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.7/q1pulse/program.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/sequencer/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/sequencer/__init__.py
--rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.7/q1pulse/sequencer/builderbase.py
--rw-rw-rw-   0        0        0    14021 2023-06-30 11:37:00.000000 q1pulse-0.8.7/q1pulse/sequencer/control.py
--rw-rw-rw-   0        0        0     6224 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/sequencer/readout.py
--rw-rw-rw-   0        0        0     9429 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/sequencer/sequencer.py
--rw-rw-rw-   0        0        0     3389 2022-12-22 08:51:07.000000 q1pulse-0.8.7/q1pulse/sequencer/sequencer_data.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/util/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/util/__init__.py
--rw-rw-rw-   0        0        0      543 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/util/qblox_version.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/
--rw-rw-rw-   0        0        0      193 2023-06-30 12:43:51.000000 q1pulse-0.8.7/q1pulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:43:51.000000 q1pulse-0.8.7/q1pulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-06-30 12:43:52.000000 q1pulse-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-06-30 12:43:30.000000 q1pulse-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/
+-rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-07-11 15:27:33.000000 q1pulse-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/
+-rw-rw-rw-   0        0        0      139 2023-07-11 15:27:10.000000 q1pulse-0.8.8/q1pulse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/assembler/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/assembler/__init__.py
+-rw-rw-rw-   0        0        0    28695 2023-07-11 13:10:51.000000 q1pulse-0.8.8/q1pulse/assembler/generator.py
+-rw-rw-rw-   0        0        0     1813 2023-07-11 13:10:59.000000 q1pulse-0.8.8/q1pulse/assembler/generator_data.py
+-rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.8/q1pulse/assembler/instruction_queue.py
+-rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.8/q1pulse/assembler/registers.py
+-rw-rw-rw-   0        0        0    11312 2023-06-30 12:58:43.000000 q1pulse-0.8.8/q1pulse/instrument.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/lang/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/lang/__init__.py
+-rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.8/q1pulse/lang/base.py
+-rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.8/q1pulse/lang/exceptions.py
+-rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.8/q1pulse/lang/expression.py
+-rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.8/q1pulse/lang/flow_statements.py
+-rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.8/q1pulse/lang/generator.py
+-rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.8/q1pulse/lang/loops.py
+-rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.8/q1pulse/lang/math_expressions.py
+-rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.8/q1pulse/lang/register.py
+-rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.8/q1pulse/lang/register_statements.py
+-rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.8/q1pulse/lang/registers.py
+-rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.8/q1pulse/lang/sequence.py
+-rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.8/q1pulse/lang/simulator_statements.py
+-rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.8/q1pulse/lang/timed_statements.py
+-rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.8/q1pulse/lang/timeline.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/modules/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/modules/__init__.py
+-rw-rw-rw-   0        0        0     8732 2023-06-30 11:37:00.000000 q1pulse-0.8.8/q1pulse/modules/modules.py
+-rw-rw-rw-   0        0        0     2924 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/modules/sequencer_states.py
+-rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.8/q1pulse/program.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/sequencer/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/sequencer/__init__.py
+-rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.8/q1pulse/sequencer/builderbase.py
+-rw-rw-rw-   0        0        0    14021 2023-06-30 11:37:00.000000 q1pulse-0.8.8/q1pulse/sequencer/control.py
+-rw-rw-rw-   0        0        0     6224 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/sequencer/readout.py
+-rw-rw-rw-   0        0        0     9429 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/sequencer/sequencer.py
+-rw-rw-rw-   0        0        0     3395 2023-07-11 13:19:38.000000 q1pulse-0.8.8/q1pulse/sequencer/sequencer_data.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/util/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/util/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/util/qblox_version.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-11 15:27:33.000000 q1pulse-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      310 2023-07-11 15:27:10.000000 q1pulse-0.8.8/setup.py
```

### Comparing `q1pulse-0.8.7/LICENSE` & `q1pulse-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/README.md` & `q1pulse-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/assembler/generator.py` & `q1pulse-0.8.8/q1pulse/assembler/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/assembler/generator_data.py` & `q1pulse-0.8.8/q1pulse/assembler/generator_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/assembler/instruction_queue.py` & `q1pulse-0.8.8/q1pulse/assembler/instruction_queue.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/assembler/registers.py` & `q1pulse-0.8.8/q1pulse/assembler/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/instrument.py` & `q1pulse-0.8.8/q1pulse/instrument.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/exceptions.py` & `q1pulse-0.8.8/q1pulse/lang/exceptions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/flow_statements.py` & `q1pulse-0.8.8/q1pulse/lang/flow_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/generator.py` & `q1pulse-0.8.8/q1pulse/lang/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/loops.py` & `q1pulse-0.8.8/q1pulse/lang/loops.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/math_expressions.py` & `q1pulse-0.8.8/q1pulse/lang/math_expressions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/register.py` & `q1pulse-0.8.8/q1pulse/lang/register.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/register_statements.py` & `q1pulse-0.8.8/q1pulse/lang/register_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/registers.py` & `q1pulse-0.8.8/q1pulse/lang/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/sequence.py` & `q1pulse-0.8.8/q1pulse/lang/sequence.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/simulator_statements.py` & `q1pulse-0.8.8/q1pulse/lang/simulator_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/timed_statements.py` & `q1pulse-0.8.8/q1pulse/lang/timed_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/lang/timeline.py` & `q1pulse-0.8.8/q1pulse/lang/timeline.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/modules/modules.py` & `q1pulse-0.8.8/q1pulse/modules/modules.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/modules/sequencer_states.py` & `q1pulse-0.8.8/q1pulse/modules/sequencer_states.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/program.py` & `q1pulse-0.8.8/q1pulse/program.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/sequencer/control.py` & `q1pulse-0.8.8/q1pulse/sequencer/control.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/sequencer/readout.py` & `q1pulse-0.8.8/q1pulse/sequencer/readout.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/sequencer/sequencer.py` & `q1pulse-0.8.8/q1pulse/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse/sequencer/sequencer_data.py` & `q1pulse-0.8.8/q1pulse/sequencer/sequencer_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,17 @@
             raise Q1NameError(f'Wave {name} already defined')
         wave = Wave(name, data)
         self._waves[name] = wave
         return wave
 
     def get_ramp(self, n_samples, start=0.0, stop=1.0):
         if start == 0.0 and stop == 1.0:
-            name = f'_ramp({n_samples})'
+            name = f'_ramp_{n_samples}'
         else:
-            name = f'_ramp({n_samples}, {start:5.3f}, {stop:5.3f})'
+            name = f'_ramp_{n_samples}_{start*1e5:.0f}_{stop*1e5:.0f}'
 
         try:
             return self._waves[name]
         except:
             data = np.linspace(start, stop, n_samples, endpoint=False)
             wave = self.add_wave(name, data)
             return wave
@@ -46,16 +46,16 @@
         # dp/ns = 0, 1, 2, 3, 4, ...
         # phase = 0, 1, 3, 6, 10, ...
         # phase expressed in rotations!
         dp_ns_end = f_end / 1e9
         dp = np.linspace(0, dp_ns_end, n_samples, endpoint=False)
         phase = np.cumsum(dp)
         dp_next = (phase[-1] + dp_ns_end) * 2
-        nameI = f'_chirp({n_samples}, {f_end}).real'
-        nameQ = f'_chirp({n_samples}, {f_end}).imag'
+        nameI = f'_chirp_{n_samples}_{f_end:.0f}_real'
+        nameQ = f'_chirp_{n_samples}_{f_end:.0f}_imag'
         try:
             return self._waves[nameI], self._waves[nameQ], dp_next
         except:
             waveI = self.add_wave(nameI, np.cos(2*np.pi*phase))
             waveQ = self.add_wave(nameQ, np.sin(2*np.pi*phase))
             # phase shift for next chirp, expressed in pi*rad!
             return waveI, waveQ, dp_next
```

### Comparing `q1pulse-0.8.7/q1pulse/util/qblox_version.py` & `q1pulse-0.8.8/q1pulse/util/qblox_version.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.7/q1pulse.egg-info/SOURCES.txt` & `q1pulse-0.8.8/q1pulse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

