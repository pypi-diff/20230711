# Comparing `tmp/exem-logs-1.1.3.tar.gz` & `tmp/exem-logs-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exem-logs-1.1.3.tar", last modified: Fri Jun 23 12:14:06 2023, max compression
+gzip compressed data, was "exem-logs-1.1.4.tar", last modified: Tue Jul 11 08:04:49 2023, max compression
```

## Comparing `exem-logs-1.1.3.tar` & `exem-logs-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 12:14:06.530616 exem-logs-1.1.3/
--rw-rw-rw-   0        0        0     5467 2023-06-23 10:28:22.000000 exem-logs-1.1.3/Log.py
--rw-rw-rw-   0        0        0     1765 2023-06-23 12:14:06.530616 exem-logs-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1362 2023-06-23 09:32:24.000000 exem-logs-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 12:14:06.483233 exem-logs-1.1.3/exem_logs.egg-info/
--rw-rw-rw-   0        0        0     1765 2023-06-23 12:14:06.000000 exem-logs-1.1.3/exem_logs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2023-06-23 12:14:06.000000 exem-logs-1.1.3/exem_logs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 12:14:06.000000 exem-logs-1.1.3/exem_logs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-23 12:14:06.000000 exem-logs-1.1.3/exem_logs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-23 12:14:06.000000 exem-logs-1.1.3/exem_logs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 12:14:06.530616 exem-logs-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      731 2023-06-23 12:13:24.000000 exem-logs-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:14:06.467612 exem-logs-1.1.3/venv10/
-drwxrwxrwx   0        0        0        0 2023-06-23 12:14:06.514501 exem-logs-1.1.3/venv10/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-06-23 07:53:35.000000 exem-logs-1.1.3/venv10/Scripts/activate_this.py
--rw-rw-rw-   0        0        0     6456 2023-06-23 08:01:20.000000 exem-logs-1.1.3/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py
--rw-rw-rw-   0        0        0      664 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2html.py
--rw-rw-rw-   0        0        0      786 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2html4.py
--rw-rw-rw-   0        0        0     1121 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2html5.py
--rw-rw-rw-   0        0        0      863 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2latex.py
--rw-rw-rw-   0        0        0      686 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2man.py
--rw-rw-rw-   0        0        0      852 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2odt.py
--rw-rw-rw-   0        0        0      658 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2odt_prepstyles.py
--rw-rw-rw-   0        0        0      671 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2pseudoxml.py
--rw-rw-rw-   0        0        0      707 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2s5.py
--rw-rw-rw-   0        0        0      943 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2xetex.py
--rw-rw-rw-   0        0        0      672 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rst2xml.py
--rw-rw-rw-   0        0        0      740 2023-06-23 07:54:36.000000 exem-logs-1.1.3/venv10/Scripts/rstpep2html.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:04:49.104111 exem-logs-1.1.4/
+-rw-rw-rw-   0        0        0     5581 2023-07-11 08:01:33.000000 exem-logs-1.1.4/Log.py
+-rw-rw-rw-   0        0        0     1765 2023-07-11 08:04:49.104111 exem-logs-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2023-06-23 09:32:24.000000 exem-logs-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:04:49.071542 exem-logs-1.1.4/exem_logs.egg-info/
+-rw-rw-rw-   0        0        0     1765 2023-07-11 08:04:49.000000 exem-logs-1.1.4/exem_logs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-07-11 08:04:49.000000 exem-logs-1.1.4/exem_logs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:04:49.000000 exem-logs-1.1.4/exem_logs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-11 08:04:49.000000 exem-logs-1.1.4/exem_logs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 08:04:49.000000 exem-logs-1.1.4/exem_logs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:04:49.104111 exem-logs-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      731 2023-07-11 08:04:22.000000 exem-logs-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:04:49.055903 exem-logs-1.1.4/venv10/
+drwxrwxrwx   0        0        0        0 2023-07-11 08:04:49.104111 exem-logs-1.1.4/venv10/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-06-23 07:53:35.000000 exem-logs-1.1.4/venv10/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0     6456 2023-06-23 08:01:20.000000 exem-logs-1.1.4/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py
+-rw-rw-rw-   0        0        0      664 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2html.py
+-rw-rw-rw-   0        0        0      786 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2html4.py
+-rw-rw-rw-   0        0        0     1121 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2html5.py
+-rw-rw-rw-   0        0        0      863 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2latex.py
+-rw-rw-rw-   0        0        0      686 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2man.py
+-rw-rw-rw-   0        0        0      852 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2odt.py
+-rw-rw-rw-   0        0        0      658 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2odt_prepstyles.py
+-rw-rw-rw-   0        0        0      671 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2pseudoxml.py
+-rw-rw-rw-   0        0        0      707 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2s5.py
+-rw-rw-rw-   0        0        0      943 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2xetex.py
+-rw-rw-rw-   0        0        0      672 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rst2xml.py
+-rw-rw-rw-   0        0        0      740 2023-06-23 07:54:36.000000 exem-logs-1.1.4/venv10/Scripts/rstpep2html.py
```

### Comparing `exem-logs-1.1.3/Log.py` & `exem-logs-1.1.4/Log.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import shutil
 import sys
 from datetime import datetime
 import logging
 import os
 import traceback
 import zipfile
+from os.path import join, abspath, isdir, exists, basename, splitext
 from pathlib import Path
 
 from google.oauth2.service_account import Credentials
 
 """
 To install libraries:
     pip install -r requirements.txt
@@ -49,28 +50,28 @@
             if level == Log.Level.WARNING:
                 return logging.WARNING
             return logging.NOTSET
 
     def __init__(self, log_name=None):
         self.log_name = log_name
 
+        self._generate_log_name()
         self._create_dirs()
         self._archive()
-        self._generate_log_name()
 
         self.handler = logging.FileHandler(filename=os.path.join(self.log_dir, "any.log"), encoding='utf-8', mode='a+')
         logging.basicConfig(
             handlers=[
                 self.handler
             ],
             format="%(asctime)s %(levelname)s: %(message)s",
             datefmt="%F %T",
             level=logging.NOTSET
         )
-        self.logger = logging.getLogger(log_name)
+        self.logger = logging.getLogger(self.log_name)
 
         self.cloud_project_id = None
 
     def verbose(self, text, level):
         if level == self.Level.ERROR:
             text = f"{text}\n{traceback.format_exc()}"
         self.logger.log(self.Level.logger(level), text)
@@ -107,61 +108,63 @@
             )
         else:
             client = google.cloud.logging.Client(project=self.cloud_project_id)
         setup_logging(self.handler)
         setup_logging(CloudLoggingHandler(client, resource=_resource))
 
     def _generate_log_name(self):
-        _scripts = inspect.stack()
-        _file_path = None
-        for _script in _scripts:
-            if _script.filename != __file__:
-                _file_path = _script.filename
-                break
-        if _file_path:
-            _filename_match = re.search(r"([^\\]+)\.py", _file_path)
-            if _filename_match.lastindex > 0:
-                self.log_name = _filename_match.group(_filename_match.lastindex)
-        if not self.log_name:
-            self.log_name = sys.argv[0]
-        return self.log_name
+        try:
+            if not self.log_name:
+                frame = inspect.stack()[1]
+                module = inspect.getmodule(frame[0])
+                self.log_name = module.__file__
+                if not self.log_name:
+                    self.log_name = sys.argv[0]
+                self.log_name = splitext(basename(self.log_name))[0]
+        except Exception as e:
+            print(f"Error while generating log name: {e}")
 
     def _create_dirs(self):
         self.date = datetime.now().strftime(self._LOG_FILE_DATE_FORMAT)
 
         self.logs_dir = self._LOGS_FOLER
-        self.log_dir = os.path.abspath(os.path.join(self.logs_dir, self.date))
-
-        os.umask(0)
-        os.makedirs(self.log_dir, exist_ok=True)
+        self.log_dir = abspath(join(self.logs_dir, self.date))
+        try:
+            os.umask(0)
+            os.makedirs(self.log_dir, exist_ok=True)
+        except OSError as e:
+            print(f"Error while creating {self.log_dir}: {e}")
 
-        self.log_file = os.path.join(self.log_dir, f"{self.log_name}.log")
+        self.log_file = join(self.log_dir, f"{self.log_name}.log")
 
         print(f"{self.log_name} logs can be found in {self.log_dir}")
 
     def _save_file(self, log, level):
+        print(self.log_file)
+        print(self.log_dir)
+        print(self.log_name)
         with open(self.log_file, "a+") as f:
             at = self._log_date()
             f.write(f"{at[:-3]} {level}: {log}\n")
 
     def _log_date(self):
         return datetime.now().strftime(self._LOG_FILE_DATE_FORMAT)
 
     def _archive(self):
         today = self._log_date()
         current_year = today[:4]
         log_directories = [
-            os.path.join(self._LOGS_FOLER, directory)
+            join(self._LOGS_FOLER, directory)
             for directory in os.listdir(self._LOGS_FOLER)
-            if os.path.isdir(os.path.join(self._LOGS_FOLER, directory))
+            if isdir(os.path.join(self._LOGS_FOLER, directory))
             and directory != today
         ]
 
-        zip_path = os.path.join(self._LOGS_FOLER, current_year + ".zip")
-        zip_mode = "a" if os.path.exists(zip_path) else "w"
+        zip_path = join(self._LOGS_FOLER, current_year + ".zip")
+        zip_mode = "a" if exists(zip_path) else "w"
         with zipfile.ZipFile(zip_path, zip_mode, zipfile.ZIP_DEFLATED) as zip_file:
             for log_directory in log_directories:
                 for file in os.listdir(log_directory):
                     if file.endswith(".log"):
-                        file_path = os.path.join(log_directory, file)
-                        zip_file.write(file_path, arcname=os.path.join(os.path.basename(log_directory), file))
+                        file_path = join(log_directory, file)
+                        zip_file.write(file_path, arcname=join(os.path.basename(log_directory), file))
                 shutil.rmtree(log_directory)
```

### Comparing `exem-logs-1.1.3/PKG-INFO` & `exem-logs-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exem-logs
-Version: 1.1.3
+Version: 1.1.4
 Summary: Powerfull but simplest way to log your python application.
 Home-page: https://gitlab.com/exem2/libraries/logs
 Author: Félix BOULE--REIFF
 Author-email: boulereiff@exem.fr
 License: BSD 2-clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `exem-logs-1.1.3/README.md` & `exem-logs-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/exem_logs.egg-info/PKG-INFO` & `exem-logs-1.1.4/exem_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exem-logs
-Version: 1.1.3
+Version: 1.1.4
 Summary: Powerfull but simplest way to log your python application.
 Home-page: https://gitlab.com/exem2/libraries/logs
 Author: Félix BOULE--REIFF
 Author-email: boulereiff@exem.fr
 License: BSD 2-clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `exem-logs-1.1.3/exem_logs.egg-info/SOURCES.txt` & `exem-logs-1.1.4/exem_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/setup.py` & `exem-logs-1.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='exem-logs',
-    version='1.1.3',
+    version='1.1.4',
     description='Powerfull but simplest way to log your python application.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/exem2/libraries/logs',
     author='Félix BOULE--REIFF',
     author_email='boulereiff@exem.fr',
     license='BSD 2-clause',
```

### Comparing `exem-logs-1.1.3/venv10/Scripts/activate_this.py` & `exem-logs-1.1.4/venv10/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py` & `exem-logs-1.1.4/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2html.py` & `exem-logs-1.1.4/venv10/Scripts/rst2html.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2html4.py` & `exem-logs-1.1.4/venv10/Scripts/rst2html4.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2html5.py` & `exem-logs-1.1.4/venv10/Scripts/rst2html5.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2latex.py` & `exem-logs-1.1.4/venv10/Scripts/rst2latex.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2man.py` & `exem-logs-1.1.4/venv10/Scripts/rst2man.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2odt.py` & `exem-logs-1.1.4/venv10/Scripts/rst2odt.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2odt_prepstyles.py` & `exem-logs-1.1.4/venv10/Scripts/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2pseudoxml.py` & `exem-logs-1.1.4/venv10/Scripts/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2s5.py` & `exem-logs-1.1.4/venv10/Scripts/rst2s5.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2xetex.py` & `exem-logs-1.1.4/venv10/Scripts/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rst2xml.py` & `exem-logs-1.1.4/venv10/Scripts/rst2xml.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.3/venv10/Scripts/rstpep2html.py` & `exem-logs-1.1.4/venv10/Scripts/rstpep2html.py`

 * *Files identical despite different names*

