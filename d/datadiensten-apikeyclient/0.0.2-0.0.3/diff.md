# Comparing `tmp/datadiensten-apikeyclient-0.0.2.tar.gz` & `tmp/datadiensten-apikeyclient-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadiensten-apikeyclient-0.0.2.tar", last modified: Thu Mar 30 14:00:10 2023, max compression
+gzip compressed data, was "datadiensten-apikeyclient-0.0.3.tar", last modified: Tue Jul 11 15:01:22 2023, max compression
```

## Comparing `datadiensten-apikeyclient-0.0.2.tar` & `datadiensten-apikeyclient-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-03-30 14:00:10.934988 datadiensten-apikeyclient-0.0.2/
--rw-rw-r--   0 lars      (1000) lars      (1000)      176 2023-03-30 14:00:10.934988 datadiensten-apikeyclient-0.0.2/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)      474 2023-03-30 13:57:28.000000 datadiensten-apikeyclient-0.0.2/pyproject.toml
--rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-03-30 14:00:10.934988 datadiensten-apikeyclient-0.0.2/setup.cfg
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-03-30 14:00:10.934988 datadiensten-apikeyclient-0.0.2/src/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-03-30 14:00:10.934988 datadiensten-apikeyclient-0.0.2/src/apikeyclient/
--rw-rw-r--   0 lars      (1000) lars      (1000)     3059 2023-03-30 13:57:28.000000 datadiensten-apikeyclient-0.0.2/src/apikeyclient/__init__.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-03-30 14:00:10.934988 datadiensten-apikeyclient-0.0.2/src/datadiensten_apikeyclient.egg-info/
--rw-rw-r--   0 lars      (1000) lars      (1000)      176 2023-03-30 14:00:10.000000 datadiensten-apikeyclient-0.0.2/src/datadiensten_apikeyclient.egg-info/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)      255 2023-03-30 14:00:10.000000 datadiensten-apikeyclient-0.0.2/src/datadiensten_apikeyclient.egg-info/SOURCES.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-03-30 14:00:10.000000 datadiensten-apikeyclient-0.0.2/src/datadiensten_apikeyclient.egg-info/dependency_links.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       13 2023-03-30 14:00:10.000000 datadiensten-apikeyclient-0.0.2/src/datadiensten_apikeyclient.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      196 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)      619 2023-07-11 15:00:21.000000 datadiensten-apikeyclient-0.0.3/pyproject.toml
+-rw-rw-r--   0 jan       (1000) jan       (1000)       38 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/setup.cfg
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/src/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/src/apikeyclient/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3042 2023-06-30 07:23:15.000000 datadiensten-apikeyclient-0.0.3/src/apikeyclient/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      196 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)      307 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       66 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       13 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/top_level.txt
```

### Comparing `datadiensten-apikeyclient-0.0.2/src/apikeyclient/__init__.py` & `datadiensten-apikeyclient-0.0.3/src/apikeyclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     * APIKEY_ENDPOINT, to fetch signing keys from. Normally the /signingkeys/
       endpoint from apikeyserv.
     * APIKEY_MANDATORY, boolean that indicates whether API keys are required.
       If set to False, API keys are checked only when they are present, while
       requests without a key are still allowed.
     """
 
-    def __init__(self, get_response, mandatory: bool):
+    def __init__(self, get_response):
         self._client = Client(settings.APIKEY_ENDPOINT)
         self._get_response = get_response
         self._mandatory = bool(settings.APIKEY_MANDATORY)
 
     def __call__(self, request: HttpRequest):
         token = request.headers.get("X-Api-Key")
         if token is None and self._mandatory:
```

