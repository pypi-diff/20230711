# Comparing `tmp/whois21-1.2.0.tar.gz` & `tmp/whois21-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois21-1.2.0.tar", last modified: Thu Dec  1 18:55:09 2022, max compression
+gzip compressed data, was "whois21-1.2.1.tar", last modified: Tue Jul 11 15:49:38 2023, max compression
```

## Comparing `whois21-1.2.0.tar` & `whois21-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 18:55:09.743024 whois21-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-12-01 18:55:06.000000 whois21-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-01 18:55:06.000000 whois21-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8274 2022-12-01 18:55:09.743024 whois21-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7766 2022-12-01 18:55:06.000000 whois21-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 18:55:09.743024 whois21-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-01 18:55:06.000000 whois21-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 18:55:09.743024 whois21-1.2.0/whois21/
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2022-12-01 18:55:06.000000 whois21-1.2.0/whois21/API.py
--rw-r--r--   0 runner    (1001) docker     (122)     6858 2022-12-01 18:55:06.000000 whois21-1.2.0/whois21/ASN.py
--rw-r--r--   0 runner    (1001) docker     (122)     6544 2022-12-01 18:55:06.000000 whois21-1.2.0/whois21/DNS.py
--rw-r--r--   0 runner    (1001) docker     (122)    22952 2022-12-01 18:55:06.000000 whois21-1.2.0/whois21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2022-12-01 18:55:06.000000 whois21-1.2.0/whois21/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2022-12-01 18:55:06.000000 whois21-1.2.0/whois21/vcard-map.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 18:55:09.743024 whois21-1.2.0/whois21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8274 2022-12-01 18:55:09.000000 whois21-1.2.0/whois21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      334 2022-12-01 18:55:09.000000 whois21-1.2.0/whois21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 18:55:09.000000 whois21-1.2.0/whois21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-01 18:55:09.000000 whois21-1.2.0/whois21.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2022-12-01 18:55:09.000000 whois21-1.2.0/whois21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-12-01 18:55:09.000000 whois21-1.2.0/whois21.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:49:38.614425 whois21-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:49:28.000000 whois21-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 15:49:28.000000 whois21-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-11 15:49:38.614425 whois21-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-11 15:49:28.000000 whois21-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-11 15:49:28.000000 whois21-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:49:38.614425 whois21-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:49:38.614425 whois21-1.2.1/whois21/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/ASN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/DNS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/vcard-map.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:49:38.614425 whois21-1.2.1/whois21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/top_level.txt
```

### Comparing `whois21-1.2.0/LICENSE` & `whois21-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whois21-1.2.0/PKG-INFO` & `whois21-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: whois21
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple and easy to use Python package that lets you query whois/RDAP information of a domain/IP.
-Home-page: https://github.com/MPCodeWriter21/whois21
-Author: CodeWriter21
-Author-email: CodeWriter21@gmail.com
+Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/MPCodeWriter21/whois21
+Project-URL: Donations, https://github.com/MPCodeWriter21/whois21/blob/master/DONATE.md
+Project-URL: Source, https://github.com/MPCodeWriter21/whois21
 Keywords: python,python3,CodeWriter21,WHOIS,whois21,RDAP,Registration Data Access Protocol,DNS,ASN
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 whois21
 =====
 
 ![version](https://img.shields.io/pypi/v/whois21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/whois21)
@@ -54,15 +57,15 @@
 # And install it using this command
 pip install whois21-x.x.x.tar.gz
 ```
 
 Or you can clone [the repository](https://github.com/MPCodeWriter21/whois21) and run:
 
 ```shell
-python setup.py install
+python -m build .
 ```
 
 ### Dependencies
 
 + [requests](https://requests.readthedocs.io/en/master/): Used for:
     - Downloading list of whois and RDAP servers.
     - Downloading RDAP information.
@@ -89,17 +92,17 @@
     - Type hinting.
 + [re](https://docs.python.org/3/library/re.html) (A core python module): Used for:
     - Matching date-time strings with regular expressions.
 
 Changes
 -------
 
-### 1.2.0
+### 1.2.1
 
-Added ip-api.com API support.
+Switched from `setup.py` to `pyproject.toml`.
 
 Usage Examples:
 ---------------
 
 ### CLI Examples
 
 + Example 1: Query whois information of google.com
```

### Comparing `whois21-1.2.0/README.md` & `whois21-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # And install it using this command
 pip install whois21-x.x.x.tar.gz
 ```
 
 Or you can clone [the repository](https://github.com/MPCodeWriter21/whois21) and run:
 
 ```shell
-python setup.py install
+python -m build .
 ```
 
 ### Dependencies
 
 + [requests](https://requests.readthedocs.io/en/master/): Used for:
     - Downloading list of whois and RDAP servers.
     - Downloading RDAP information.
@@ -76,17 +76,17 @@
     - Type hinting.
 + [re](https://docs.python.org/3/library/re.html) (A core python module): Used for:
     - Matching date-time strings with regular expressions.
 
 Changes
 -------
 
-### 1.2.0
+### 1.2.1
 
-Added ip-api.com API support.
+Switched from `setup.py` to `pyproject.toml`.
 
 Usage Examples:
 ---------------
 
 ### CLI Examples
 
 + Example 1: Query whois information of google.com
```

### Comparing `whois21-1.2.0/whois21/API.py` & `whois21-1.2.1/whois21/API.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.0/whois21/ASN.py` & `whois21-1.2.1/whois21/ASN.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.0/whois21/DNS.py` & `whois21-1.2.1/whois21/DNS.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.0/whois21/__init__.py` & `whois21-1.2.1/whois21/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 # whois21.__init__.py
 
-import re
 import os
+import re
 import json
 import socket
-
+from typing import Set, Union, Optional, Sequence
 from datetime import datetime
-from typing import Union, Set, Sequence
 
 import log21
 import requests
 import importlib_resources
 
-from whois21.ASN import download_asn_json, get_asn_dict, get_asn_services, ip_registration_data_lookup_, \
-    ip_registration_data_lookup, validate_ip
-from whois21.DNS import download_dns_json, get_dns_dict, get_dns_services, domain_registration_data_lookup_, \
-    domain_registration_data_lookup
 from whois21.API import lookup_ip_ip_api, batch_lookup_ip_ip_api
+from whois21.ASN import (validate_ip, get_asn_dict, get_asn_services, download_asn_json,
+                         ip_registration_data_lookup, ip_registration_data_lookup_)
+from whois21.DNS import (get_dns_dict, get_dns_services, download_dns_json,
+                         domain_registration_data_lookup,
+                         domain_registration_data_lookup_)
 
 __version__ = '1.2.0'
 __github__ = 'https://github.com/MPCodeWriter21/whois21'
 __author__ = 'CodeWriter21'
 __email__ = 'CodeWriter21@gmail.com'
 __license__ = 'Apache License 2.0'
 
-__all__ = ['__version__', '__github__', '__author__', '__email__', '__license__', 'download_asn_json',
-           'get_asn_dict', 'get_asn_services', 'ip_registration_data_lookup_', 'ip_registration_data_lookup',
-           'download_dns_json', 'get_dns_dict', 'get_dns_services', 'domain_registration_data_lookup_',
-           'domain_registration_data_lookup', 'validate_ip', 'WHOIS', 'registration_data_lookup', 'get_whois_servers',
-           'whois_servers', 'vcard_map']
+__all__ = [
+    '__version__', '__github__', '__author__', '__email__', '__license__',
+    'download_asn_json', 'get_asn_dict', 'get_asn_services',
+    'ip_registration_data_lookup_', 'ip_registration_data_lookup', 'download_dns_json',
+    'get_dns_dict', 'get_dns_services', 'domain_registration_data_lookup_',
+    'domain_registration_data_lookup', 'validate_ip', 'WHOIS',
+    'registration_data_lookup', 'get_whois_servers', 'whois_servers', 'vcard_map',
+    'lookup_ip_ip_api', 'batch_lookup_ip_ip_api'
+]
 
 LRED = log21.get_color('Light Red')
 LGREEN = log21.get_color('Light Green')
 LBLUE = log21.get_color('Light Blue')
 LCYAN = log21.get_color('Light Cyan')
 RED = log21.get_color('Red')
 GREEN = log21.get_color('Green')
 BLUE = log21.get_color('Blue')
 CYAN = log21.get_color('Cyan')
 RESET = log21.get_color('Reset')
 
 
-def download_whois_servers(path: Union[str, os.PathLike] = None) -> str:
-    """
-    Downloads the whois whois-servers.txt file from https://www.nirsoft.net/whois-servers.txt.
+def download_whois_servers(path: Optional[Union[str, os.PathLike]] = None) -> str:
+    """Downloads the whois whois-servers.txt file from
+    https://www.nirsoft.net/whois-servers.txt.
 
     :param path: The path to the whois file.
     :return: The path to the downloaded file.
     """
     if not path:
-        path = importlib_resources.files('whois21') / 'whois-servers.txt'
+        path = str(importlib_resources.files('whois21') / 'whois-servers.txt')
 
     if not os.path.exists(path):
         os.makedirs(os.path.dirname(path), exist_ok=True)
 
-    log21.debug(f'Downloading {LGREEN}whois-servers.txt{RESET} file to `{BLUE}{path}{RESET}`')
+    log21.debug(
+        f'Downloading {LGREEN}whois-servers.txt{RESET} file to `{BLUE}{path}{RESET}`'
+    )
 
     with open(path, 'wb') as file:
         file.write(requests.get('https://www.nirsoft.net/whois-servers.txt').content)
 
     return str(path)
 
 
-def get_whois_servers(force_download: bool = False, path: Union[str, os.PathLike] = None):
-    """
-    Returns a dictionary of the whois-servers.txt file.
+def get_whois_servers(
+    force_download: bool = False, path: Optional[Union[str, os.PathLike]] = None
+):
+    """Returns a dictionary of the whois-servers.txt file.
 
     :param force_download: If True, the whois-servers.txt file will be downloaded again.
     :param path: The path to the whois-servers.txt file.
     :return: A dictionary of the whois-servers.txt file.
     """
     if not path:
-        path = importlib_resources.files('whois21') / 'whois-servers.txt'
+        path = str(importlib_resources.files('whois21') / 'whois-servers.txt')
 
     if not os.path.exists(path) or force_download:
         download_whois_servers(path)
 
     data = dict()
     with open(path, 'r') as file:
         for line in file:
@@ -85,24 +92,27 @@
             data[key] = value.strip(' \n')
 
     return data
 
 
 whois_servers: dict = {
     'ABUSE_HOST': 'whois.abuse.net',
-    'LNICHOST': 'whois.lacnic.net',  # Types of queries: POCs, ownerid, CIDR blocks, IP and AS numbers.
+    # Types of queries: POCs, ownerid, CIDR blocks, IP and AS numbers.
+    'LNICHOST': 'whois.lacnic.net',  
     'ai': {'whois.nic.ai'},
     'app': {'whois.nic.google'},
     'ar': {'whois.nic.ar'},
     'by': {'whois.cctld.by'},
     'ca': {'whois.ca.fury.ca'},
     'chat': {'whois.nic.chat'},
     'cl': {'whois.nic.cl'},
-    'com': {'whois.crsnic.net', 'WHOIS.ENOM.COM', 'whois.joker.com', 'whois.corporatedomains.com',
-            'whois.verisign-grs.com'},
+    'com': {
+        'whois.crsnic.net', 'WHOIS.ENOM.COM', 'whois.joker.com',
+        'whois.corporatedomains.com', 'whois.verisign-grs.com'
+    },
     'cr': {'whois.nic.cr'},
     'edu': {'whois.crsnic.net', 'whois.educause.net'},
     'de': {'whois.denic.de'},
     'dev': {'whois.nic.google'},
     'do': {'whois.nic.do'},
     'games': {'whois.nic.games'},
     'gov': {'whois.nic.gov'},
@@ -123,15 +133,16 @@
     'market': {'whois.nic.market'},
     'money': {'whois.nic.money'},
     'mx': {'whois.mx'},
     'net': {'whois.crsnic.net'},
     'nl': {'whois.domain-registry.nl'},
     'online': {'whois.nic.online'},
     'ooo': {'whois.nic.ooo'},
-    'org': {'whois.publicdomainregistry.com', 'whois.gandi.net', 'whois.markmonitor.com'},
+    'org':
+    {'whois.publicdomainregistry.com', 'whois.gandi.net', 'whois.markmonitor.com'},
     'page': {'whois.nic.page'},
     'pe': {'kero.yachay.pe'},
     'website': {'whois.nic.website'},
     'za': {'whois.registry.net.za'}
 }
 
 for _key, _value in get_whois_servers().items():
@@ -147,28 +158,41 @@
     __error: str = ''
     __raw: bytes = b''
     __servers: Set[str] = set()
     __whois_data: dict = {}
     __rdap_data: dict = {}
     timeout: int = 10
 
-    def __init__(self, domain: str, servers: Sequence[str] = None, timeout: int = 10, use_rdap: bool = True,
-                 force_rdap: bool = False):
+    def __init__(
+        self,
+        domain: str,
+        servers: Optional[Sequence[str]] = None,
+        timeout: int = 10,
+        use_rdap: bool = True,
+        force_rdap: bool = False
+    ):
         self.whois(domain, servers, timeout, use_rdap, force_rdap)
 
-    def whois(self, domain: str, servers: Sequence[str] = None, timeout: int = 10, use_rdap: bool = True,
-              force_rdap: bool = False):
-        """
-        Queries the whois server for the domain.
+    def whois(
+        self,
+        domain: str,
+        servers: Optional[Sequence[str]] = None,
+        timeout: int = 10,
+        use_rdap: bool = True,
+        force_rdap: bool = False
+    ):
+        """Queries the whois server for the domain.
 
         :param domain: The domain/ip to query.
         :param servers: The servers to use.
         :param timeout: The timeout in seconds.
-        :param use_rdap: If True, the RDAP server will be used if the whois servers don't respond.
-        :param force_rdap: If True, the RDAP server will be used even if the whois servers respond.
+        :param use_rdap: If True, the RDAP server will be used if the
+                whois servers don't respond.
+        :param force_rdap: If True, the RDAP server will be used even if
+                the whois servers respond.
         """
         self.__domain = domain.lower()
         self.__success = False
         self.__servers = set(servers) if servers else set()
         self.__whois_data = {}
         self.timeout = timeout
         self.__error = ''
@@ -181,35 +205,44 @@
             self.__rdap()
 
         self.__set_attrs()
 
     def __set_attrs(self):
         # Save the whois information in object attributes.
         self.registry_domain_id = self.__whois_data.get('REGISTRY DOMAIN ID', '')
-        self.registrar_whois_server = self.__whois_data.get('REGISTRAR WHOIS SERVER', '')
+        self.registrar_whois_server = self.__whois_data.get(
+            'REGISTRAR WHOIS SERVER', ''
+        )
         self.registrar_url = self.__whois_data.get('REGISTRAR URL', '')
         self.updated_date = self.__whois_data.get('UPDATED DATE', '')
         self.creation_date = self.__whois_data.get('CREATION DATE', '')
-        self.expires_date = self.__whois_data.get('REGISTRY EXPIRY DATE', '') or \
-                            self.__whois_data.get('REGISTRAR REGISTRATION EXPIRATION DATE', '')
+        self.expires_date = (
+            self.__whois_data.get('REGISTRY EXPIRY DATE', '')
+            or self.__whois_data.get('REGISTRAR REGISTRATION EXPIRATION DATE', '')
+        )
         self.registrar_name = self.__whois_data.get('REGISTRAR', '')
         self.registrar_iana_id = self.__whois_data.get('REGISTRAR IANA ID', '')
-        self.registrar_abuse_contact_email = self.__whois_data.get('REGISTRAR ABUSE CONTACT EMAIL', '')
-        self.registrar_abuse_contact_phone = self.__whois_data.get('REGISTRAR ABUSE CONTACT PHONE', '')
+        self.registrar_abuse_contact_email = self.__whois_data.get(
+            'REGISTRAR ABUSE CONTACT EMAIL', ''
+        )
+        self.registrar_abuse_contact_phone = self.__whois_data.get(
+            'REGISTRAR ABUSE CONTACT PHONE', ''
+        )
         self.status = self.__whois_data.get('DOMAIN STATUS', [])
         self.name_servers = self.__whois_data.get('NAME SERVER', [])
 
         def parse_time(date_time: str) -> Union[datetime, None]:
-            """
-            Parses a date time string.
+            """Parses a date time string.
 
             :param date_time: The date time string.
             :return: The parsed date time.
             """
-            result = re.findall(r'(\d{4}\-\d{2}\-\d{2}).(\d{2}:\d{2}:\d{2})*', date_time)
+            result = re.findall(
+                r'(\d{4}\-\d{2}\-\d{2}).(\d{2}:\d{2}:\d{2})*', date_time
+            )
             if result:
                 return datetime.strptime(' '.join(result[0]), '%Y-%m-%d %H:%M:%S')
             return None
 
         # Convert the dates to datetime objects.
         if self.updated_date:
             self.updated_date = parse_time(self.updated_date)
@@ -237,58 +270,75 @@
             return
 
         self.__success = True
         self.__error = ''
         log21.debug(f'{LGREEN}WHOIS data successfully parsed.{RESET}')
 
     def __whois_iana(self):
-        # Send a query to the whois.iana.org server to find the whois server for the domain.
+        # Send a query to the whois.iana.org server to find the whois server for the
+        # domain.
         # Create a socket connection to the whois.iana.org server.
         log21.debug(f'Connecting to {LBLUE}whois.iana.org:43{RESET}...')
         try:
             sock = socket.create_connection(('whois.iana.org', 43))
             sock.settimeout(self.timeout)
         except socket.error as e:
-            log21.debug(f'Error connecting to "{RED}whois.iana.org:43{RESET}": '
-                        f'{LRED}{e.__class__.__name__}: {e}{RESET}')
-            self.__error = f'Error connecting "to whois.iana.org:43": {e.__class__.__name__}: {e}'
+            log21.debug(
+                f'Error connecting to "{RED}whois.iana.org:43{RESET}": '
+                f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+            )
+            self.__error = (
+                'Error connecting "to whois.iana.org:43": '
+                f'{e.__class__.__name__}: {e}'
+            )
             return
         # Send the domain name to the whois.iana.org server.
         log21.debug(f'Sending query for {LCYAN}{self.domain}{RESET}...')
         try:
             sock.send(self.domain.encode('utf-8') + b'\r\n')
         except socket.error as e:
-            log21.debug(f'Error sending query to "{RED}whois.iana.org:43{RESET}": '
-                        f'{LRED}{e.__class__.__name__}: {e}{RESET}')
-            self.__error = f'Error sending query to "whois.iana.org:43": {e.__class__.__name__}: {e}'
+            log21.debug(
+                f'Error sending query to "{RED}whois.iana.org:43{RESET}": '
+                f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+            )
+            self.__error = (
+                'Error sending query to "whois.iana.org:43": '
+                f'{e.__class__.__name__}: {e}'
+            )
             return
         # Receive the raw data from the whois.iana.org server.
         self.__raw = b''
         log21.debug('Receiving data...')
         try:
             while True:
                 data = sock.recv(4096)
                 if not data:
                     break
                 self.__raw += data
         except socket.error as e:
-            log21.debug(f'Error receiving data from "{RED}whois.iana.org:43{RESET}": '
-                        f'{LRED}{e.__class__.__name__}: {e}{RESET}')
-            self.__error = f'Error receiving data from "whois.iana.org:43": {e.__class__.__name__}: {e}'
+            log21.debug(
+                f'Error receiving data from "{RED}whois.iana.org:43{RESET}": '
+                f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+            )
+            self.__error = (
+                'Error receiving data from "whois.iana.org:43": '
+                f'{e.__class__.__name__}: {e}'
+            )
             return
         sock.close()
 
         # Checks if we received any data from the whois.iana.org server.
         if not self.__raw:
             log21.debug(f'{LRED}No data received.{RESET}')
             self.__error = 'No data received from whois.iana.org.'
             return
 
         log21.debug('Parsing data: Searching for whois server...')
-        # Parse the raw data from the whois.iana.org server and extract the whois server.
+        # Parse the raw data from the whois.iana.org server and extract the whois
+        # server.
         for line in self.__raw.decode('utf-8').split('\n'):
             if line.startswith('whois:'):
                 self.__servers.add(line[6:].strip())
                 break
         else:
             log21.debug(f'{LRED}No whois server found.{RESET}')
             self.__error = 'No whois server found.'
@@ -314,49 +364,65 @@
         for whois_server in self.__servers:
             # Create a socket connection to the whois server.
             log21.debug(f'Connecting to {LBLUE}{whois_server}{RESET}...')
             try:
                 sock = socket.create_connection((whois_server, 43))
                 sock.settimeout(self.timeout)
             except socket.error as e:
-                log21.debug(f'Error connecting to "{RED}{whois_server}{RESET}": '
-                            f'{LRED}{e.__class__.__name__}: {e}{RESET}')
-                self.__error = f'Error connecting to "{whois_server}": {e.__class__.__name__}: {e}'
+                log21.debug(
+                    f'Error connecting to "{RED}{whois_server}{RESET}": '
+                    f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                )
+                self.__error = (
+                    f'Error connecting to "{whois_server}": '
+                    f'{e.__class__.__name__}: {e}'
+                )
                 continue
             # Send the domain name to the whois server.
             log21.debug(f'Sending query for {LCYAN}{self.domain}{RESET}...')
             try:
                 sock.send(self.domain.encode('utf-8') + b'\r\n')
             except socket.error as e:
-                log21.debug(f'Error sending query to "{RED}{whois_server}{RESET}": '
-                            f'{LRED}{e.__class__.__name__}: {e}{RESET}')
-                self.__error = f'Error sending query to "{whois_server}": {e.__class__.__name__}: {e}'
+                log21.debug(
+                    f'Error sending query to "{RED}{whois_server}{RESET}": '
+                    f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                )
+                self.__error = (
+                    f'Error sending query to "{whois_server}": '
+                    f'{e.__class__.__name__}: {e}'
+                )
                 continue
             # Receive the raw whois data from the whois server.
             self.__raw = b''
             log21.debug('Receiving data...')
             try:
                 while True:
                     data = sock.recv(4096)
                     if not data:
                         break
                     self.__raw += data
             except socket.error as e:
-                log21.debug(f'Error receiving data from "{RED}{whois_server}{RESET}": '
-                            f'{LRED}{e.__class__.__name__}: {e}{RESET}')
-                self.__error = f'Error receiving data from "{whois_server}": {e.__class__.__name__}: {e}'
+                log21.debug(
+                    f'Error receiving data from "{RED}{whois_server}{RESET}": '
+                    f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                )
+                self.__error = (
+                    f'Error receiving data from "{whois_server}": '
+                    f'{e.__class__.__name__}: {e}'
+                )
                 continue
             sock.close()
 
             # Checks if we received any data from the whois server.
             if not self.__raw:
                 log21.debug(f'No data received from {RED}{whois_server}{RESET}.')
                 self.__error = f'No data received from {whois_server}.'
                 continue
-            # Parse the raw whois data from the whois server and extract the whois information.
+            # Parse the raw whois data from the whois server and extract the whois
+            # information.
             log21.debug('Parsing data...')
             self.__whois_data = {}
             i = 0
             lines = self.__raw.decode('utf-8').split('\n')
             while i < len(lines):
                 line = lines[i]
                 if line.startswith('%') or line.startswith('#'):
@@ -375,16 +441,18 @@
                             i = j
                     if key.strip().upper() not in self.__whois_data:
                         self.__whois_data[key.strip().upper()] = value.strip()
                     else:
                         if isinstance(self.__whois_data[key.strip().upper()], list):
                             self.__whois_data[key.strip().upper()].append(value.strip())
                         elif isinstance(self.__whois_data[key.strip().upper()], str):
-                            self.__whois_data[key.strip().upper()] = [self.__whois_data[key.strip().upper()],
-                                                                      value.strip()]
+                            self.__whois_data[key.strip().upper()] = [
+                                self.__whois_data[key.strip().upper()],
+                                value.strip()
+                            ]
                 i += 1
 
             if not self.__whois_data:
                 log21.debug(f'{LRED}No data found.{RESET}')
                 self.__error = 'No whois data found.'
                 continue
 
@@ -399,16 +467,22 @@
 
     def __rdap(self):
         # Get the rdap information for the domain.
         log21.debug('Getting rdap information...')
         try:
             self.__rdap_data = registration_data_lookup(self.domain)
         except Exception as e:
-            log21.debug(f'{LRED}Error{RESET} getting rdap information: {e.__class__.__name__}: {e}')
-            self.__error = f'Error getting rdap information: {e.__class__.__name__}: {e}'
+            log21.debug(
+                f'{LRED}Error{RESET} getting rdap information: '
+                f'{e.__class__.__name__}: {e}'
+            )
+            self.__error = (
+                'Error getting rdap information: '
+                f'{e.__class__.__name__}: {e}'
+            )
             return
 
         if not self.__rdap_data:
             log21.debug(f'{LRED}No data found.{RESET}')
             self.__error = 'No rdap data found.'
             return
 
@@ -418,17 +492,16 @@
             self.__error = 'Error found in rdap data.'
             return
 
         self.__parse_rdap_data()
         return
 
     def __parse_rdap_data(self):
-        """
-        Parses the RDAP data and puts some information in whois_data dictionary.
-        """
+        """Parses the RDAP data and puts some information in whois_data
+        dictionary."""
 
         # Parse the rdap data and extract the whois information.
         log21.debug('Parsing rdap data...')
         self.__whois_data = {
             'REGISTRAR WHOIS SERVER': self.__rdap_data.get('port43'),
             'REGISTRY DOMAIN ID': self.__rdap_data.get('handle')
         }
@@ -479,15 +552,16 @@
                 # "publicIds": [
                 #     {
                 #         "type": "IANA Registrar ID",
                 #         "identifier": "292"
                 #     }
                 # ]
                 if 'type' in public_id and 'identifier' in public_id:
-                    self.__whois_data[public_id.get('type').upper()] = public_id.get('identifier')
+                    self.__whois_data[public_id.get('type').upper()
+                                      ] = public_id.get('identifier')
 
             # Handle vcards
             # Reference: https://www.rfc-editor.org/rfc/rfc6350.txt
             # Reference: https://en.wikipedia.org/wiki/VCard
             # vcardArray Example:
             # "vcardArray": [
             #                   "vcard",
@@ -564,16 +638,16 @@
         return self.__whois_data.get(key.upper(), default)
 
     def __getitem__(self, key: str):
         return self.__whois_data[key.upper()]
 
 
 def registration_data_lookup(domain: str, timeout: int = 10) -> dict:
-    """
-    Lookup the registration data for a domain/ip.
+    """Lookup the registration data for a domain/ip.
+
     :param domain: The domain/ip to lookup.
     :param timeout: The timeout for the socket connection.
     :return: A WHOIS object.
     """
     if validate_ip(domain):
         return ip_registration_data_lookup(domain, timeout)
     else:
```

### Comparing `whois21-1.2.0/whois21/__main__.py` & `whois21-1.2.1/whois21/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # whois21.__main__.py
 
 import os
 import json
 
 import log21
+
 import whois21
 
 
 def get_filename(directory: str, domain: str, format_: str = 'json') -> str:
-    """
-    Gets a filename to store the registration data in.
+    """Gets a filename to store the registration data in.
 
     :param directory: The directory to store the registration data in.
     :param domain: The domain to get the name for.
     :param format_: The format to store the registration data in.
     :return: The filename.
     """
     name = domain + '.' + format_
@@ -30,27 +30,55 @@
 
     return filename
 
 
 def main():
     parser = log21.ColorizingArgumentParser()
     parser.add_argument('domains', help='The domain/ip to lookup.', type=str, nargs='*')
-    parser.add_argument('-r', '--registration-data', action='store_true',
-                        help='Lookup the registration data for a domain.')
-    parser.add_argument('-i', '--ip-api', action='store_true', help='Lookup the ip using ip-api.com.')
-    parser.add_argument('-to', '--timeout', type=int, default=10,
-                        help='The time out for the WHOIS request(default=10).')
-    parser.add_argument('-t', '--tree-print', action='store_true',
-                        help='Print the registration data in a tree format.')
+    parser.add_argument(
+        '-r',
+        '--registration-data',
+        action='store_true',
+        help='Lookup the registration data for a domain.'
+    )
+    parser.add_argument(
+        '-i', '--ip-api', action='store_true', help='Lookup the ip using ip-api.com.'
+    )
+    parser.add_argument(
+        '-to',
+        '--timeout',
+        type=int,
+        default=10,
+        help='The time out for the WHOIS request(default=10).'
+    )
+    parser.add_argument(
+        '-t',
+        '--tree-print',
+        action='store_true',
+        help='Print the registration data in a tree format.'
+    )
     parser.add_argument('-o', '--output', help='The output folder.', type=str)
-    parser.add_argument('-R', '--raw', action='store_true', help='Print/save the raw whois data.')
-    parser.add_argument('-np', '--no-print', action='store_true', help='Don\'t print the registration/whois data.')
-    parser.add_argument('-q', '--quiet', action='store_true', help='Don\'t print any output.')
-    parser.add_argument('-v', '--verbose', action='store_true', help='Enable verbose output.')
-    parser.add_argument('-V', '--version', action='version', version=f'whois21 {whois21.__version__}')
+    parser.add_argument(
+        '-R', '--raw', action='store_true', help='Print/save the raw whois data.'
+    )
+    parser.add_argument(
+        '-np',
+        '--no-print',
+        action='store_true',
+        help='Don\'t print the registration/whois data.'
+    )
+    parser.add_argument(
+        '-q', '--quiet', action='store_true', help='Don\'t print any output.'
+    )
+    parser.add_argument(
+        '-v', '--verbose', action='store_true', help='Enable verbose output.'
+    )
+    parser.add_argument(
+        '-V', '--version', action='version', version=f'whois21 {whois21.__version__}'
+    )
     args = parser.parse_args()
 
     if args.verbose and args.quiet:
         parser.error('Cannot use both -v and -q.')
     if args.verbose:
         log21.basic_config(level=log21.DEBUG)
     elif args.quiet:
@@ -64,18 +92,26 @@
         parser.error('Cannot use both -r and -i.')
 
     if args.raw and args.registration_data:
         log21.warn('-R will not effect results from -r.')
     if args.raw and args.ip_api:
         log21.warn('-R will not effect results from -i.')
 
+    # I did not want my IDE to tell me not to assign lambdas to variables so I did
+    # this:
+    # locals().update({'print_result': lambda *_, **__: None})
+    # The point is that this makes my IDE think that `print_result` function might be
+    # unbound...
+    # So you know what? I use the other idea I had(which I thought is too stupid to put
+    # here at first)
+    print_result = (lambda f: f)(lambda *_, **__: None)
+
     if args.no_print:
         if not args.output:
             parser.error('Must specify an output folder with -o when using -np.')
-        print_result = lambda *_args, **kwargs: None
     elif args.tree_print:
         print_result = log21.tree_print
     else:
         print_result = log21.pprint
 
     if args.output:
         os.makedirs(args.output, exist_ok=True)
@@ -115,15 +151,17 @@
                         filename = get_filename(args.output, domain)
                         with open(filename, 'w') as file:
                             json.dump(result, file, indent=4)
                         log21.info(f'Saved registration data to {filename}.')
             elif args.registration_data:
                 for domain in args.domains:
                     log21.info(f'Looking up registration data for {domain}...')
-                    result = whois21.WHOIS(domain, timeout=args.timeout, force_rdap=True).rdap_data
+                    result = whois21.WHOIS(
+                        domain, timeout=args.timeout, force_rdap=True
+                    ).rdap_data
                     print_result(result)
                     if args.output:
                         filename = get_filename(args.output, domain)
                         with open(filename, 'w') as file:
                             json.dump(result, file, indent=4)
                         log21.info(f'Saved registration data to {filename}.')
             else:
```

### Comparing `whois21-1.2.0/whois21/vcard-map.json` & `whois21-1.2.1/whois21/vcard-map.json`

 * *Files identical despite different names*

### Comparing `whois21-1.2.0/whois21.egg-info/PKG-INFO` & `whois21-1.2.1/whois21.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: whois21
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple and easy to use Python package that lets you query whois/RDAP information of a domain/IP.
-Home-page: https://github.com/MPCodeWriter21/whois21
-Author: CodeWriter21
-Author-email: CodeWriter21@gmail.com
+Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/MPCodeWriter21/whois21
+Project-URL: Donations, https://github.com/MPCodeWriter21/whois21/blob/master/DONATE.md
+Project-URL: Source, https://github.com/MPCodeWriter21/whois21
 Keywords: python,python3,CodeWriter21,WHOIS,whois21,RDAP,Registration Data Access Protocol,DNS,ASN
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 whois21
 =====
 
 ![version](https://img.shields.io/pypi/v/whois21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/whois21)
@@ -54,15 +57,15 @@
 # And install it using this command
 pip install whois21-x.x.x.tar.gz
 ```
 
 Or you can clone [the repository](https://github.com/MPCodeWriter21/whois21) and run:
 
 ```shell
-python setup.py install
+python -m build .
 ```
 
 ### Dependencies
 
 + [requests](https://requests.readthedocs.io/en/master/): Used for:
     - Downloading list of whois and RDAP servers.
     - Downloading RDAP information.
@@ -89,17 +92,17 @@
     - Type hinting.
 + [re](https://docs.python.org/3/library/re.html) (A core python module): Used for:
     - Matching date-time strings with regular expressions.
 
 Changes
 -------
 
-### 1.2.0
+### 1.2.1
 
-Added ip-api.com API support.
+Switched from `setup.py` to `pyproject.toml`.
 
 Usage Examples:
 ---------------
 
 ### CLI Examples
 
 + Example 1: Query whois information of google.com
```

