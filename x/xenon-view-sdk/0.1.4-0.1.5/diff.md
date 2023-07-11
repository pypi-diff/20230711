# Comparing `tmp/xenon-view-sdk-0.1.4.tar.gz` & `tmp/xenon-view-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xenon-view-sdk-0.1.4.tar", last modified: Tue Feb 21 05:09:55 2023, max compression
+gzip compressed data, was "dist/xenon-view-sdk-0.1.5.tar", last modified: Tue Jul 11 06:28:18 2023, max compression
```

## Comparing `xenon-view-sdk-0.1.4.tar` & `xenon-view-sdk-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 05:09:55.000000 xenon-view-sdk-0.1.4/
--rw-r--r--   0 root         (0) root         (0)       24 2023-02-21 05:09:43.000000 xenon-view-sdk-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    41692 2023-02-21 05:09:55.000000 xenon-view-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    41019 2023-02-21 05:09:43.000000 xenon-view-sdk-0.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-21 05:09:55.000000 xenon-view-sdk-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1231 2023-02-21 05:09:43.000000 xenon-view-sdk-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 05:09:54.000000 xenon-view-sdk-0.1.4/xenon_view_sdk/
--rw-r--r--   0 root         (0) root         (0)    18811 2023-02-21 05:09:43.000000 xenon-view-sdk-0.1.4/xenon_view_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 05:09:55.000000 xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    41692 2023-02-21 05:09:54.000000 xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-02-21 05:09:54.000000 xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 05:09:54.000000 xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-21 05:09:54.000000 xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-21 05:09:54.000000 xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-11 06:28:08.000000 xenon-view-sdk-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    41725 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    41052 2023-07-11 06:28:08.000000 xenon-view-sdk-0.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-07-11 06:28:08.000000 xenon-view-sdk-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk/
+-rw-r--r--   0 root         (0) root         (0)    17885 2023-07-11 06:28:08.000000 xenon-view-sdk-0.1.5/xenon_view_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    41725 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 06:28:18.000000 xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/top_level.txt
```

### Comparing `xenon-view-sdk-0.1.4/PKG-INFO` & `xenon-view-sdk-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenon-view-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python access to Xenon View.
 Home-page: https://github.com/xenonview-com/view-python-sdk
 Maintainer: Luke Woydziak
 Maintainer-email: lwoydziak@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/xenonview-com/view-python-sdk/tarball/1.0
 Platform: any
@@ -53,14 +53,15 @@
     * [(Optional) Custom Customer Journey Milestones](#custom)
     * [(Optional) Journey Identification](#cuuid)
 * [License](#license)
 
 <br/>
 
 ## What's New <a id='whats-new'></a>
+* v0.1.5 - remove journeys call 
 * v0.1.4 - Rename tag to variant
 * v0.1.3 - Readme update
 * v0.1.2 - typo fixed
 * v0.1.1 - duplicates for new SDK handled
 * v0.1.0 - SDK redesign
 
 <br/>
```

### Comparing `xenon-view-sdk-0.1.4/README.md` & `xenon-view-sdk-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     * [(Optional) Custom Customer Journey Milestones](#custom)
     * [(Optional) Journey Identification](#cuuid)
 * [License](#license)
 
 <br/>
 
 ## What's New <a id='whats-new'></a>
+* v0.1.5 - remove journeys call 
 * v0.1.4 - Rename tag to variant
 * v0.1.3 - Readme update
 * v0.1.2 - typo fixed
 * v0.1.1 - duplicates for new SDK handled
 * v0.1.0 - SDK redesign
 
 <br/>
```

### Comparing `xenon-view-sdk-0.1.4/setup.py` & `xenon-view-sdk-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / 'README.md').read_text()
 
 setup(name='xenon-view-sdk',
-      version='0.1.4',
+      version='0.1.5',
       maintainer='Luke Woydziak',
       maintainer_email='lwoydziak@gmail.com',
       url='https://github.com/xenonview-com/view-python-sdk',
       download_url='https://github.com/xenonview-com/view-python-sdk/tarball/1.0',
       platforms=['any'],
       description='Python access to Xenon View.',
       long_description=README,
```

### Comparing `xenon-view-sdk-0.1.4/xenon_view_sdk/__init__.py` & `xenon-view-sdk-0.1.5/xenon_view_sdk/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = 'xenon_view_sdk'
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 __author__ = 'Xenon'
 __copyright__ = 'Copyright 2021 Xenon'
 '''
 Created on September 20, 2021
 @author: lwoydziak
 '''
 from datetime import datetime
@@ -547,39 +547,14 @@
     def duplicateMilestone(self, last, content, lastKeys, contentKeys):
         if content['category'] == 'Feature' or last['category'] == 'Feature': return False
         if content['category'] == 'Content' or last['category'] == 'Content': return False
         if content['name'] != last['name']: return False
         if content['details'] != last['details']: return False
         return True
 
-    def journeys(self, PostMethod=post, sleepTime=1, verify=True):
-        headers = {"Authorization": "Bearer " + self.__apiKey}
-        journeysApi = {
-            "name": "ApiJourneys",
-            "parameters": {"uuid": self.__id}
-        }
-        response = None
-        for _ in range(3):
-            try:
-                path = 'https://' + self.__apiUrl + "/journeys"
-                response = PostMethod(path, data=dumps(journeysApi), headers=headers, verify=verify)
-                break
-            except requests.exceptions.SSLError as exception:
-                sleep(sleepTime)
-                continue
-            except Exception as exception:
-                sleep(sleepTime)
-                continue
-
-        if not response or not int(response.status_code) == 200:
-            raise ApiException(response, "Api responded with error.")
-
-        jsonResponse = response.json()
-        return jsonResponse
-
     def journey(self):
         return self.__journey
 
     def storeJourney(self, journey):
         self.__journey = journey
 
     def reset(self):
```

### Comparing `xenon-view-sdk-0.1.4/xenon_view_sdk.egg-info/PKG-INFO` & `xenon-view-sdk-0.1.5/xenon_view_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenon-view-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python access to Xenon View.
 Home-page: https://github.com/xenonview-com/view-python-sdk
 Maintainer: Luke Woydziak
 Maintainer-email: lwoydziak@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/xenonview-com/view-python-sdk/tarball/1.0
 Platform: any
@@ -53,14 +53,15 @@
     * [(Optional) Custom Customer Journey Milestones](#custom)
     * [(Optional) Journey Identification](#cuuid)
 * [License](#license)
 
 <br/>
 
 ## What's New <a id='whats-new'></a>
+* v0.1.5 - remove journeys call 
 * v0.1.4 - Rename tag to variant
 * v0.1.3 - Readme update
 * v0.1.2 - typo fixed
 * v0.1.1 - duplicates for new SDK handled
 * v0.1.0 - SDK redesign
 
 <br/>
```

