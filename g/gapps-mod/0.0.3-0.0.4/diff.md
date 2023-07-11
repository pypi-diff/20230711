# Comparing `tmp/gapps-mod-0.0.3.tar.gz` & `tmp/gapps-mod-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/gapps/dist/tmpr7tt80v8/gapps-mod-0.0.3.tar", last modified: Sun Mar 13 23:22:58 2022, max compression
+gzip compressed data, was "gapps-mod-0.0.4.tar", last modified: Tue Jul 11 18:28:07 2023, max compression
```

## Comparing `gapps-mod-0.0.3.tar` & `gapps-mod-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    14798 2022-03-13 23:22:09.000000 gapps-mod-0.0.3/gapps.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:50:00.000000 gapps-mod-0.0.3/LICENSE
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/gapps_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/gapps_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/gapps_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      224 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/gapps_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      102 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/gapps_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      638 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/gapps_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       68 2022-03-13 21:47:12.000000 gapps-mod-0.0.3/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-13 21:42:41.000000 gapps-mod-0.0.3/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      638 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      838 2022-03-13 23:22:58.000000 gapps-mod-0.0.3/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 21:42:00.000000 gapps-mod-0.0.3/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 18:28:07.702495 gapps-mod-0.0.4/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:50:00.000000 gapps-mod-0.0.4/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-11 18:28:07.702495 gapps-mod-0.0.4/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       68 2022-03-13 21:47:12.000000 gapps-mod-0.0.4/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    15295 2023-07-11 18:27:07.000000 gapps-mod-0.0.4/gapps.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-11 18:28:07.702495 gapps-mod-0.0.4/gapps_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      224 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      102 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-07-11 18:28:07.000000 gapps-mod-0.0.4/gapps_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-13 21:42:41.000000 gapps-mod-0.0.4/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      838 2023-07-11 18:28:07.706496 gapps-mod-0.0.4/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 21:42:00.000000 gapps-mod-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gapps-mod-0.0.3/gapps.py` & `gapps-mod-0.0.4/gapps.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 #
 # Variables
 #
 
 # Version Stuff
-VERSION = (0,0,3)
+VERSION=(0,0,4)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Config Location (if in Use)
 GappsConfigSection = "gapps"
 GappsCredsValue = "gappscreds"
 GappsTokenValue = "gappstoken"
 
@@ -106,14 +106,26 @@
 			else:
 				scopelist.append(GappsAppScopes[scope])
 
 	Scopes = list(scopelist)
 
 	return scopelist
 
+def ReAuthToken(credfile,scopes):
+	"""Reauthorize a Refresh Token"""
+
+	// This will activate a Lynx like web browser
+	// If using the supplied reauth URL, the browser being used must be running on the host
+	// Where this script is running
+
+	flow = InstalledAppFlow.from_client_secrets_file(credfile,scopes)
+	creds = flow.run_local_server(port=0)
+
+	return creds
+
 #
 # Get Service Function (The Main Function)
 #
 
 # Get Google Service (for email, spreadsheets, etc)
 def GetService(scopes=None,credfile='credentials.json',tokenfile='token.json',svc_name=ServiceNames["gmail"],svc_version=ServiceVersion):
 	global Creds, Service, Scopes
@@ -127,18 +139,22 @@
 	DbgMsg(scopes)
 
 	if os.path.exists(tokenfile):
 		creds = Creds = Credentials.from_authorized_user_file(tokenfile,scopes)
 
 	if not creds or not creds.valid:
 		if creds and creds.expired and creds.refresh_token:
-			creds.refresh(Request())
+			try:
+				creds.refresh(Request())
+			except Exception as err:
+				// This will create an interactive Lynx like web browser
+				creds = Creds = ReAuthToken(credfile,scopes)
 		else:
-			flow = InstalledAppFlow.from_client_secrets_file(credfile,scopes)
-			creds = Creds = flow.run_local_server(port=0)
+			// This will create an interactive Lynx like web browser
+			creds = Creds = ReAuthToken(credfile,scopes)
 
 		with open(tokenfile,"w") as token:
 			token.write(creds.to_json())
 
 	Service = build(svc_name,svc_version,credentials=creds)
 
 	return Service
```

### Comparing `gapps-mod-0.0.3/LICENSE` & `gapps-mod-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gapps-mod-0.0.3/setup.cfg` & `gapps-mod-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = gapps-mod
-version = 0.0.3
+version = 0.0.4
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = A wrapper for some Google App functionality (Sheets and email mostly)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/gapps
 project_urls =
```

