# Comparing `tmp/starfish_library-1.4.22.tar.gz` & `tmp/starfish_library-1.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfish_library-1.4.22.tar", last modified: Thu Mar 30 06:25:18 2023, max compression
+gzip compressed data, was "starfish_library-1.4.23.tar", last modified: Tue Jul 11 02:35:43 2023, max compression
```

## Comparing `starfish_library-1.4.22.tar` & `starfish_library-1.4.23.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 06:25:18.228625 starfish_library-1.4.22/
--rw-rw-rw-   0        0        0        0 2022-10-12 07:46:00.000000 starfish_library-1.4.22/LICENSE
--rw-rw-rw-   0        0        0      175 2023-03-30 06:25:18.227125 starfish_library-1.4.22/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-10-19 05:15:42.000000 starfish_library-1.4.22/README.md
--rw-rw-rw-   0        0        0       42 2023-03-30 06:25:18.229125 starfish_library-1.4.22/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-03-30 06:24:46.000000 starfish_library-1.4.22/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:25:18.196627 starfish_library-1.4.22/starfish_library/
--rw-rw-rw-   0        0        0      234 2022-10-19 03:49:55.000000 starfish_library-1.4.22/starfish_library/__init__.py
--rw-rw-rw-   0        0        0    11970 2023-03-30 06:23:25.000000 starfish_library-1.4.22/starfish_library/common.py
--rw-rw-rw-   0        0        0       31 2022-10-06 02:51:09.000000 starfish_library-1.4.22/starfish_library/common_db_setting.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:25:18.222626 starfish_library-1.4.22/starfish_library.egg-info/
--rw-rw-rw-   0        0        0      175 2023-03-30 06:25:17.000000 starfish_library-1.4.22/starfish_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-03-30 06:25:18.000000 starfish_library-1.4.22/starfish_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 06:25:17.000000 starfish_library-1.4.22/starfish_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-30 06:25:17.000000 starfish_library-1.4.22/starfish_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 02:35:43.881425 starfish_library-1.4.23/
+-rw-rw-rw-   0        0        0        0 2022-10-12 07:46:00.000000 starfish_library-1.4.23/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-07-11 02:35:43.880925 starfish_library-1.4.23/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-10-19 05:15:42.000000 starfish_library-1.4.23/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 02:35:43.881924 starfish_library-1.4.23/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-07-11 02:35:34.000000 starfish_library-1.4.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:35:43.867425 starfish_library-1.4.23/starfish_library/
+-rw-rw-rw-   0        0        0      234 2022-10-19 03:49:55.000000 starfish_library-1.4.23/starfish_library/__init__.py
+-rw-rw-rw-   0        0        0    11971 2023-07-11 02:34:41.000000 starfish_library-1.4.23/starfish_library/common.py
+-rw-rw-rw-   0        0        0       31 2022-10-06 02:51:09.000000 starfish_library-1.4.23/starfish_library/common_db_setting.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:35:43.880424 starfish_library-1.4.23/starfish_library.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-07-11 02:35:43.000000 starfish_library-1.4.23/starfish_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-11 02:35:43.000000 starfish_library-1.4.23/starfish_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 02:35:43.000000 starfish_library-1.4.23/starfish_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 02:35:43.000000 starfish_library-1.4.23/starfish_library.egg-info/top_level.txt
```

### Comparing `starfish_library-1.4.22/starfish_library/common.py` & `starfish_library-1.4.23/starfish_library/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     return token
 
 
 # MCCに紐づくアカウントIDの取得
 # token = generate_yahoo_token()
 def get_yahoo_account_ids(token):
     serviceType = 'AccountLinkService/get'
-    url = 'https://ads-search.yahooapis.jp/api/v6/' + serviceType
+    url = 'https://ads-search.yahooapis.jp/api/v11/' + serviceType
 
     request_header = {
         'accept': 'application/json',
         'Content-Type': 'application/json',
         'Authorization': f'Bearer {token}'
     }
```

