# Comparing `tmp/vinyldns-python-0.9.6.tar.gz` & `tmp/vinyldns-python-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vinyldns-python-0.9.6.tar", last modified: Thu Aug 20 21:34:30 2020, max compression
+gzip compressed data, was "vinyldns-python-0.9.7.tar", last modified: Tue Jul 11 18:13:27 2023, max compression
```

## Comparing `vinyldns-python-0.9.6.tar` & `vinyldns-python-0.9.7.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 remerl200  (1000) remerl200  (1000)        0 2020-08-20 21:34:30.000000 vinyldns-python-0.9.6/
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)    11357 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/LICENSE
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)       53 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/MANIFEST.in
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)      678 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/NOTICE
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     4160 2020-08-20 21:34:30.000000 vinyldns-python-0.9.6/PKG-INFO
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     3010 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/README.md
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)      451 2020-08-20 21:34:30.000000 vinyldns-python-0.9.6/setup.cfg
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     2653 2020-08-20 21:34:22.000000 vinyldns-python-0.9.6/setup.py
-drwxr-xr-x   0 remerl200  (1000) remerl200  (1000)        0 2020-08-20 21:34:30.000000 vinyldns-python-0.9.6/src/
-drwxr-xr-x   0 remerl200  (1000) remerl200  (1000)        0 2020-08-20 21:34:30.000000 vinyldns-python-0.9.6/src/vinyldns/
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)      722 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/__init__.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)    10547 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/batch_change.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     4285 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/boto_request_signer.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)    27655 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/client.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     5730 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/membership.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     7752 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/record.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     4456 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/serdes.py
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     5754 2020-08-20 17:02:42.000000 vinyldns-python-0.9.6/src/vinyldns/zone.py
-drwxr-xr-x   0 remerl200  (1000) remerl200  (1000)        0 2020-08-20 21:34:30.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)     4160 2020-08-20 21:34:29.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/PKG-INFO
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)      518 2020-08-20 21:34:29.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/SOURCES.txt
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)        1 2020-08-20 21:34:29.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/dependency_links.txt
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)        1 2020-08-20 17:20:45.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/not-zip-safe
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)       68 2020-08-20 21:34:29.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/requires.txt
--rw-r--r--   0 remerl200  (1000) remerl200  (1000)        9 2020-08-20 21:34:29.000000 vinyldns-python-0.9.6/src/vinyldns_python.egg-info/top_level.txt
+drwxr-xr-x   0 nspada233   (502) staff       (20)        0 2023-07-11 18:13:27.086527 vinyldns-python-0.9.7/
+-rw-r--r--   0 nspada233   (502) staff       (20)    11357 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/LICENSE
+-rw-r--r--   0 nspada233   (502) staff       (20)       53 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/MANIFEST.in
+-rw-r--r--   0 nspada233   (502) staff       (20)      678 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/NOTICE
+-rw-r--r--   0 nspada233   (502) staff       (20)     3596 2023-07-11 18:13:27.086641 vinyldns-python-0.9.7/PKG-INFO
+-rw-r--r--   0 nspada233   (502) staff       (20)     3010 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/README.md
+-rw-r--r--   0 nspada233   (502) staff       (20)      451 2023-07-11 18:13:27.087121 vinyldns-python-0.9.7/setup.cfg
+-rw-r--r--   0 nspada233   (502) staff       (20)     2653 2023-07-11 18:13:26.000000 vinyldns-python-0.9.7/setup.py
+drwxr-xr-x   0 nspada233   (502) staff       (20)        0 2023-07-11 18:13:27.025501 vinyldns-python-0.9.7/src/
+drwxr-xr-x   0 nspada233   (502) staff       (20)        0 2023-07-11 18:13:27.068205 vinyldns-python-0.9.7/src/vinyldns/
+-rw-r--r--   0 nspada233   (502) staff       (20)      722 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/__init__.py
+-rw-r--r--   0 nspada233   (502) staff       (20)    10547 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/batch_change.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     4285 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/boto_request_signer.py
+-rw-r--r--   0 nspada233   (502) staff       (20)    29480 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/client.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     5730 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/membership.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     7752 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/record.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     4456 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/serdes.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     5754 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/src/vinyldns/zone.py
+drwxr-xr-x   0 nspada233   (502) staff       (20)        0 2023-07-11 18:13:27.078250 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/
+-rw-r--r--   0 nspada233   (502) staff       (20)     3596 2023-07-11 18:13:26.000000 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/PKG-INFO
+-rw-r--r--   0 nspada233   (502) staff       (20)      612 2023-07-11 18:13:26.000000 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/SOURCES.txt
+-rw-r--r--   0 nspada233   (502) staff       (20)        1 2023-07-11 18:13:26.000000 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/dependency_links.txt
+-rw-r--r--   0 nspada233   (502) staff       (20)        1 2023-01-25 16:39:25.000000 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/not-zip-safe
+-rw-r--r--   0 nspada233   (502) staff       (20)       68 2023-07-11 18:13:26.000000 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/requires.txt
+-rw-r--r--   0 nspada233   (502) staff       (20)        9 2023-07-11 18:13:26.000000 vinyldns-python-0.9.7/src/vinyldns_python.egg-info/top_level.txt
+drwxr-xr-x   0 nspada233   (502) staff       (20)        0 2023-07-11 18:13:27.086113 vinyldns-python-0.9.7/tests/
+-rw-r--r--   0 nspada233   (502) staff       (20)    11008 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/tests/test_batch_change.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     7243 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/tests/test_membership.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     8026 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/tests/test_records.py
+-rw-r--r--   0 nspada233   (502) staff       (20)     6993 2023-01-09 22:19:52.000000 vinyldns-python-0.9.7/tests/test_zones.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vinyldns-python-0.9.6/LICENSE` & `vinyldns-python-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/NOTICE` & `vinyldns-python-0.9.7/NOTICE`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/PKG-INFO` & `vinyldns-python-0.9.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: vinyldns-python
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python client library for VinylDNS
 Home-page: https://github.com/vinyldns/vinyldns-python
 Author: vinyldns
 Author-email: vinyldns-core@googlegroups.com
 License: Apache Software License 2.0
-Description: [![PyPI version](https://badge.fury.io/py/vinyldns-python.svg)](https://badge.fury.io/py/vinyldns-python) [![Travis build](https://api.travis-ci.org/vinyldns/vinyldns-python.svg?branch=master)](https://travis-ci.org/vinyldns/vinyldns-python)
-        ![GitHub](https://img.shields.io/github/license/vinyldns/vinyldns-python)
-        
-        # vinyldns-python
-        
-        Python client library for [VinylDNS](https://www.vinyldns.io/)
-        
-        This project is a work in progress! If you would like to help us get this where it needs to be,
-        please reach out to us in [gitter](https://gitter.im/vinyldns/Lobby).
-        
-        To run, `pip install vinyldns-python` and then:
-        
-        ```python
-        >>> from vinyldns.client import VinylDNSClient
-        >>> local_client = VinylDNSClient("ApiEndpoint", "UserAccessKey", "UserSecretKey")
-        >>> local_client.list_zones()
-        >>>
-        >>> # If all of the following environments are set
-        >>> # - VINYLDNS_API_URL
-        >>> # - VINYLDNS_ACCESS_KEY_ID
-        >>> # - VINYLDNS_SECRET_ACCESS_KEY
-        >>> from vinyldns.client import VinylDNSClient
-        >>> local_client = VinylDNSClient.from_env()
-        >>> local_client.list_zones()
-        ```
-        
-        ## Contributing
-        
-        **Requirements**
-        
-        * `python3`
-        * `pip`
-        * `virtualenv`
-        
-        To get started, you will want to setup your virtual environment.
-        
-        1. Ensure that you have `virtualenv` installed `> pip install virtualenv`
-        1. Run `./bootstrap.sh` to setup your environment (unless you really want all these dependencies to be installed locally, which we do not recommend).
-        1. Activate your virtual environment `> source .virtualenv/bin/activate` and you will be ready to go!
-        
-        **Unit Tests**
-        
-        Unit tests are developed using [pytest](https://docs.pytest.org/en/latest/).  We use
-        [Responses](https://github.com/getsentry/responses), which allows for simple mocking of HTTP endpoints.
-        
-        To run unit tests, you can simply run `python3 setup.py test`.  To target a specific test, you can
-        run `python3 setup.py test -a "-k my_test"`
-        
-        **Functional Tests**
-        
-        Functional tests are also developed with pytest. These tests run against a local instance of VinylDNS. Note that for now
-        they are not tied into our travis build, so they must be run locally for validation.
-        
-        From your virtualenv, run `tox -e func_test`
-        
-        **Running a full build**
-        
-        When you are finished writing your code you will want to run everything including linters.  The
-        simplest way to do this is to run `tox -e check,py36`, which will run static checks and run unit tests.
-        
-        If you see any failures / warnings, correct them until `tox` runs successfully.
-        
-        If you do not have `tox` in your environment, `pip install tox` to add it.  For more information you can
-        read the [tox docs](https://tox.readthedocs.io/en/latest/index.html).
-        
-        ## Local Development
-        See the [quickstart](https://github.com/vinyldns/vinyldns/blob/master/README.md#quickstart) in the
-        VinylDNS api for details on how to start up a local instance of the api in docker. With that
-        running, you can make requests with the following client details:
-        ```python
-        local_client = VinylDNSClient("http://localhost:9000", "okAccessKey", "okSecretKey")
-        ```
-        
 Keywords: dns,python,vinyldns
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
+[![PyPI version](https://badge.fury.io/py/vinyldns-python.svg)](https://badge.fury.io/py/vinyldns-python) [![Travis build](https://api.travis-ci.org/vinyldns/vinyldns-python.svg?branch=master)](https://travis-ci.org/vinyldns/vinyldns-python)
+![GitHub](https://img.shields.io/github/license/vinyldns/vinyldns-python)
+
+# vinyldns-python
+
+Python client library for [VinylDNS](https://www.vinyldns.io/)
+
+This project is a work in progress! If you would like to help us get this where it needs to be,
+please reach out to us in [gitter](https://gitter.im/vinyldns/Lobby).
+
+To run, `pip install vinyldns-python` and then:
+
+```python
+>>> from vinyldns.client import VinylDNSClient
+>>> local_client = VinylDNSClient("ApiEndpoint", "UserAccessKey", "UserSecretKey")
+>>> local_client.list_zones()
+>>>
+>>> # If all of the following environments are set
+>>> # - VINYLDNS_API_URL
+>>> # - VINYLDNS_ACCESS_KEY_ID
+>>> # - VINYLDNS_SECRET_ACCESS_KEY
+>>> from vinyldns.client import VinylDNSClient
+>>> local_client = VinylDNSClient.from_env()
+>>> local_client.list_zones()
+```
+
+## Contributing
+
+**Requirements**
+
+* `python3`
+* `pip`
+* `virtualenv`
+
+To get started, you will want to setup your virtual environment.
+
+1. Ensure that you have `virtualenv` installed `> pip install virtualenv`
+1. Run `./bootstrap.sh` to setup your environment (unless you really want all these dependencies to be installed locally, which we do not recommend).
+1. Activate your virtual environment `> source .virtualenv/bin/activate` and you will be ready to go!
+
+**Unit Tests**
+
+Unit tests are developed using [pytest](https://docs.pytest.org/en/latest/).  We use
+[Responses](https://github.com/getsentry/responses), which allows for simple mocking of HTTP endpoints.
+
+To run unit tests, you can simply run `python3 setup.py test`.  To target a specific test, you can
+run `python3 setup.py test -a "-k my_test"`
+
+**Functional Tests**
+
+Functional tests are also developed with pytest. These tests run against a local instance of VinylDNS. Note that for now
+they are not tied into our travis build, so they must be run locally for validation.
+
+From your virtualenv, run `tox -e func_test`
+
+**Running a full build**
+
+When you are finished writing your code you will want to run everything including linters.  The
+simplest way to do this is to run `tox -e check,py36`, which will run static checks and run unit tests.
+
+If you see any failures / warnings, correct them until `tox` runs successfully.
+
+If you do not have `tox` in your environment, `pip install tox` to add it.  For more information you can
+read the [tox docs](https://tox.readthedocs.io/en/latest/index.html).
+
+## Local Development
+See the [quickstart](https://github.com/vinyldns/vinyldns/blob/master/README.md#quickstart) in the
+VinylDNS api for details on how to start up a local instance of the api in docker. With that
+running, you can make requests with the following client details:
+```python
+local_client = VinylDNSClient("http://localhost:9000", "okAccessKey", "okSecretKey")
+```
```

### Comparing `vinyldns-python-0.9.6/README.md` & `vinyldns-python-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/setup.py` & `vinyldns-python-0.9.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     cmdclass={'test': PyTest},
     name='vinyldns-python',
-    version='0.9.6',
+    version='0.9.7',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
     url='https://github.com/vinyldns/vinyldns-python',
     license='Apache Software License 2.0',
```

### Comparing `vinyldns-python-0.9.6/src/vinyldns/__init__.py` & `vinyldns-python-0.9.7/src/vinyldns/__init__.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns/batch_change.py` & `vinyldns-python-0.9.7/src/vinyldns/batch_change.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns/boto_request_signer.py` & `vinyldns-python-0.9.7/src/vinyldns/boto_request_signer.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns/client.py` & `vinyldns-python-0.9.7/src/vinyldns/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -561,14 +561,48 @@
             args.append(u'recordNameFilter={0}'.format(record_name_filter))
 
         url = urljoin(self.index_url, u'/zones/{0}/recordsets'.format(zone_id)) + u'?' + u'&'.join(args)
 
         response, data = self.__make_request(url, u'GET', self.headers, **kwargs)
         return ListRecordSetsResponse.from_dict(data)
 
+    def search_record_sets(self, start_from=None, max_items=None, record_name_filter=None,
+                           record_type_filter=None, record_owner_group_filter=None, name_sort=None, **kwargs):
+        """
+        Retrieves a list of RecordSets globally in the VinylDNS database based on search criteria.
+        A minimum of two alpha-numeric characters is required.
+
+        :param start_from: the start key of the page
+        :param max_items: the page limit
+        :param record_name_filter: only returns record_sets whose names contain filter string
+        :param record_type_filter: only returns record_sets whose type is present in the given list
+        :param record_owner_group_filter: only returns record_sets belonging to the given owner
+        :param name_sort: sort the results as per given order
+        :return: the content of the response
+        """
+        args = []
+        if start_from is not None:
+            args.append(u'startFrom={0}'.format(start_from))
+        if max_items is not None:
+            args.append(u'maxItems={0}'.format(max_items))
+        if record_name_filter is not None:
+            args.append(u'recordNameFilter={0}'.format(record_name_filter))
+        if record_type_filter is not None:
+            for record_type in record_type_filter:
+                args.append(u'recordTypeFilter[]={0}'.format(record_type))
+        if record_owner_group_filter is not None:
+            args.append(u'recordOwnerGroupFilter={0}'.format(record_owner_group_filter))
+        if name_sort is not None:
+            args.append(u'nameSort={0}'.format(name_sort))
+
+        url = urljoin(self.index_url, u'/recordsets') + u'?' + u'&'.join(args)
+
+        response, data = self.__make_request(url, u'GET', self.headers, **kwargs)
+        return ListRecordSetsResponse.from_dict(data)
+
     def get_record_set_change(self, zone_id, rs_id, change_id, **kwargs):
         """
         Get an existing record_set change.
 
         :param zone_id: the zone id the record_set belongs to
         :param rs_id: the id of the record_set to be retrieved
         :param change_id: the id of the change to be retrieved
```

### Comparing `vinyldns-python-0.9.6/src/vinyldns/membership.py` & `vinyldns-python-0.9.7/src/vinyldns/membership.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns/record.py` & `vinyldns-python-0.9.7/src/vinyldns/record.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns/serdes.py` & `vinyldns-python-0.9.7/src/vinyldns/serdes.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns/zone.py` & `vinyldns-python-0.9.7/src/vinyldns/zone.py`

 * *Files identical despite different names*

### Comparing `vinyldns-python-0.9.6/src/vinyldns_python.egg-info/PKG-INFO` & `vinyldns-python-0.9.7/src/vinyldns_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: vinyldns-python
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python client library for VinylDNS
 Home-page: https://github.com/vinyldns/vinyldns-python
 Author: vinyldns
 Author-email: vinyldns-core@googlegroups.com
 License: Apache Software License 2.0
-Description: [![PyPI version](https://badge.fury.io/py/vinyldns-python.svg)](https://badge.fury.io/py/vinyldns-python) [![Travis build](https://api.travis-ci.org/vinyldns/vinyldns-python.svg?branch=master)](https://travis-ci.org/vinyldns/vinyldns-python)
-        ![GitHub](https://img.shields.io/github/license/vinyldns/vinyldns-python)
-        
-        # vinyldns-python
-        
-        Python client library for [VinylDNS](https://www.vinyldns.io/)
-        
-        This project is a work in progress! If you would like to help us get this where it needs to be,
-        please reach out to us in [gitter](https://gitter.im/vinyldns/Lobby).
-        
-        To run, `pip install vinyldns-python` and then:
-        
-        ```python
-        >>> from vinyldns.client import VinylDNSClient
-        >>> local_client = VinylDNSClient("ApiEndpoint", "UserAccessKey", "UserSecretKey")
-        >>> local_client.list_zones()
-        >>>
-        >>> # If all of the following environments are set
-        >>> # - VINYLDNS_API_URL
-        >>> # - VINYLDNS_ACCESS_KEY_ID
-        >>> # - VINYLDNS_SECRET_ACCESS_KEY
-        >>> from vinyldns.client import VinylDNSClient
-        >>> local_client = VinylDNSClient.from_env()
-        >>> local_client.list_zones()
-        ```
-        
-        ## Contributing
-        
-        **Requirements**
-        
-        * `python3`
-        * `pip`
-        * `virtualenv`
-        
-        To get started, you will want to setup your virtual environment.
-        
-        1. Ensure that you have `virtualenv` installed `> pip install virtualenv`
-        1. Run `./bootstrap.sh` to setup your environment (unless you really want all these dependencies to be installed locally, which we do not recommend).
-        1. Activate your virtual environment `> source .virtualenv/bin/activate` and you will be ready to go!
-        
-        **Unit Tests**
-        
-        Unit tests are developed using [pytest](https://docs.pytest.org/en/latest/).  We use
-        [Responses](https://github.com/getsentry/responses), which allows for simple mocking of HTTP endpoints.
-        
-        To run unit tests, you can simply run `python3 setup.py test`.  To target a specific test, you can
-        run `python3 setup.py test -a "-k my_test"`
-        
-        **Functional Tests**
-        
-        Functional tests are also developed with pytest. These tests run against a local instance of VinylDNS. Note that for now
-        they are not tied into our travis build, so they must be run locally for validation.
-        
-        From your virtualenv, run `tox -e func_test`
-        
-        **Running a full build**
-        
-        When you are finished writing your code you will want to run everything including linters.  The
-        simplest way to do this is to run `tox -e check,py36`, which will run static checks and run unit tests.
-        
-        If you see any failures / warnings, correct them until `tox` runs successfully.
-        
-        If you do not have `tox` in your environment, `pip install tox` to add it.  For more information you can
-        read the [tox docs](https://tox.readthedocs.io/en/latest/index.html).
-        
-        ## Local Development
-        See the [quickstart](https://github.com/vinyldns/vinyldns/blob/master/README.md#quickstart) in the
-        VinylDNS api for details on how to start up a local instance of the api in docker. With that
-        running, you can make requests with the following client details:
-        ```python
-        local_client = VinylDNSClient("http://localhost:9000", "okAccessKey", "okSecretKey")
-        ```
-        
 Keywords: dns,python,vinyldns
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
+[![PyPI version](https://badge.fury.io/py/vinyldns-python.svg)](https://badge.fury.io/py/vinyldns-python) [![Travis build](https://api.travis-ci.org/vinyldns/vinyldns-python.svg?branch=master)](https://travis-ci.org/vinyldns/vinyldns-python)
+![GitHub](https://img.shields.io/github/license/vinyldns/vinyldns-python)
+
+# vinyldns-python
+
+Python client library for [VinylDNS](https://www.vinyldns.io/)
+
+This project is a work in progress! If you would like to help us get this where it needs to be,
+please reach out to us in [gitter](https://gitter.im/vinyldns/Lobby).
+
+To run, `pip install vinyldns-python` and then:
+
+```python
+>>> from vinyldns.client import VinylDNSClient
+>>> local_client = VinylDNSClient("ApiEndpoint", "UserAccessKey", "UserSecretKey")
+>>> local_client.list_zones()
+>>>
+>>> # If all of the following environments are set
+>>> # - VINYLDNS_API_URL
+>>> # - VINYLDNS_ACCESS_KEY_ID
+>>> # - VINYLDNS_SECRET_ACCESS_KEY
+>>> from vinyldns.client import VinylDNSClient
+>>> local_client = VinylDNSClient.from_env()
+>>> local_client.list_zones()
+```
+
+## Contributing
+
+**Requirements**
+
+* `python3`
+* `pip`
+* `virtualenv`
+
+To get started, you will want to setup your virtual environment.
+
+1. Ensure that you have `virtualenv` installed `> pip install virtualenv`
+1. Run `./bootstrap.sh` to setup your environment (unless you really want all these dependencies to be installed locally, which we do not recommend).
+1. Activate your virtual environment `> source .virtualenv/bin/activate` and you will be ready to go!
+
+**Unit Tests**
+
+Unit tests are developed using [pytest](https://docs.pytest.org/en/latest/).  We use
+[Responses](https://github.com/getsentry/responses), which allows for simple mocking of HTTP endpoints.
+
+To run unit tests, you can simply run `python3 setup.py test`.  To target a specific test, you can
+run `python3 setup.py test -a "-k my_test"`
+
+**Functional Tests**
+
+Functional tests are also developed with pytest. These tests run against a local instance of VinylDNS. Note that for now
+they are not tied into our travis build, so they must be run locally for validation.
+
+From your virtualenv, run `tox -e func_test`
+
+**Running a full build**
+
+When you are finished writing your code you will want to run everything including linters.  The
+simplest way to do this is to run `tox -e check,py36`, which will run static checks and run unit tests.
+
+If you see any failures / warnings, correct them until `tox` runs successfully.
+
+If you do not have `tox` in your environment, `pip install tox` to add it.  For more information you can
+read the [tox docs](https://tox.readthedocs.io/en/latest/index.html).
+
+## Local Development
+See the [quickstart](https://github.com/vinyldns/vinyldns/blob/master/README.md#quickstart) in the
+VinylDNS api for details on how to start up a local instance of the api in docker. With that
+running, you can make requests with the following client details:
+```python
+local_client = VinylDNSClient("http://localhost:9000", "okAccessKey", "okSecretKey")
+```
```

