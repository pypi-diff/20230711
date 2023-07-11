# Comparing `tmp/exem-logs-1.1.5.tar.gz` & `tmp/exem-logs-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exem-logs-1.1.5.tar", last modified: Tue Jul 11 08:17:20 2023, max compression
+gzip compressed data, was "exem-logs-1.1.6.tar", last modified: Tue Jul 11 09:05:54 2023, max compression
```

## Comparing `exem-logs-1.1.5.tar` & `exem-logs-1.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:17:20.535265 exem-logs-1.1.5/
--rw-rw-rw-   0        0        0     5581 2023-07-11 08:01:33.000000 exem-logs-1.1.5/Log.py
--rw-rw-rw-   0        0        0     1947 2023-07-11 08:17:20.531729 exem-logs-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1544 2023-07-11 08:11:18.000000 exem-logs-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 08:17:20.498867 exem-logs-1.1.5/exem_logs.egg-info/
--rw-rw-rw-   0        0        0     1947 2023-07-11 08:17:20.000000 exem-logs-1.1.5/exem_logs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2023-07-11 08:17:20.000000 exem-logs-1.1.5/exem_logs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:17:20.000000 exem-logs-1.1.5/exem_logs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-11 08:17:20.000000 exem-logs-1.1.5/exem_logs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 08:17:20.000000 exem-logs-1.1.5/exem_logs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 08:17:20.535265 exem-logs-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      731 2023-07-11 08:11:25.000000 exem-logs-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:17:20.483219 exem-logs-1.1.5/venv10/
-drwxrwxrwx   0        0        0        0 2023-07-11 08:17:20.531729 exem-logs-1.1.5/venv10/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-06-23 07:53:35.000000 exem-logs-1.1.5/venv10/Scripts/activate_this.py
--rw-rw-rw-   0        0        0     6456 2023-06-23 08:01:20.000000 exem-logs-1.1.5/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py
--rw-rw-rw-   0        0        0      664 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2html.py
--rw-rw-rw-   0        0        0      786 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2html4.py
--rw-rw-rw-   0        0        0     1121 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2html5.py
--rw-rw-rw-   0        0        0      863 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2latex.py
--rw-rw-rw-   0        0        0      686 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2man.py
--rw-rw-rw-   0        0        0      852 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2odt.py
--rw-rw-rw-   0        0        0      658 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2odt_prepstyles.py
--rw-rw-rw-   0        0        0      671 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2pseudoxml.py
--rw-rw-rw-   0        0        0      707 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2s5.py
--rw-rw-rw-   0        0        0      943 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2xetex.py
--rw-rw-rw-   0        0        0      672 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rst2xml.py
--rw-rw-rw-   0        0        0      740 2023-06-23 07:54:36.000000 exem-logs-1.1.5/venv10/Scripts/rstpep2html.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:54.342861 exem-logs-1.1.6/
+-rw-rw-rw-   0        0        0     5492 2023-07-11 09:05:09.000000 exem-logs-1.1.6/Log.py
+-rw-rw-rw-   0        0        0     1947 2023-07-11 09:05:54.341875 exem-logs-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1544 2023-07-11 08:11:18.000000 exem-logs-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:54.312200 exem-logs-1.1.6/exem_logs.egg-info/
+-rw-rw-rw-   0        0        0     1947 2023-07-11 09:05:54.000000 exem-logs-1.1.6/exem_logs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-07-11 09:05:54.000000 exem-logs-1.1.6/exem_logs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:05:54.000000 exem-logs-1.1.6/exem_logs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-11 09:05:54.000000 exem-logs-1.1.6/exem_logs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 09:05:54.000000 exem-logs-1.1.6/exem_logs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:05:54.343862 exem-logs-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      731 2023-07-11 09:05:09.000000 exem-logs-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:54.295489 exem-logs-1.1.6/venv10/
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:54.339859 exem-logs-1.1.6/venv10/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-06-23 07:53:35.000000 exem-logs-1.1.6/venv10/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0     6456 2023-06-23 08:01:20.000000 exem-logs-1.1.6/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py
+-rw-rw-rw-   0        0        0      664 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2html.py
+-rw-rw-rw-   0        0        0      786 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2html4.py
+-rw-rw-rw-   0        0        0     1121 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2html5.py
+-rw-rw-rw-   0        0        0      863 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2latex.py
+-rw-rw-rw-   0        0        0      686 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2man.py
+-rw-rw-rw-   0        0        0      852 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2odt.py
+-rw-rw-rw-   0        0        0      658 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2odt_prepstyles.py
+-rw-rw-rw-   0        0        0      671 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2pseudoxml.py
+-rw-rw-rw-   0        0        0      707 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2s5.py
+-rw-rw-rw-   0        0        0      943 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2xetex.py
+-rw-rw-rw-   0        0        0      672 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rst2xml.py
+-rw-rw-rw-   0        0        0      740 2023-06-23 07:54:36.000000 exem-logs-1.1.6/venv10/Scripts/rstpep2html.py
```

### Comparing `exem-logs-1.1.5/Log.py` & `exem-logs-1.1.6/Log.py`

 * *Files 7% similar despite different names*

```diff
@@ -135,17 +135,14 @@
             print(f"Error while creating {self.log_dir}: {e}")
 
         self.log_file = join(self.log_dir, f"{self.log_name}.log")
 
         print(f"{self.log_name} logs can be found in {self.log_dir}")
 
     def _save_file(self, log, level):
-        print(self.log_file)
-        print(self.log_dir)
-        print(self.log_name)
         with open(self.log_file, "a+") as f:
             at = self._log_date()
             f.write(f"{at[:-3]} {level}: {log}\n")
 
     def _log_date(self):
         return datetime.now().strftime(self._LOG_FILE_DATE_FORMAT)
```

### Comparing `exem-logs-1.1.5/PKG-INFO` & `exem-logs-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exem-logs
-Version: 1.1.5
+Version: 1.1.6
 Summary: Powerfull but simplest way to log your python application.
 Home-page: https://gitlab.com/exem2/libraries/logs
 Author: Félix BOULE--REIFF
 Author-email: boulereiff@exem.fr
 License: BSD 2-clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `exem-logs-1.1.5/README.md` & `exem-logs-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/exem_logs.egg-info/PKG-INFO` & `exem-logs-1.1.6/exem_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exem-logs
-Version: 1.1.5
+Version: 1.1.6
 Summary: Powerfull but simplest way to log your python application.
 Home-page: https://gitlab.com/exem2/libraries/logs
 Author: Félix BOULE--REIFF
 Author-email: boulereiff@exem.fr
 License: BSD 2-clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `exem-logs-1.1.5/exem_logs.egg-info/SOURCES.txt` & `exem-logs-1.1.6/exem_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/setup.py` & `exem-logs-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='exem-logs',
-    version='1.1.5',
+    version='1.1.6',
     description='Powerfull but simplest way to log your python application.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/exem2/libraries/logs',
     author='Félix BOULE--REIFF',
     author_email='boulereiff@exem.fr',
     license='BSD 2-clause',
```

### Comparing `exem-logs-1.1.5/venv10/Scripts/activate_this.py` & `exem-logs-1.1.6/venv10/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py` & `exem-logs-1.1.6/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2html.py` & `exem-logs-1.1.6/venv10/Scripts/rst2html.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2html4.py` & `exem-logs-1.1.6/venv10/Scripts/rst2html4.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2html5.py` & `exem-logs-1.1.6/venv10/Scripts/rst2html5.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2latex.py` & `exem-logs-1.1.6/venv10/Scripts/rst2latex.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2man.py` & `exem-logs-1.1.6/venv10/Scripts/rst2man.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2odt.py` & `exem-logs-1.1.6/venv10/Scripts/rst2odt.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2odt_prepstyles.py` & `exem-logs-1.1.6/venv10/Scripts/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2pseudoxml.py` & `exem-logs-1.1.6/venv10/Scripts/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2s5.py` & `exem-logs-1.1.6/venv10/Scripts/rst2s5.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2xetex.py` & `exem-logs-1.1.6/venv10/Scripts/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rst2xml.py` & `exem-logs-1.1.6/venv10/Scripts/rst2xml.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.5/venv10/Scripts/rstpep2html.py` & `exem-logs-1.1.6/venv10/Scripts/rstpep2html.py`

 * *Files identical despite different names*

