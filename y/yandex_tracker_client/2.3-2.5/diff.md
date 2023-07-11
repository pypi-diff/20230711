# Comparing `tmp/yandex_tracker_client-2.3.tar.gz` & `tmp/yandex_tracker_client-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandex_tracker_client-2.3.tar", last modified: Mon Apr  4 08:44:11 2022, max compression
+gzip compressed data, was "dist/yandex_tracker_client-2.5.tar", last modified: Tue Jul 11 11:47:08 2023, max compression
```

## Comparing `yandex_tracker_client-2.3.tar` & `yandex_tracker_client-2.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client/
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       80 2021-09-28 20:00:15.000000 yandex_tracker_client-2.3/yandex_tracker_client/__init__.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     2394 2022-03-18 09:14:51.000000 yandex_tracker_client-2.3/yandex_tracker_client/client.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)    35987 2022-04-04 08:41:54.000000 yandex_tracker_client-2.3/yandex_tracker_client/collections.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7458 2021-09-28 20:00:15.000000 yandex_tracker_client-2.3/yandex_tracker_client/connection.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     3337 2021-09-28 20:00:15.000000 yandex_tracker_client-2.3/yandex_tracker_client/exceptions.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7424 2021-09-28 20:00:15.000000 yandex_tracker_client-2.3/yandex_tracker_client/objects.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       93 2021-09-28 20:00:15.000000 yandex_tracker_client-2.3/yandex_tracker_client/settings.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1096 2021-09-28 20:00:15.000000 yandex_tracker_client-2.3/yandex_tracker_client/uriutils.py
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client.egg-info/
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client.egg-info/PKG-INFO
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      519 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client.egg-info/SOURCES.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)        1 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client.egg-info/dependency_links.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       52 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client.egg-info/requires.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       22 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/yandex_tracker_client.egg-info/top_level.txt
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     8810 2021-09-28 19:59:59.000000 yandex_tracker_client-2.3/README.rst
--rwxrwxr-x   0 smosker  (346405873) LD\Domain Users (593637566)     1495 2022-04-04 08:44:07.000000 yandex_tracker_client-2.3/setup.py
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/PKG-INFO
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       38 2022-04-04 08:44:11.000000 yandex_tracker_client-2.3/setup.cfg
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client/
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       80 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/__init__.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     2394 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/client.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)    37008 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/collections.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7744 2023-07-11 09:41:20.000000 yandex_tracker_client-2.5/yandex_tracker_client/connection.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     3337 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/exceptions.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7480 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/objects.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       93 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/settings.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1096 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/yandex_tracker_client/uriutils.py
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/PKG-INFO
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      535 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/SOURCES.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)        1 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/dependency_links.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       52 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/requires.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       22 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/yandex_tracker_client.egg-info/top_level.txt
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)      180 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/AUTHORS
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1607 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/LICENSE
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     8808 2023-04-28 20:02:24.000000 yandex_tracker_client-2.5/README.rst
+-rwxrwxr-x   0 smosker  (346405873) LD\Domain Users (593637566)     1520 2023-07-11 11:28:09.000000 yandex_tracker_client-2.5/setup.py
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/PKG-INFO
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       38 2023-07-11 11:47:08.000000 yandex_tracker_client-2.5/setup.cfg
```

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client/client.py` & `yandex_tracker_client-2.5/yandex_tracker_client/client.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client/collections.py` & `yandex_tracker_client-2.5/yandex_tracker_client/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,17 @@
     def path(self):
         pass
 
     @abc.abstractproperty
     def fields(self):
         pass
 
+    @property
+    def local_fields(self):
+        return self._local_fields_map
 
     def _parse_value(self, value):
         if self.has_local_fields:
             local_fields_to_add = {}
             for field, field_value in six.iteritems(value):
                 if '--' in field:
                     local_field_key = field.split('--')[-1]
@@ -483,14 +486,15 @@
         language,
         embed,
         localized,
         notifyAuthor
     """
     path = '/{api_version}/issues/{id}'
     search_path = '/{api_version}/issues/_search'
+    count_search_path = '/{api_version}/issues/_count'
     import_path = '/{api_version}/issues/_import'
     unique_path = '/{api_version}/issues/_findByUnique'
     has_local_fields = True
     date_format = '%Y-%m-%dT%H:%M:%S.%f%z'
 
     _fields = None
 
@@ -540,15 +544,16 @@
             kwargs['unique'] = uuid.uuid4().hex
 
     @injected_method
     def update(self, obj, params=None, **kwargs):
         _upload_attachments(self, kwargs)
         return super(Issues, self).update(obj, params=params, **kwargs)
 
-    def find(self, query=None, per_page=None, keys=None, filter=None, filter_id=None, order=None, **kwargs):
+    def find(self, query=None, per_page=None, keys=None, filter=None, filter_id=None, order=None,
+             count_only=False, **kwargs):
         """
         Parameters 'orderBy' and 'orderAsc' are deprecated in this method.
         Instead use the parameter 'order' in the form of the fields list
         like in Django: ['field1', '-field2', '+field3']
         """
         data = {
             'filter': filter,
@@ -558,17 +563,18 @@
             'queue': kwargs.pop('queue', None),
             'order': self._parse_order_params(
                 kwargs.pop('orderBy', None),
                 kwargs.pop('orderAsc', True),
                 order or [],
             ),
         }
+        path = self.count_search_path if count_only else self.search_path
         return self._execute_request(
             self._connection.post,
-            path=self.search_path,
+            path=path,
             params=dict(kwargs, perPage=per_page),
             data=data,
         )
 
     @injected_method
     def add_remotelink(self, issue, relation, target_url):
         return self._connection.link(
@@ -749,21 +755,35 @@
     @injected_property
     def macros(self, queue):
         return self._execute_request(
             self._connection.get,
             path=queue._path + '/macros',
         )
 
+    @injected_property
+    def workflows(self, queue):
+        return self._execute_request(
+            self._connection.get,
+            path=queue._path + '/workflows',
+        )
+
     @injected_method
     def check_permissions(self, queue, permission_code):
         return self._execute_request(
             self._connection.get,
             path=queue._path + '/checkPermissions/{}'.format(permission_code),
         )
 
+    @injected_property
+    def local_fields(self, queue):
+        return self._execute_request(
+            self._connection.get,
+            path=queue._path + '/localFields',
+        )
+
 
 class QueueDefaultValues(Collection):
     """Extra get params = localized"""
     path = '/{api_version}/queues/{queue}/defaultValues/{id}'
     fields = {
         'id': None,
         'self': None,
@@ -841,14 +861,15 @@
         'attachments': [],
         'createdBy': None,
         'createdAt': None,
         'updatedBy': None,
         'updatedAt': None,
         'summonees': [],
         'email': None,
+        'reactionsCount': None,
     }
     _priority = 1
 
     def create(self, params=None, **kwargs):
         _upload_attachments(self, kwargs)
         return super(IssueComments, self).create(params=params, **kwargs)
 
@@ -936,15 +957,15 @@
         else:
             filename = getattr(file, 'name', None)
 
         if not filename:
             return DEFAULT_FILENAME
 
         try:
-            filename.encode('ascii')
+            filename.encode('utf-8')
         except UnicodeEncodeError:
             return DEFAULT_FILENAME
 
         return filename.rsplit('/', 1)[-1]
 
     @injected_method
     def read(self, attachment):
@@ -1071,14 +1092,15 @@
         'self': None,
         'name': None,
         'description': None,
         'schema': None,
         'readonly': None,
         'options': None,
         'suggest': None,
+        'optionsProvider': None,
     }
 
 
 class Sprints(Collection):
     path = '/{api_version}/sprints/{id}'
     fields = {
         'id': None,
@@ -1359,7 +1381,24 @@
             text=text,
             checked=checked,
             assignee=assignee,
             deadline=deadline,
             url=url,
             checklistItemType=item_type
         )
+
+
+class LocalFields(Collection):
+    path = '/{api_version}/localFields/{id}'
+    fields = {
+        'id': None,
+        'self': None,
+        'name': None,
+        'key': None,
+        'version': None,
+        'schema': None,
+        'category': None,
+        'readonly': None,
+        'options': None,
+        'suggest': None,
+        'queue': None
+    }
```

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client/connection.py` & `yandex_tracker_client-2.5/yandex_tracker_client/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,33 +29,39 @@
     return method
 
 
 class Connection(object):
 
     def __init__(self,
                  token,
-                 org_id,
+                 org_id=None,
                  base_url="https://api.tracker.yandex.net",
                  timeout=10,
                  retries=10,
                  headers=None,
                  api_version=VERSION_V2,
                  verify=True,
+                 cloud_org_id=None,
                  ):
 
         self.session = requests.Session()
         self.session.verify = verify
 
         if headers is not None:
             self.session.headers.update(headers)
 
         self.session.headers['Authorization'] = 'OAuth ' + (token or 'not provided')
         self.session.headers['X-Org-Id'] = org_id or 'not provided'
         self.session.headers['Content-Type'] = 'application/json'
 
+        if cloud_org_id:
+            if cloud_org_id and org_id:
+                raise exceptions.TrackerClientError("Use either org_id or cloud_org_id to specify organization")
+            self.session.headers['X-Cloud-Org-Id'] = cloud_org_id
+
         # Check validity headers for requests >= 2.11
         for header in self.session.headers.items():
             check_header_validity(header)
 
         self.base_url = base_url
         self.api_version = api_version
         self.timeout = timeout
```

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client/exceptions.py` & `yandex_tracker_client-2.5/yandex_tracker_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client/objects.py` & `yandex_tracker_client-2.5/yandex_tracker_client/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,16 @@
     def __repr__(self):
         return '<Resource {path}>'.format(
             path=self._path
         )
 
     def __dir__(self):
         return sorted(
-            set(self._collection.fields.keys())
+            set(self._collection.local_fields.keys())
+            | set(self._collection.fields.keys())
             | set(self._collection._injected_properties)
             | set(self._collection._injected_methods)
         )
 
     def __getattr__(self, key):
         collection = self._collection
         if key in collection._injected_methods:
```

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client/uriutils.py` & `yandex_tracker_client-2.5/yandex_tracker_client/uriutils.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client.egg-info/PKG-INFO` & `yandex_tracker_client-2.5/yandex_tracker_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yandex-tracker-client
-Version: 2.3
+Version: 2.5
 Summary: Client for Yandex.Tracker
 Home-page: https://github.com/yandex/yandex_tracker_client
 Author: Yandex Team
 Author-email: smosker@yandex-team.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python yandex.tracker api-client
```

### Comparing `yandex_tracker_client-2.3/yandex_tracker_client.egg-info/SOURCES.txt` & `yandex_tracker_client-2.5/yandex_tracker_client.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS
+LICENSE
 README.rst
 setup.py
 yandex_tracker_client/__init__.py
 yandex_tracker_client/client.py
 yandex_tracker_client/collections.py
 yandex_tracker_client/connection.py
 yandex_tracker_client/exceptions.py
```

### Comparing `yandex_tracker_client-2.3/README.rst` & `yandex_tracker_client-2.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
    [attachment.download_to('some/path') for attachments in client.get_attachments('MYQUEUE-42')]
 
 **Uploading an attachment**
 
 .. code:: python
 
    issue = client.issues['MYQUEUE-42']
-   client.attachments.create('path/to/file')
+   issue.attachments.create('path/to/file')
 
 **Deleting an attachment**
 
 .. code:: python
 
    ATTACHMENTS_TO_DELETE = {'to_delete.txt', 'smth.jpeg'}
    issue = client.issues['MYQUEUE-42']
@@ -157,15 +157,15 @@
        if attach.name in ATTACHMENTS_TO_DELETE:
            attach.delete()
 
 or
 
 .. code:: python
 
-   client.attachments[42].delete()
+   issue.attachments[42].delete()
 
 **List issue comments:**
 
 .. code:: python
 
    issue = client.issues['MYQUEUE-42']
    comments = list(issue.comments.get_all())[:3]
```

### Comparing `yandex_tracker_client-2.3/setup.py` & `yandex_tracker_client-2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='yandex_tracker_client',
-    version='2.3',
+    version='2.5',
     description='Client for Yandex.Tracker',
     author='Yandex Team',
     author_email='smosker@yandex-team.ru',
     url='https://github.com/yandex/yandex_tracker_client',
+    long_description='',
     packages=['yandex_tracker_client'],
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Intended Audience :: Developers',
                  'License :: OSI Approved :: BSD License',
                  'Operating System :: OS Independent',
                  'Topic :: Software Development :: Libraries :: Python Modules',
                  'Programming Language :: Python',
```

### Comparing `yandex_tracker_client-2.3/PKG-INFO` & `yandex_tracker_client-2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yandex_tracker_client
-Version: 2.3
+Version: 2.5
 Summary: Client for Yandex.Tracker
 Home-page: https://github.com/yandex/yandex_tracker_client
 Author: Yandex Team
 Author-email: smosker@yandex-team.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python yandex.tracker api-client
```

