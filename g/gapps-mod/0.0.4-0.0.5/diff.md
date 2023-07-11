# Comparing `tmp/gapps-mod-0.0.4.tar.gz` & `tmp/gapps-mod-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gapps-mod-0.0.4.tar", last modified: Tue Jul 11 18:28:07 2023, max compression
+gzip compressed data, was "gapps-mod-0.0.5.tar", last modified: Tue Jul 11 18:30:49 2023, max compression
```

## Comparing `gapps-mod-0.0.4.tar` & `gapps-mod-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 18:28:07.702495 gapps-mod-0.0.4/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:50:00.000000 gapps-mod-0.0.4/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-11 18:28:07.702495 gapps-mod-0.0.4/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       68 2022-03-13 21:47:12.000000 gapps-mod-0.0.4/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    15295 2023-07-11 18:27:07.000000 gapps-mod-0.0.4/gapps.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 18:28:07.702495 gapps-mod-0.0.4/gapps_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      224 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      102 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-13 21:42:41.000000 gapps-mod-0.0.4/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      838 2023-07-11 18:28:07.706496 gapps-mod-0.0.4/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 21:42:00.000000 gapps-mod-0.0.4/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 18:30:49.808697 gapps-mod-0.0.5/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:50:00.000000 gapps-mod-0.0.5/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-11 18:30:49.812697 gapps-mod-0.0.5/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       68 2022-03-13 21:47:12.000000 gapps-mod-0.0.5/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    15290 2023-07-11 18:30:06.000000 gapps-mod-0.0.5/gapps.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 18:30:49.808697 gapps-mod-0.0.5/gapps_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-11 18:30:49.000000 gapps-mod-0.0.5/gapps_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      224 2023-07-11 18:30:49.000000 gapps-mod-0.0.5/gapps_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 18:30:49.000000 gapps-mod-0.0.5/gapps_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      102 2023-07-11 18:30:49.000000 gapps-mod-0.0.5/gapps_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-07-11 18:30:49.000000 gapps-mod-0.0.5/gapps_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-13 21:42:41.000000 gapps-mod-0.0.5/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      838 2023-07-11 18:30:49.812697 gapps-mod-0.0.5/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 21:42:00.000000 gapps-mod-0.0.5/setup.py
```

### Comparing `gapps-mod-0.0.4/LICENSE` & `gapps-mod-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gapps-mod-0.0.4/PKG-INFO` & `gapps-mod-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapps-mod
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper for some Google App functionality (Sheets and email mostly)
 Home-page: https://github.com/ejohnfel/gapps
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/gapps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gapps-mod-0.0.4/gapps.py` & `gapps-mod-0.0.5/gapps.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 #
 # Variables
 #
 
 # Version Stuff
-VERSION=(0,0,4)
+VERSION=(0,0,5)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Config Location (if in Use)
 GappsConfigSection = "gapps"
 GappsCredsValue = "gappscreds"
 GappsTokenValue = "gappstoken"
 
@@ -109,17 +109,17 @@
 	Scopes = list(scopelist)
 
 	return scopelist
 
 def ReAuthToken(credfile,scopes):
 	"""Reauthorize a Refresh Token"""
 
-	// This will activate a Lynx like web browser
-	// If using the supplied reauth URL, the browser being used must be running on the host
-	// Where this script is running
+	# This will activate a Lynx like web browser
+	# If using the supplied reauth URL, the browser being used must be running on the host
+	# Where this script is running
 
 	flow = InstalledAppFlow.from_client_secrets_file(credfile,scopes)
 	creds = flow.run_local_server(port=0)
 
 	return creds
 
 #
@@ -142,18 +142,18 @@
 		creds = Creds = Credentials.from_authorized_user_file(tokenfile,scopes)
 
 	if not creds or not creds.valid:
 		if creds and creds.expired and creds.refresh_token:
 			try:
 				creds.refresh(Request())
 			except Exception as err:
-				// This will create an interactive Lynx like web browser
+				# This will create an interactive Lynx like web browser
 				creds = Creds = ReAuthToken(credfile,scopes)
 		else:
-			// This will create an interactive Lynx like web browser
+			# This will create an interactive Lynx like web browser
 			creds = Creds = ReAuthToken(credfile,scopes)
 
 		with open(tokenfile,"w") as token:
 			token.write(creds.to_json())
 
 	Service = build(svc_name,svc_version,credentials=creds)
```

### Comparing `gapps-mod-0.0.4/gapps_mod.egg-info/PKG-INFO` & `gapps-mod-0.0.5/gapps_mod.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapps-mod
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper for some Google App functionality (Sheets and email mostly)
 Home-page: https://github.com/ejohnfel/gapps
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/gapps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gapps-mod-0.0.4/setup.cfg` & `gapps-mod-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = gapps-mod
-version = 0.0.4
+version = 0.0.5
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = A wrapper for some Google App functionality (Sheets and email mostly)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/gapps
 project_urls =
```

