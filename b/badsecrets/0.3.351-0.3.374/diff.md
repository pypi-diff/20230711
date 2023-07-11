# Comparing `tmp/badsecrets-0.3.351.tar.gz` & `tmp/badsecrets-0.3.374.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.3.351.tar", max compression
+gzip compressed data, was "badsecrets-0.3.374.tar", max compression
```

## Comparing `badsecrets-0.3.351.tar` & `badsecrets-0.3.374.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    35149 2023-06-21 22:06:51.945127 badsecrets-0.3.351/LICENSE
--rw-r--r--   0        0        0    31849 2023-06-21 22:06:51.945127 badsecrets-0.3.351/README.md
--rw-r--r--   0        0        0      711 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/__init__.py
--rw-r--r--   0        0        0     6802 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4220 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     7821 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3544 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     3570 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0     5868 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0      986 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2022 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0     1057 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     4057 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    14819 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2172 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1931 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3061 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2932 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4949 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     3718 2023-06-21 22:06:51.945127 badsecrets-0.3.351/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654111 2023-06-21 22:06:51.953127 badsecrets-0.3.351/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-06-21 22:06:51.953127 badsecrets-0.3.351/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-06-21 22:06:51.953127 badsecrets-0.3.351/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-06-21 22:06:51.969128 badsecrets-0.3.351/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-06-21 22:06:51.969128 badsecrets-0.3.351/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-06-21 22:06:51.969128 badsecrets-0.3.351/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-06-21 22:06:51.969128 badsecrets-0.3.351/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-06-21 22:06:51.969128 badsecrets-0.3.351/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-06-21 22:06:51.973128 badsecrets-0.3.351/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      957 2023-06-21 22:07:13.917563 badsecrets-0.3.351/pyproject.toml
--rw-r--r--   0        0        0    32703 1970-01-01 00:00:00.000000 badsecrets-0.3.351/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-11 04:16:58.264845 badsecrets-0.3.374/LICENSE
+-rw-r--r--   0        0        0    31849 2023-07-11 04:16:58.264845 badsecrets-0.3.374/README.md
+-rw-r--r--   0        0        0      711 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/__init__.py
+-rw-r--r--   0        0        0     6986 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4210 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     7875 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     5076 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0    10204 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0      986 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2022 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/express_signedcookies.py
+-rw-r--r--   0        0        0     1057 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4057 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14819 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2172 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1931 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3077 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2932 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     4949 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3718 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654096 2023-07-11 04:16:58.272845 badsecrets-0.3.374/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-07-11 04:16:58.272845 badsecrets-0.3.374/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-07-11 04:16:58.272845 badsecrets-0.3.374/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-07-11 04:17:28.720888 badsecrets-0.3.374/pyproject.toml
+-rw-r--r--   0        0        0    32703 1970-01-01 00:00:00.000000 badsecrets-0.3.374/PKG-INFO
```

### Comparing `badsecrets-0.3.351/LICENSE` & `badsecrets-0.3.374/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/README.md` & `badsecrets-0.3.374/README.md`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/__init__.py` & `badsecrets-0.3.374/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/base.py` & `badsecrets-0.3.374/badsecrets/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             filepaths.append(f"{os.path.dirname(os.path.abspath(__file__))}/resources/{r}")
         for filepath in filepaths:
             with open(filepath) as r:
                 for l in r.readlines():
                     if len(l) > 0:
                         yield l
 
-    def carve_to_check_secret(self, s):
+    def carve_to_check_secret(self, s, **kwargs):
         if s.groups():
             r = self.check_secret(s.groups()[0])
             return r
 
     @abstractmethod
     def carve_regex(self):
         return None
@@ -115,15 +115,15 @@
 
         if body:
             if type(body) != str:
                 raise badsecrets.errors.CarveException("Body argument must be type str")
             if self.carve_regex():
                 s = re.search(self.carve_regex(), body)
                 if s:
-                    r = self.carve_to_check_secret(s)
+                    r = self.carve_to_check_secret(s, url=kwargs.get("url", None))
                     if r:
                         r["type"] = "SecretFound"
                     else:
                         r = {"type": "IdentifyOnly"}
                         r["hashcat"] = self.get_hashcat_commands(s.groups()[0])
                     r["product"] = s.groups()[0]
                     r["location"] = "body"
@@ -145,28 +145,29 @@
     @staticmethod
     def search_dict(d, query):
         items = [key for key, value in d.items() if query == value]
         if items:
             return items
 
 
-def hashcat_all_modules(product):
+def hashcat_all_modules(product, detecting_module=None, *args):
     hashcat_candidates = []
     for m in BadsecretsBase.__subclasses__():
-        x = m()
-        if x.identify(product):
-            hashcat_commands = x.get_hashcat_commands(product)
-            if hashcat_commands:
-                for hcc in hashcat_commands:
-                    z = {
-                        "detecting_module": m.__name__,
-                        "hashcat_command": hcc["command"],
-                        "hashcat_description": hcc["description"],
-                    }
-                    hashcat_candidates.append(z)
+        if detecting_module == m.__name__ or detecting_module == None:
+            x = m()
+            if x.identify(product):
+                hashcat_commands = x.get_hashcat_commands(product)
+                if hashcat_commands:
+                    for hcc in hashcat_commands:
+                        z = {
+                            "detecting_module": m.__name__,
+                            "hashcat_command": hcc["command"],
+                            "hashcat_description": hcc["description"],
+                        }
+                        hashcat_candidates.append(z)
     return hashcat_candidates
 
 
 def check_all_modules(*args, **kwargs):
     for m in BadsecretsBase.__subclasses__():
         x = m(custom_resource=kwargs.get("custom_resource", None))
         r = x.check_secret(*args[0 : x.check_secret_args])
```

### Comparing `badsecrets-0.3.351/badsecrets/examples/blacklist3r.py` & `badsecrets-0.3.374/badsecrets/examples/blacklist3r.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from badsecrets import modules_loaded
 
 ASPNET_Viewstate = modules_loaded["aspnet_viewstate"]
 
 
 def check_viewstate(viewstate, generator):
     bs_vs = ASPNET_Viewstate()
-    r = bs_vs.check_secret(viewstate, generator=generator)
+    r = bs_vs.check_secret(viewstate, generator)
     return r
 
 
 def print_result(r):
     print("Matching MachineKeys found!")
     print(r["secret"])
```

### Comparing `badsecrets-0.3.351/badsecrets/examples/cli.py` & `badsecrets-0.3.374/badsecrets/examples/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,22 +204,22 @@
 
         try:
             res = requests.get(args.url, proxies=proxies, headers=headers, verify=False)
         except (requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout):
             print_status(f"Error connecting to URL: [{args.url}]", color=Fore.RED)
             return
 
-        r_list = carve_all_modules(requests_response=res, custom_resource=custom_resource)
+        r_list = carve_all_modules(requests_response=res, custom_resource=custom_resource, url=args.url)
         if r_list:
             for r in r_list:
                 if r["type"] == "SecretFound":
                     report = ReportSecret(r)
                 else:
                     if not args.no_hashcat:
-                        hashcat_candidates = hashcat_all_modules(r["product"])
+                        hashcat_candidates = hashcat_all_modules(r["product"], detecting_module=r["detecting_module"])
                         if hashcat_candidates:
                             r["hashcat"] = hashcat_candidates
                     report = ReportIdentify(r)
                 report.report()
         else:
             print_status("No secrets found :(", color=Fore.RED)
```

### Comparing `badsecrets-0.3.351/badsecrets/examples/symfony_knownkey.py` & `badsecrets-0.3.374/badsecrets/examples/symfony_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.3.374/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/helpers.py` & `badsecrets-0.3.374/badsecrets/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,62 @@
 import sys
+import hmac
+import struct
 import hashlib
 from badsecrets.errors import BadsecretsException
 
 
+def _writeuint(v):
+    return struct.pack(">I", v)
+
+
 def unpad(s):
     return s[: -ord(s[len(s) - 1 :])]
 
 
+def sp800_108_derivekey(key, label, context, keyLengthInBits):
+    lblcnt = 0 if label is None else len(label)
+    ctxcnt = 0 if context is None else len(context)
+    buffer = b"\x00" * (4 + lblcnt + 1 + ctxcnt + 4)
+    if lblcnt != 0:
+        buffer = buffer[:4] + label + buffer[4 + lblcnt :]
+    if ctxcnt != 0:
+        buffer = buffer[: 5 + lblcnt] + context + buffer[5 + lblcnt + ctxcnt :]
+    buffer = buffer[: 5 + lblcnt + ctxcnt] + _writeuint(keyLengthInBits) + buffer[5 + lblcnt + ctxcnt + 4 :]
+    v = int(keyLengthInBits / 8)
+    res = b"\x00" * v
+    num = 1
+    while v > 0:
+        buffer = _writeuint(num) + buffer[4:]
+        h = hmac.new(key, buffer, hashlib.sha512)
+        hash = h.digest()
+        cnt = min(v, len(hash))
+        res = hash[:cnt] + res[cnt:]
+        v -= cnt
+        num += 1
+    return res
+
+
+def write_vlq_string(string):
+    encoded_string = string.encode("utf-8")
+    length = len(encoded_string)
+    length_vlq = bytearray()
+    while length >= 0x80:
+        length_vlq.append((length | 0x80) & 0xFF)
+        length >>= 7
+    length_vlq.append(length)
+    return bytes(length_vlq) + encoded_string
+
+
+def sp800_108_get_key_derivation_parameters(primary_purpose, specific_purposes):
+    derived_key_label = primary_purpose.encode("utf-8")
+    derived_key_context = b"".join([write_vlq_string(purpose) for purpose in specific_purposes])
+    return derived_key_label, derived_key_context
+
+
 class Csharp_pbkdf1_exception(BadsecretsException):
     pass
 
 
 class Csharp_pbkdf1:
     def __init__(self, passwordBytes, saltBytes, iterations):
         self.passwordBytes = passwordBytes
```

### Comparing `badsecrets-0.3.351/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.3.374/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.3.374/badsecrets/modules/express_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.3.374/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/generic_jwt.py` & `badsecrets-0.3.374/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.3.374/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.3.374/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.3.374/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.3.374/badsecrets/modules/rails_secretkeybase.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         # Cookie is likely Rails 4/5/6 AES-CBC Cookie
         elif len(split_rails_cookie) == 2:
             try:
                 encrypted_data = base64.b64decode(data).decode()
                 iv = encrypted_data.split("--")[1]
                 data = encrypted_data.split("--")[0]
-            except (UnicodeDecodeError, IndexError):
+            except (UnicodeDecodeError, IndexError, binascii.Error):
                 return
 
             if len(base64.b64decode(iv)) == 16:
                 aes_secret = PBKDF2(secret_key_base, "encrypted cookie", 64, 1000)
                 cipher = AES.new(aes_secret[:32], AES.MODE_CBC, base64.b64decode(iv))
                 try:
                     dec = unpad(cipher.decrypt(base64.b64decode(data)), 16)
```

### Comparing `badsecrets-0.3.351/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.3.374/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.3.374/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.3.374/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.3.374/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2775,15 +2775,14 @@
 C3C2EDA6DCB508C788D73FC5810F68C37036B60C6BB3232BC1AFAB69A10EC6DFD4771D875F10F105903054AF44517F52599AB0F4123467A35D62F55C5A1E8F97,2CD322113C05C2BAE1971179824F04A5EFF5113E7AB60BAF
 C3D75060EB9CDF8B88B71AFC2CE882D8B0D15A99F78C60DE96C2CE35893EC082,D120AA1747A5D31CB9D2AD1479BA15CDCC9EC4072CCFBC34F6E49E21D475560C
 C3DD3F2A15D70EE0E82A130E430FAFF65588C98DFA3D494ED7F4DFB9F9B0E8C2684342DC5E8BB712A0F92194919D7E3B78324B1AEB21AC6F35B5175B87BB1012,9F4000BFD1E861B291441C2F725603A49398ADA004C4B896
 C3DD5E21134BDCAF7D951A2ED8E45F7E7395A8CEBAA6A43A8D8528A85B9AB00D,ADCBCFC864936D0248917F2CF276E6F392F5A202F1DB53D9
 C3E566B36D7D737C3642E6AEE1FBF7E40F002E08,D993D168BAA3518CB12F32BBBF93D259A2D3E91EA0DE65A8
 C3ECDA658438CB56E1B2214D481AD1357E57469F,E23294FEFD59AF24CA7BE43F355F38E94D1FB48B687A6D3C
 C3F4C2EA177D400D5079E51F9CF1C9F8BBC4BD1E8ACC3C08EBB55D3FEB9D2076AFB83A4E23856B34CF4A10F98FADB0625147D3B5EC5C425995DECFFD0D10B0B7,A2C88FF5B85D9A4073DF6E63BFEDC8122D26BEFFD1436284
-***REMOVED***
 C404DBC640257AA6DD1632CC42279467947E0539A484964B67AF2706E0C1E50A7D0075698C692D5E27A5337A223A1D7EE78678B803918D5F8C1F0A623E2FFC07,C3C74BBF830D1FD79576F70BEE59D12D9A99CC7AB564E3BD851C27A2563A72C1
 C40E61DCB9CF02AF9B87ECF85E4F098A7A92858E34654EC633A04992E4D9222AA9EE7E5B13A1A67F36336404E93A664BA05E797543C1163BF5088618507E6853,E62236F1C28D325263320588532A716642411E7417752D4D
 C41E5BEB7FD938AC1368A9EE0A97BAD2F6DBC4AB563FB9F89ED37C4D0CD5B7918FA822AD2A181A5B4FB7CF3826C56F043A93B4B08816E037485F61070AB2AD6A,968DB8BE829EC55028B809D75D3DF3BAB406B2D8EF7FF712D7F36B9ABCD99016
 C41EA302D392690C49CAA100699BB8934C2FBCC62458168F7386E37A4B94B8CE7B19DA0F50704D3D8E3165FA1C79824F34FE9FBF4A3648B37A3F661ACA293FC3,DDCEB3EE06FC331AD835FBEDA73D1FDDDF5E3C93C8DA043C
 C42CF6EA5587DA3C75EDEFC1918DEDC576427672803540B203F3643417D91AD6236B82052463CD43F99E35E0010AE85D932236C989E52C2361A6A1B779060582,E7781353BC934C20632783D0BD8CBB9296BA8E6FADCF58BDA5A12D40ECE18FD5
 C42FDB4C86E27F70053C19DB53BFE92154CD4ED45B3599F287D4C55060367D0688715355B7B5DC846C240FE84162D3C74B5C3A26EC615CBABDAF971E9A19BA07,6ABF64223B49482D5A38A4D7E9FC1A4145C3D9EBD188FA85F5152F8D9EFE4692
 C435FCF3C6BC11FC9D54093AA3F64EADE882D0B434FD25A2FCBC7068B9F2E817,FA9217D420AEB67377A079A68163A3164802DB79CA76AFA8AC8BDA7CAA4F93D4
```

### Comparing `badsecrets-0.3.351/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.3.374/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.3.374/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.3.374/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.3.374/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.3.374/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.3.374/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.3.374/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.3.374/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.3.374/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.3.374/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.3.374/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.351/pyproject.toml` & `badsecrets-0.3.374/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.3.351"
+version = "v0.3.374"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
```

### Comparing `badsecrets-0.3.351/PKG-INFO` & `badsecrets-0.3.374/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.3.351
+Version: 0.3.374
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

