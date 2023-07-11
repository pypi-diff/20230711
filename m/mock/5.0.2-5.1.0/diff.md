# Comparing `tmp/mock-5.0.2.tar.gz` & `tmp/mock-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock-5.0.2.tar", last modified: Sun Apr 16 11:26:52 2023, max compression
+gzip compressed data, was "mock-5.1.0.tar", last modified: Tue Jul 11 13:34:34 2023, max compression
```

## Comparing `mock-5.0.2.tar` & `mock-5.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.041844 mock-5.0.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16940 2023-04-16 11:26:45.000000 mock-5.0.2/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-04-16 11:26:45.000000 mock-5.0.2/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-16 11:26:45.000000 mock-5.0.2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-04-16 11:26:52.041844 mock-5.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-16 11:26:45.000000 mock-5.0.2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.037844 mock-5.0.2/mock/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-04-16 11:26:45.000000 mock-5.0.2/mock/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2808 2023-04-16 11:26:45.000000 mock-5.0.2/mock/backports.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105795 2023-04-16 11:26:45.000000 mock-5.0.2/mock/mock.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.041844 mock-5.0.2/mock/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/support.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38696 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testasync.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4263 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testcallable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34990 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testhelpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testmagicmethods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    77314 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testmock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60095 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testpatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7391 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testsealable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1316 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testsentinel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12208 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testwith.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.037844 mock-5.0.2/mock.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1410 2023-04-16 11:26:52.041844 mock-5.0.2/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      246 2023-04-16 11:26:45.000000 mock-5.0.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-11 13:34:34.394673 mock-5.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17574 2023-07-11 13:34:26.000000 mock-5.1.0/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-07-11 13:34:26.000000 mock-5.1.0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-07-11 13:34:26.000000 mock-5.1.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2775 2023-07-11 13:34:34.394673 mock-5.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-07-11 13:34:26.000000 mock-5.1.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-11 13:34:34.390673 mock-5.1.0/mock/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-07-11 13:34:26.000000 mock-5.1.0/mock/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2808 2023-07-11 13:34:26.000000 mock-5.1.0/mock/backports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   110383 2023-07-11 13:34:26.000000 mock-5.1.0/mock/mock.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-11 13:34:34.394673 mock-5.1.0/mock/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/support.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39695 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testasync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4263 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testcallable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34990 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testhelpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testmagicmethods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78854 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testmock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60095 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testpatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7391 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testsealable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1316 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testsentinel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10144 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testthreadingmock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12256 2023-07-11 13:34:26.000000 mock-5.1.0/mock/tests/testwith.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-11 13:34:34.390673 mock-5.1.0/mock.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2775 2023-07-11 13:34:34.000000 mock-5.1.0/mock.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-11 13:34:34.000000 mock-5.1.0/mock.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-11 13:34:34.000000 mock-5.1.0/mock.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-07-11 13:34:34.000000 mock-5.1.0/mock.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-07-11 13:34:34.000000 mock-5.1.0/mock.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1410 2023-07-11 13:34:34.394673 mock-5.1.0/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      246 2023-07-11 13:34:26.000000 mock-5.1.0/setup.py
```

### Comparing `mock-5.0.2/CHANGELOG.rst` & `mock-5.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+5.1.0
+-----
+
+- bpo-44185: :func:`unittest.mock.mock_open` will call the :func:`close`
+  method of the file handle mock when it is exiting from the context
+  manager. Patch by Samet Yaslan.
+
+- gh-94924: :func:`unittest.mock.create_autospec` now properly returns
+  coroutine functions compatible with :func:`inspect.iscoroutinefunction`
+
+- bpo-17013: Add ``ThreadingMock`` to :mod:`unittest.mock` that can be used
+  to create Mock objects that can wait until they are called. Patch by
+  Karthikeyan Singaravelan and Mario Corchero.
+
+- bpo-41768: :mod:`unittest.mock` speccing no longer calls class properties.
+  Patch by Melanie Witt.
+
 5.0.2
 -----
 
 - gh-102978: Fixes :func:`unittest.mock.patch` not enforcing function
   signatures for methods decorated with ``@classmethod`` or
   ``@staticmethod`` when patch is called with ``autospec=True``.
```

### Comparing `mock-5.0.2/LICENSE.txt` & `mock-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/PKG-INFO` & `mock-5.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mock
-Version: 5.0.2
+Version: 5.1.0
 Summary: Rolling backport of unittest.mock for all Pythons
 Home-page: http://mock.readthedocs.org/en/latest/
 Author: Testing Cabal
 Author-email: testing-in-python@lists.idyll.org
-License: UNKNOWN
 Project-URL: Source, https://github.com/testing-cabal/mock
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -63,9 +61,7 @@
     .. |Docs| image:: https://readthedocs.org/projects/mock/badge/?version=latest
     .. _Docs: http://mock.readthedocs.org/en/latest/
 
 .. _Mock Homepage: http://mock.readthedocs.org/en/latest/
 .. _BSD License: https://github.com/testing-cabal/mock/blob/master/LICENSE.txt
 .. _Python Docs: https://docs.python.org/dev/library/unittest.mock.html
 .. _mock on PyPI: https://pypi.org/project/mock/
-
-
```

### Comparing `mock-5.0.2/README.rst` & `mock-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/backports.py` & `mock-5.1.0/mock/backports.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/mock.py` & `mock-5.1.0/mock/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     'patch',
     'sentinel',
     'DEFAULT',
     'ANY',
     'call',
     'create_autospec',
     'AsyncMock',
+    'ThreadingMock',
     'FILTER_DIR',
     'NonCallableMock',
     'NonCallableMagicMock',
     'mock_open',
     'PropertyMock',
     'seal',
 )
@@ -25,16 +26,16 @@
 
 import asyncio
 import contextlib
 import io
 import inspect
 import pprint
 import sys
+import threading
 import builtins
-from asyncio import iscoroutinefunction
 from types import CodeType, ModuleType, MethodType
 from unittest.util import safe_repr
 from functools import wraps, partial
 from threading import RLock
 
 
 from mock import IS_PYPY
@@ -203,14 +204,36 @@
     _checksig_(*args, **kwargs)
     return mock(*args, **kwargs)""" % name
     exec (src, context)
     funcopy = context[name]
     _setup_func(funcopy, mock, sig)
     return funcopy
 
+def _set_async_signature(mock, original, instance=False, is_async_mock=False):
+    # creates an async function with signature (*args, **kwargs) that delegates to a
+    # mock. It still does signature checking by calling a lambda with the same
+    # signature as the original.
+
+    skipfirst = isinstance(original, type)
+    func, sig = _get_signature_object(original, instance, skipfirst)
+    def checksig(*args, **kwargs):
+        sig.bind(*args, **kwargs)
+    _copy_func_details(func, checksig)
+
+    name = original.__name__
+    context = {'_checksig_': checksig, 'mock': mock}
+    src = """async def %s(*args, **kwargs):
+    _checksig_(*args, **kwargs)
+    return await mock(*args, **kwargs)""" % name
+    exec (src, context)
+    funcopy = context[name]
+    _setup_func(funcopy, mock, sig)
+    _setup_async_mock(funcopy)
+    return funcopy
+
 
 def _setup_func(funcopy, mock, sig):
     funcopy.mock = mock
 
     def assert_called_with(*args, **kwargs):
         return mock.assert_called_with(*args, **kwargs)
     def assert_called(*args, **kwargs):
@@ -525,15 +548,21 @@
             res = _get_signature_object(spec,
                                         _spec_as_instance, _eat_self)
             _spec_signature = res and res[1]
 
             spec_list = dir(spec)
 
             for attr in spec_list:
-                if iscoroutinefunction(getattr(spec, attr, None)):
+                static_attr = inspect.getattr_static(spec, attr, None)
+                unwrapped_attr = static_attr
+                try:
+                    unwrapped_attr = inspect.unwrap(unwrapped_attr)
+                except ValueError:
+                    pass
+                if iscoroutinefunction(unwrapped_attr):
                     _spec_asyncs.append(attr)
 
             spec = spec_list
 
         __dict__ = self.__dict__
         __dict__['_spec_class'] = _spec_class
         __dict__['_spec_set'] = spec_set
@@ -2788,17 +2817,18 @@
 
     mock = Klass(parent=_parent, _new_parent=_parent, _new_name=_new_name,
                  name=_name, **_kwargs)
 
     if isinstance(spec, FunctionTypes):
         # should only happen at the top level because we don't
         # recurse for functions
-        mock = _set_signature(mock, spec)
         if is_async_func:
-            _setup_async_mock(mock)
+            mock = _set_async_signature(mock, spec)
+        else:
+            mock = _set_signature(mock, spec)
     else:
         _check_signature(spec, mock, is_type, instance)
 
     if _parent is not None and not instance:
         _parent._mock_children[_name] = mock
 
     if is_type and not instance and 'return_value' not in kwargs:
@@ -2956,14 +2986,17 @@
             yield line
 
     def _next_side_effect():
         if handle.readline.return_value is not None:
             return handle.readline.return_value
         return next(_state[0])
 
+    def _exit_side_effect(exctype, excinst, exctb):
+        handle.close()
+
     global file_spec
     if file_spec is None:
         import _io
         file_spec = list(set(dir(_io.TextIOWrapper)).union(set(dir(_io.BytesIO))))
 
     global open_spec
     if open_spec is None:
@@ -2982,14 +3015,15 @@
 
     handle.read.side_effect = _read_side_effect
     _state[1] = _readline_side_effect()
     handle.readline.side_effect = _state[1]
     handle.readlines.side_effect = _readlines_side_effect
     handle.__iter__.side_effect = _iter_side_effect
     handle.__next__.side_effect = _next_side_effect
+    handle.__exit__.side_effect = _exit_side_effect
 
     def reset_data(*args, **kwargs):
         _state[0] = _to_stream(read_data)
         if handle.readline.side_effect == _state[1]:
             # Only reset the side effect if the user hasn't overridden it.
             _state[1] = _readline_side_effect()
             handle.readline.side_effect = _state[1]
@@ -3014,14 +3048,104 @@
 
     def __get__(self, obj, obj_type=None):
         return self()
     def __set__(self, obj, val):
         self(val)
 
 
+_timeout_unset = sentinel.TIMEOUT_UNSET
+
+class ThreadingMixin(Base):
+
+    DEFAULT_TIMEOUT = None
+
+    def _get_child_mock(self, **kw):
+        if isinstance(kw.get("parent"), ThreadingMixin):
+            kw["timeout"] = kw["parent"]._mock_wait_timeout
+        elif isinstance(kw.get("_new_parent"), ThreadingMixin):
+            kw["timeout"] = kw["_new_parent"]._mock_wait_timeout
+        return super()._get_child_mock(**kw)
+
+    def __init__(self, *args, timeout=_timeout_unset, **kwargs):
+        super().__init__(*args, **kwargs)
+        if timeout is _timeout_unset:
+            timeout = self.DEFAULT_TIMEOUT
+        self.__dict__["_mock_event"] = threading.Event()  # Event for any call
+        self.__dict__["_mock_calls_events"] = []  # Events for each of the calls
+        self.__dict__["_mock_calls_events_lock"] = threading.Lock()
+        self.__dict__["_mock_wait_timeout"] = timeout
+
+    def reset_mock(self, *args, **kwargs):
+        """
+        See :func:`.Mock.reset_mock()`
+        """
+        super().reset_mock(*args, **kwargs)
+        self.__dict__["_mock_event"] = threading.Event()
+        self.__dict__["_mock_calls_events"] = []
+
+    def __get_event(self, expected_args, expected_kwargs):
+        with self._mock_calls_events_lock:
+            for args, kwargs, event in self._mock_calls_events:
+                if (args, kwargs) == (expected_args, expected_kwargs):
+                    return event
+            new_event = threading.Event()
+            self._mock_calls_events.append((expected_args, expected_kwargs, new_event))
+        return new_event
+
+    def _mock_call(self, *args, **kwargs):
+        ret_value = super()._mock_call(*args, **kwargs)
+
+        call_event = self.__get_event(args, kwargs)
+        call_event.set()
+
+        self._mock_event.set()
+
+        return ret_value
+
+    def wait_until_called(self, *, timeout=_timeout_unset):
+        """Wait until the mock object is called.
+
+        `timeout` - time to wait for in seconds, waits forever otherwise.
+        Defaults to the constructor provided timeout.
+        Use None to block undefinetively.
+        """
+        if timeout is _timeout_unset:
+            timeout = self._mock_wait_timeout
+        if not self._mock_event.wait(timeout=timeout):
+            msg = (f"{self._mock_name or 'mock'} was not called before"
+                   f" timeout({timeout}).")
+            raise AssertionError(msg)
+
+    def wait_until_any_call_with(self, *args, **kwargs):
+        """Wait until the mock object is called with given args.
+
+        Waits for the timeout in seconds provided in the constructor.
+        """
+        event = self.__get_event(args, kwargs)
+        if not event.wait(timeout=self._mock_wait_timeout):
+            expected_string = self._format_mock_call_signature(args, kwargs)
+            raise AssertionError(f'{expected_string} call not found')
+
+
+class ThreadingMock(ThreadingMixin, MagicMixin, Mock):
+    """
+    A mock that can be used to wait until on calls happening
+    in a different thread.
+
+    The constructor can take a `timeout` argument which
+    controls the timeout in seconds for all `wait` calls of the mock.
+
+    You can change the default timeout of all instances via the
+    `ThreadingMock.DEFAULT_TIMEOUT` attribute.
+
+    If no timeout is set, it will block undefinetively.
+    """
+    pass
+
+
 def seal(mock):
     """Disable the automatic generation of child mocks.
 
     Given an input Mock, seals it to ensure no further mocks will be generated
     when accessing an attribute that was not already defined.
 
     The operation recursively seals the mock passed in, meaning that
```

### Comparing `mock-5.0.2/mock/tests/support.py` & `mock-5.1.0/mock/tests/support.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testasync.py` & `mock-5.1.0/mock/tests/testasync.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,36 +238,59 @@
         self.assertIsNone(spec.await_args)
         self.assertEqual(spec.await_args_list, [])
         spec.assert_not_awaited()
 
         run(main())
 
         self.assertTrue(iscoroutinefunction(spec))
+        self.assertTrue(inspect.iscoroutinefunction(spec))
         self.assertTrue(asyncio.iscoroutine(awaitable))
+        self.assertTrue(inspect.iscoroutine(awaitable))
         self.assertEqual(spec.await_count, 1)
         self.assertEqual(spec.await_args, call(1, 2, c=3))
         self.assertEqual(spec.await_args_list, [call(1, 2, c=3)])
         spec.assert_awaited_once()
         spec.assert_awaited_once_with(1, 2, c=3)
         spec.assert_awaited_with(1, 2, c=3)
         spec.assert_awaited()
 
         with self.assertRaises(AssertionError):
             spec.assert_any_await(e=1)
 
+    def test_autospec_checks_signature(self):
+        spec = create_autospec(async_func_args)
+        # signature is not checked when called
+        awaitable = spec()
+        self.assertListEqual(spec.mock_calls, [])
+
+        async def main():
+            await awaitable
+
+        # but it is checked when awaited
+        with self.assertRaises(TypeError):
+            run(main())
+
+        # _checksig_ raises before running or awaiting the mock
+        self.assertListEqual(spec.mock_calls, [])
+        self.assertEqual(spec.await_count, 0)
+        self.assertIsNone(spec.await_args)
+        self.assertEqual(spec.await_args_list, [])
+        spec.assert_not_awaited()
 
     def test_patch_with_autospec(self):
 
         async def test_async():
             with patch(f"{__name__}.async_func_args", autospec=True) as mock_method:
                 awaitable = mock_method(1, 2, c=3)
                 self.assertIsInstance(mock_method.mock, AsyncMock)
 
                 self.assertTrue(iscoroutinefunction(mock_method))
+                self.assertTrue(inspect.iscoroutinefunction(mock_method))
                 self.assertTrue(asyncio.iscoroutine(awaitable))
+                self.assertTrue(inspect.iscoroutine(awaitable))
                 self.assertTrue(inspect.isawaitable(awaitable))
 
                 # Verify the default values during mock setup
                 self.assertEqual(mock_method.await_count, 0)
                 self.assertEqual(mock_method.await_args_list, [])
                 self.assertIsNone(mock_method.await_args)
                 mock_method.assert_not_awaited()
@@ -442,17 +465,18 @@
 
         mock = AsyncMock(addition, return_value=10)
         output = await mock(5)
 
         self.assertEqual(output, 10)
 
     async def test_add_side_effect_exception(self):
+        class CustomError(Exception): pass
         async def addition(var): pass
-        mock = AsyncMock(addition, side_effect=Exception('err'))
-        with self.assertRaises(Exception):
+        mock = AsyncMock(addition, side_effect=CustomError('side-effect'))
+        with self.assertRaisesRegex(CustomError, 'side-effect'):
             await mock(5)
 
     async def test_add_side_effect_coroutine(self):
         async def addition(var):
             return var + 1
         mock = AsyncMock(side_effect=addition)
         result = await mock(5)
```

### Comparing `mock-5.0.2/mock/tests/testcallable.py` & `mock-5.1.0/mock/tests/testcallable.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testhelpers.py` & `mock-5.1.0/mock/tests/testhelpers.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testmagicmethods.py` & `mock-5.1.0/mock/tests/testmagicmethods.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testmock.py` & `mock-5.1.0/mock/tests/testmock.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,25 @@
     @classmethod
     def cmeth(cls, a, b, c, d=None): pass
 
     @staticmethod
     def smeth(a, b, c, d=None): pass
 
 
+class SomethingElse(object):
+    def __init__(self):
+        self._instance = None
+
+    @property
+    def instance(self):
+        if not self._instance:
+            self._instance = 'object'
+        return self._instance
+
+
 class Typos():
     autospect = None
     auto_spec = None
     set_spec = None
 
 
 def something(a): pass
@@ -231,14 +242,22 @@
                                         "Cannot spec attr 'B' as the spec_set "):
                 mock.patch.object(A, 'B', spec_set=A.B).start()
             with self.assertRaisesRegex(InvalidSpecError, "Cannot spec a Mock object."):
                 mock.Mock(A.B)
             with mock.patch('builtins.open', mock.mock_open()):
                 mock.mock_open()  # should still be valid with open() mocked
 
+    def test_explicit_parent(self):
+        parent = Mock()
+        mock1 = Mock(parent=parent, return_value=None)
+        mock1(1, 2, 3)
+        mock2 = Mock(parent=parent, return_value=None)
+        mock2(4, 5, 6)
+
+        self.assertEqual(parent.mock_calls, [call(1, 2, 3), call(4, 5, 6)])
 
     def test_reset_mock(self):
         parent = Mock()
         spec = ["something"]
         mock = Mock(name="child", parent=parent, spec=spec)
         mock(sentinel.Something, something=sentinel.SomethingElse)
         something = mock.something
@@ -2292,10 +2311,34 @@
             pass
         with patch.object(Foo, 'one', unsafe=True, set_spec=True): pass
         m = create_autospec(Foo, set_spec=True, unsafe=True)
         with patch.multiple(
             f'{__name__}.Typos', autospect=True, set_spec=True, auto_spec=True):
             pass
 
+    def test_property_not_called_with_spec_mock(self):
+        obj = SomethingElse()
+        self.assertIsNone(obj._instance, msg='before mock')
+        mock = Mock(spec=obj)
+        self.assertIsNone(obj._instance, msg='after mock')
+        self.assertEqual('object', obj.instance)
+
+    def test_decorated_async_methods_with_spec_mock(self):
+        class Foo():
+            @classmethod
+            async def class_method(cls):
+                pass  # pragma: no cover
+            @staticmethod
+            async def static_method():
+                pass  # pragma: no cover
+            async def method(self):
+                pass  # pragma: no cover
+        mock = Mock(spec=Foo)
+        for m in (mock.method, mock.class_method, mock.static_method):
+            if sys.version_info[:2] <= (3, 9) and m is not mock.method:
+                # class and static methods need bugfixes in cpython to work:
+                self.assertIsInstance(m, Mock)
+                continue
+            self.assertIsInstance(m, AsyncMock)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mock-5.0.2/mock/tests/testpatch.py` & `mock-5.1.0/mock/tests/testpatch.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testsealable.py` & `mock-5.1.0/mock/tests/testsealable.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testsentinel.py` & `mock-5.1.0/mock/tests/testsentinel.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.2/mock/tests/testwith.py` & `mock-5.1.0/mock/tests/testwith.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,31 +154,31 @@
         mock = mock_open()
         handle = mock.return_value
         with patch('%s.open' % __name__, mock, create=True):
             with open('foo') as f:
                 f.read()
 
         expected_calls = [call('foo'), call().__enter__(), call().read(),
-                          call().__exit__(None, None, None)]
+                          call().__exit__(None, None, None), call().close()]
         self.assertEqual(mock.mock_calls, expected_calls)
         self.assertIs(f, handle)
 
     def test_mock_open_context_manager_multiple_times(self):
         mock = mock_open()
         with patch('%s.open' % __name__, mock, create=True):
             with open('foo') as f:
                 f.read()
             with open('bar') as f:
                 f.read()
 
         expected_calls = [
             call('foo'), call().__enter__(), call().read(),
-            call().__exit__(None, None, None),
+            call().__exit__(None, None, None), call().close(),
             call('bar'), call().__enter__(), call().read(),
-            call().__exit__(None, None, None)]
+            call().__exit__(None, None, None), call().close()]
         self.assertEqual(mock.mock_calls, expected_calls)
 
     def test_explicit_mock(self):
         mock = MagicMock()
         mock_open(mock)
 
         with patch('%s.open' % __name__, mock, create=True) as patched:
```

### Comparing `mock-5.0.2/mock.egg-info/PKG-INFO` & `mock-5.1.0/mock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mock
-Version: 5.0.2
+Version: 5.1.0
 Summary: Rolling backport of unittest.mock for all Pythons
 Home-page: http://mock.readthedocs.org/en/latest/
 Author: Testing Cabal
 Author-email: testing-in-python@lists.idyll.org
-License: UNKNOWN
 Project-URL: Source, https://github.com/testing-cabal/mock
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -63,9 +61,7 @@
     .. |Docs| image:: https://readthedocs.org/projects/mock/badge/?version=latest
     .. _Docs: http://mock.readthedocs.org/en/latest/
 
 .. _Mock Homepage: http://mock.readthedocs.org/en/latest/
 .. _BSD License: https://github.com/testing-cabal/mock/blob/master/LICENSE.txt
 .. _Python Docs: https://docs.python.org/dev/library/unittest.mock.html
 .. _mock on PyPI: https://pypi.org/project/mock/
-
-
```

### Comparing `mock-5.0.2/mock.egg-info/SOURCES.txt` & `mock-5.1.0/mock.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 mock/tests/testcallable.py
 mock/tests/testhelpers.py
 mock/tests/testmagicmethods.py
 mock/tests/testmock.py
 mock/tests/testpatch.py
 mock/tests/testsealable.py
 mock/tests/testsentinel.py
+mock/tests/testthreadingmock.py
 mock/tests/testwith.py
```

### Comparing `mock-5.0.2/setup.cfg` & `mock-5.1.0/setup.cfg`

 * *Files identical despite different names*

