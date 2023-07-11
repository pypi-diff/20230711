# Comparing `tmp/mailmerge-2.2.1.tar.gz` & `tmp/mailmerge-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailmerge-2.2.1.tar", last modified: Fri Oct  8 13:05:49 2021, max compression
+gzip compressed data, was "mailmerge-2.2.2.tar", last modified: Tue Jul 11 12:40:42 2023, max compression
```

## Comparing `mailmerge-2.2.1.tar` & `mailmerge-2.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 awdeorio   (503) staff       (20)        0 2021-10-08 13:05:49.682847 mailmerge-2.2.1/
--rw-rw-r--   0 awdeorio   (503) staff       (20)      384 2021-06-07 18:37:26.000000 mailmerge-2.2.1/.pylintrc
--rw-rw-r--   0 awdeorio   (503) staff       (20)      849 2021-10-08 13:05:33.000000 mailmerge-2.2.1/CONTRIBUTING.md
--rw-rw-r--   0 awdeorio   (503) staff       (20)     1080 2019-05-14 18:36:54.000000 mailmerge-2.2.1/LICENSE
--rw-rw-r--   0 awdeorio   (503) staff       (20)      228 2021-07-16 23:01:53.000000 mailmerge-2.2.1/MANIFEST.in
--rw-rw-r--   0 awdeorio   (503) staff       (20)    13672 2021-10-08 13:05:49.682488 mailmerge-2.2.1/PKG-INFO
--rw-rw-r--   0 awdeorio   (503) staff       (20)    13269 2021-10-08 13:05:33.000000 mailmerge-2.2.1/README.md
-drwxrwxr-x   0 awdeorio   (503) staff       (20)        0 2021-10-08 13:05:49.674641 mailmerge-2.2.1/mailmerge/
--rw-rw-r--   0 awdeorio   (503) staff       (20)      234 2021-07-16 17:58:04.000000 mailmerge-2.2.1/mailmerge/__init__.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    11717 2021-10-08 13:05:33.000000 mailmerge-2.2.1/mailmerge/__main__.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)      240 2021-07-16 17:58:04.000000 mailmerge-2.2.1/mailmerge/exceptions.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)     4611 2021-10-08 13:05:33.000000 mailmerge-2.2.1/mailmerge/sendmail_client.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    13311 2021-10-08 13:05:33.000000 mailmerge-2.2.1/mailmerge/template_message.py
-drwxrwxr-x   0 awdeorio   (503) staff       (20)        0 2021-10-08 13:05:49.676632 mailmerge-2.2.1/mailmerge.egg-info/
--rw-rw-r--   0 awdeorio   (503) staff       (20)    13672 2021-10-08 13:05:49.000000 mailmerge-2.2.1/mailmerge.egg-info/PKG-INFO
--rw-rw-r--   0 awdeorio   (503) staff       (20)      793 2021-10-08 13:05:49.000000 mailmerge-2.2.1/mailmerge.egg-info/SOURCES.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)        1 2021-10-08 13:05:49.000000 mailmerge-2.2.1/mailmerge.egg-info/dependency_links.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)       55 2021-10-08 13:05:49.000000 mailmerge-2.2.1/mailmerge.egg-info/entry_points.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)      147 2021-10-08 13:05:49.000000 mailmerge-2.2.1/mailmerge.egg-info/requires.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)       10 2021-10-08 13:05:49.000000 mailmerge-2.2.1/mailmerge.egg-info/top_level.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)       38 2021-10-08 13:05:49.682958 mailmerge-2.2.1/setup.cfg
--rw-rw-r--   0 awdeorio   (503) staff       (20)     1281 2021-10-08 13:05:33.000000 mailmerge-2.2.1/setup.py
-drwxrwxr-x   0 awdeorio   (503) staff       (20)        0 2021-10-08 13:05:49.680020 mailmerge-2.2.1/tests/
--rw-rw-r--   0 awdeorio   (503) staff       (20)       97 2021-07-16 17:58:04.000000 mailmerge-2.2.1/tests/__init__.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)     3461 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_helpers.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    27003 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_main.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    19537 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_main_output.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)     3619 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_ratelimit.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    12900 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_sendmail_client.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    28306 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_template_message.py
--rw-rw-r--   0 awdeorio   (503) staff       (20)    13866 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/test_template_message_encodings.py
-drwxrwxr-x   0 awdeorio   (503) staff       (20)        0 2021-10-08 13:05:49.682001 mailmerge-2.2.1/tests/testdata/
--rw-rw-r--   0 awdeorio   (503) staff       (20)       23 2019-11-01 17:36:28.000000 mailmerge-2.2.1/tests/testdata/attachment_1.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)       24 2019-11-01 17:36:28.000000 mailmerge-2.2.1/tests/testdata/attachment_17.txt
--rw-rw-r--   0 awdeorio   (503) staff       (20)     5617 2019-11-01 17:36:28.000000 mailmerge-2.2.1/tests/testdata/attachment_2.pdf
--rw-rw-r--   0 awdeorio   (503) staff       (20)      697 2021-06-07 18:37:26.000000 mailmerge-2.2.1/tests/testdata/attachment_3.jpg
--rw-rw-r--   0 awdeorio   (503) staff       (20)       36 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/testdata/mailmerge_database_with_BOM.csv
--rw-rw-r--   0 awdeorio   (503) staff       (20)      222 2021-10-08 13:05:33.000000 mailmerge-2.2.1/tests/utils.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.063787 mailmerge-2.2.2/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      384 2021-06-07 18:37:26.000000 mailmerge-2.2.2/.pylintrc
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      849 2021-10-08 13:05:33.000000 mailmerge-2.2.2/CONTRIBUTING.md
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1080 2019-05-14 18:36:54.000000 mailmerge-2.2.2/LICENSE
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      228 2021-07-16 23:01:53.000000 mailmerge-2.2.2/MANIFEST.in
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13652 2023-07-11 12:40:42.063641 mailmerge-2.2.2/PKG-INFO
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13269 2022-10-05 18:36:38.000000 mailmerge-2.2.2/README.md
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.061043 mailmerge-2.2.2/mailmerge/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      234 2021-07-16 17:58:04.000000 mailmerge-2.2.2/mailmerge/__init__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    12596 2023-07-11 12:40:31.000000 mailmerge-2.2.2/mailmerge/__main__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      240 2021-07-16 17:58:04.000000 mailmerge-2.2.2/mailmerge/exceptions.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     4866 2023-07-11 12:40:31.000000 mailmerge-2.2.2/mailmerge/sendmail_client.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13496 2023-07-11 12:40:31.000000 mailmerge-2.2.2/mailmerge/template_message.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.061776 mailmerge-2.2.2/mailmerge.egg-info/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13652 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/PKG-INFO
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      793 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/SOURCES.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        1 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/dependency_links.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       54 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/entry_points.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      147 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/requires.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/top_level.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       38 2023-07-11 12:40:42.063820 mailmerge-2.2.2/setup.cfg
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1281 2023-07-11 12:40:31.000000 mailmerge-2.2.2/setup.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.062885 mailmerge-2.2.2/tests/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       97 2021-07-16 17:58:04.000000 mailmerge-2.2.2/tests/__init__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     3455 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_helpers.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    30347 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_main.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    19537 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/test_main_output.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     3619 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/test_ratelimit.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    14167 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_sendmail_client.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    28193 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_template_message.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13866 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/test_template_message_encodings.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.063476 mailmerge-2.2.2/tests/testdata/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2019-11-01 17:36:28.000000 mailmerge-2.2.2/tests/testdata/attachment_1.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       24 2019-11-01 17:36:28.000000 mailmerge-2.2.2/tests/testdata/attachment_17.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     5617 2019-11-01 17:36:28.000000 mailmerge-2.2.2/tests/testdata/attachment_2.pdf
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      697 2021-06-07 18:37:26.000000 mailmerge-2.2.2/tests/testdata/attachment_3.jpg
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       36 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/testdata/mailmerge_database_with_BOM.csv
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      222 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/utils.py
```

### Comparing `mailmerge-2.2.1/CONTRIBUTING.md` & `mailmerge-2.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/LICENSE` & `mailmerge-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/PKG-INFO` & `mailmerge-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mailmerge
-Version: 2.2.1
+Version: 2.2.2
 Summary: A simple, command line mail merge tool
 Home-page: https://github.com/awdeorio/mailmerge/
 Author: Andrew DeOrio
 Author-email: awdeorio@umich.edu
 License: MIT
 Keywords: mail merge,mailmerge,email
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 Mailmerge
@@ -436,9 +435,7 @@
 
 ## Contributing
 Contributions from the community are welcome! Check out the [guide for contributing](CONTRIBUTING.md).
 
 
 ## Acknowledgements
 Mailmerge is written by Andrew DeOrio <awdeorio@umich.edu>, [http://andrewdeorio.com](http://andrewdeorio.com).  Sesh Sadasivam (@seshrs) contributed many features and bug fixes.
-
-
```

### Comparing `mailmerge-2.2.1/README.md` & `mailmerge-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/mailmerge/__main__.py` & `mailmerge-2.2.2/mailmerge/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,14 +236,22 @@
             # [smtp_server]
             # host = newman.eecs.umich.edu
             # port = 25
             # security = STARTTLS
             # username = YOUR_USERNAME_HERE
             # ratelimit = 0
 
+            # Example: Plain security
+            # [smtp_server]
+            # host = newman.eecs.umich.edu
+            # port = 25
+            # security = PLAIN
+            # username = YOUR_USERNAME_HERE
+            # ratelimit = 0
+
             # Example: No security
             # [smtp_server]
             # host = newman.eecs.umich.edu
             # port = 25
             # ratelimit = 0
         """))
     print(textwrap.dedent(f"""\
@@ -251,33 +259,55 @@
         Created sample database "{database_path}"
         Created sample config file "{config_path}"
 
         Edit these files, then run mailmerge again.\
     """))
 
 
+def detect_database_format(database_file):
+    """Automatically detect the database format.
+
+    Automatically detect the format ("dialect") using the CSV library's sniffer
+    class.  For example, comma-delimited, tab-delimited, etc.  Default to
+    StrictExcel if automatic detection fails.
+
+    """
+    class StrictExcel(csv.excel):
+        # Our helper class is really simple
+        # pylint: disable=too-few-public-methods, missing-class-docstring
+        strict = True
+
+    # Read a sample from database
+    sample = database_file.read(1024)
+    database_file.seek(0)
+
+    # Attempt automatic format detection, fall back on StrictExcel default
+    try:
+        csvdialect = csv.Sniffer().sniff(sample, delimiters=",;\t")
+    except csv.Error:
+        csvdialect = StrictExcel
+
+    return csvdialect
+
+
 def read_csv_database(database_path):
     """Read database CSV file, providing one line at a time.
 
-    We'll use a class to modify the csv library's default dialect ('excel') to
-    enable strict syntax checking.  This will trigger errors for things like
+    Use strict syntax checking, which will trigger errors for things like
     unclosed quotes.
 
     We open the file with the utf-8-sig encoding, which skips a byte order mark
     (BOM), if any.  Sometimes Excel will save CSV files with a BOM.  See Issue
     #93 https://github.com/awdeorio/mailmerge/issues/93
 
     """
-    class StrictExcel(csv.excel):
-        # Our helper class is really simple
-        # pylint: disable=too-few-public-methods, missing-class-docstring
-        strict = True
-
     with database_path.open(encoding="utf-8-sig") as database_file:
-        reader = csv.DictReader(database_file, dialect=StrictExcel)
+        csvdialect = detect_database_format(database_file)
+        csvdialect.strict = True
+        reader = csv.DictReader(database_file, dialect=csvdialect)
         try:
             for row in reader:
                 yield row
         except csv.Error as err:
             raise exceptions.MailmergeError(
                 f"{database_path}:{reader.line_num}: {err}"
             )
```

### Comparing `mailmerge-2.2.1/mailmerge/sendmail_client.py` & `mailmerge-2.2.2/mailmerge/sendmail_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             raise exceptions.MailmergeError(f"{self.config_path}: {err}")
 
         # Coerce legacy option "security = Never"
         if security == "Never":
             security = None
 
         # Verify security type
-        if security not in [None, "SSL/TLS", "STARTTLS"]:
+        if security not in [None, "SSL/TLS", "STARTTLS", "PLAIN"]:
             raise exceptions.MailmergeError(
                 f"{self.config_path}: unrecognized security type: '{security}'"
             )
 
         # Verify username
         if security is not None and username is None:
             raise exceptions.MailmergeError(
@@ -96,14 +96,18 @@
             elif self.config.security == "STARTTLS":
                 with smtplib.SMTP(host, port) as smtp:
                     smtp.ehlo()
                     smtp.starttls()
                     smtp.ehlo()
                     smtp.login(self.config.username, self.password)
                     smtp.sendmail(sender, recipients, message_flattened)
+            elif self.config.security == "PLAIN":
+                with smtplib.SMTP(host, port) as smtp:
+                    smtp.login(self.config.username, self.password)
+                    smtp.sendmail(sender, recipients, message_flattened)
             elif self.config.security is None:
                 with smtplib.SMTP(host, port) as smtp:
                     smtp.sendmail(sender, recipients, message_flattened)
         except smtplib.SMTPAuthenticationError as err:
             raise exceptions.MailmergeError(
                 f"{host}:{port} failed to authenticate "
                 f"user '{self.config.username}': {err}"
```

### Comparing `mailmerge-2.2.1/mailmerge/template_message.py` & `mailmerge-2.2.2/mailmerge/template_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             raise exceptions.MailmergeError(f"{self.template_path}: {err}")
         self._message = email.message_from_string(raw_message)
         self._transform_encoding(raw_message)
         self._transform_recipients()
         self._transform_markdown()
         self._transform_attachments()
         self._transform_attachment_references()
-        self._message.__setitem__('Date', email.utils.formatdate())
+        self._message.add_header('Date', email.utils.formatdate())
         assert self._sender
         assert self._recipients
         assert self._message
         return self._sender, self._recipients, self._message
 
     def _transform_encoding(self, raw_message):
         """Detect and set character encoding."""
@@ -70,36 +70,38 @@
         for part in self._message.walk():
             if part.get_content_maintype() == 'multipart':
                 continue
             part.set_charset(encoding)
 
     def _transform_recipients(self):
         """Extract sender and recipients from FROM, TO, CC and BCC fields."""
-        # Extract recipients
+        # The docs recommend using __delitem__()
+        # https://docs.python.org/3/library/email.message.html#email.message.EmailMessage.__delitem__
+        # pylint: disable=unnecessary-dunder-call
         addrs = email.utils.getaddresses(self._message.get_all("TO", [])) + \
             email.utils.getaddresses(self._message.get_all("CC", [])) + \
             email.utils.getaddresses(self._message.get_all("BCC", []))
         self._recipients = [x[1] for x in addrs]
         self._message.__delitem__("bcc")
         self._sender = self._message["from"]
 
     def _make_message_multipart(self):
         """
         Convert self._message into a multipart message.
 
         Specifically, if the message's content-type is not multipart, this
-        method will create a new `multipart/mixed` message, copy message
+        method will create a new `multipart/related` message, copy message
         headers and re-attach the original payload.
         """
         # Do nothing if message already multipart
         if self._message.is_multipart():
             return
 
         # Create empty multipart message
-        multipart_message = email.mime.multipart.MIMEMultipart('mixed')
+        multipart_message = email.mime.multipart.MIMEMultipart('related')
 
         # Copy headers.  Avoid duplicate Content-Type and MIME-Version headers,
         # which we set explicitely.  MIME-Version was set when we created an
         # empty mulitpart message.  Content-Type will be set when we copy the
         # original text later.
         for header_key in set(self._message.keys()):
             if header_key.lower() in ["content-type", "mime-version"]:
@@ -124,21 +126,21 @@
     def _transform_markdown(self):
         """
         Convert markdown in message text to HTML.
 
         Specifically, if the message's content-type is `text/markdown`, we
         transform `self._message` to have the following structure:
 
-        multipart/mixed
+        multipart/related
          └── multipart/alternative
              ├── text/plain (original markdown plaintext)
              └── text/html (converted markdown)
 
         Attachments should be added as subsequent payload items of the
-        top-level `multipart/mixed` message.
+        top-level `multipart/related` message.
         """
         # Do nothing if Content-Type is not text/markdown
         if not self._message['Content-Type'].startswith("text/markdown"):
             return
 
         # Remove the markdown Content-Type header, it's non-standard for email
         del self._message['Content-Type']
@@ -182,28 +184,28 @@
 
         self._message.attach(message_payload)
 
     def _transform_attachments(self):
         """
         Parse attachment headers and generate content-id headers for each.
 
-        Attachments are added to the payload of a `multipart/mixed` message.
+        Attachments are added to the payload of a `multipart/related` message.
         For instance, a plaintext message with attachments would have the
         following structure:
 
-        multipart/mixed
+        multipart/related
          ├── text/plain
          ├── attachment1
          └── attachment2
 
         Another example: If the original message contained `text/markdown`,
         then the message would have the following structure after transforming
         markdown and attachments:
 
-        multipart/mixed
+        multipart/related
          ├── multipart/alternative
          │   ├── text/plain
          │   └── text/html
          ├── attachment1
          └── attachment2
         """
         # Do nothing if message has no attachment header
```

### Comparing `mailmerge-2.2.1/mailmerge.egg-info/PKG-INFO` & `mailmerge-2.2.2/mailmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mailmerge
-Version: 2.2.1
+Version: 2.2.2
 Summary: A simple, command line mail merge tool
 Home-page: https://github.com/awdeorio/mailmerge/
 Author: Andrew DeOrio
 Author-email: awdeorio@umich.edu
 License: MIT
 Keywords: mail merge,mailmerge,email
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 Mailmerge
@@ -436,9 +435,7 @@
 
 ## Contributing
 Contributions from the community are welcome! Check out the [guide for contributing](CONTRIBUTING.md).
 
 
 ## Acknowledgements
 Mailmerge is written by Andrew DeOrio <awdeorio@umich.edu>, [http://andrewdeorio.com](http://andrewdeorio.com).  Sesh Sadasivam (@seshrs) contributed many features and bug fixes.
-
-
```

### Comparing `mailmerge-2.2.1/mailmerge.egg-info/SOURCES.txt` & `mailmerge-2.2.2/mailmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/setup.py` & `mailmerge-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 setuptools.setup(
     name="mailmerge",
     description="A simple, command line mail merge tool",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    version="2.2.1",
+    version="2.2.2",
     author="Andrew DeOrio",
     author_email="awdeorio@umich.edu",
     url="https://github.com/awdeorio/mailmerge/",
     license="MIT",
     packages=["mailmerge"],
     keywords=["mail merge", "mailmerge", "email"],
     install_requires=[
```

### Comparing `mailmerge-2.2.1/tests/test_helpers.py` & `mailmerge-2.2.2/tests/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     output = list(enumerate_range(["a", "b", "c"], stop=1))
     assert output == [(0, "a")]
 
 
 def test_enumerate_range_stop_zero():
     """Verify stop=0."""
     output = list(enumerate_range(["a", "b", "c"], stop=0))
-    assert output == []
+    assert not output
 
 
 def test_enumerate_range_stop_too_big():
     """Verify stop when value is greater than length."""
     output = list(enumerate_range(["a", "b", "c"], stop=10))
     assert output == [(0, "a"), (1, "b"), (2, "c")]
 
@@ -57,21 +57,21 @@
     output = list(enumerate_range(["a", "b", "c"], start=2))
     assert output == [(2, "c")]
 
 
 def test_enumerate_range_start_length():
     """Verify start=length."""
     output = list(enumerate_range(["a", "b", "c"], start=3))
-    assert output == []
+    assert not output
 
 
 def test_enumerate_range_start_too_big():
     """Verify start past the end."""
     output = list(enumerate_range(["a", "b", "c"], start=10))
-    assert output == []
+    assert not output
 
 
 def test_enumerate_range_start_stop():
     """Verify start and stop together."""
     output = list(enumerate_range(["a", "b", "c"], start=1, stop=2))
     assert output == [(1, "b")]
```

### Comparing `mailmerge-2.2.1/tests/test_main.py` & `mailmerge-2.2.2/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -855,7 +855,113 @@
 
         Hello My Name
 
         >>> message 1 sent
         >>> Limit was 1 message.  To remove the limit, use the --no-limit option.
         >>> This was a dry run.  To send messages, use the --no-dry-run option.
     """)  # noqa: E501
+
+
+def test_database_tsv(tmpdir):
+    """Automatically detect TSV database format."""
+    # Simple template
+    template_path = Path(tmpdir/"mailmerge_template.txt")
+    template_path.write_text(textwrap.dedent("""\
+        TO: {{email}}
+        FROM: My Self <myself@mydomain.com>
+
+        Hello {{name}}
+    """), encoding="utf8")
+
+    # Tab-separated format database
+    database_path = Path(tmpdir/"mailmerge_database.csv")
+    database_path.write_text(textwrap.dedent("""\
+        email\tname
+        to@test.com\tMy Name
+    """), encoding="utf8")
+
+    # Simple unsecure server config
+    config_path = Path(tmpdir/"mailmerge_server.conf")
+    config_path.write_text(textwrap.dedent("""\
+        [smtp_server]
+        host = open-smtp.example.com
+        port = 25
+    """), encoding="utf8")
+
+    # Run mailmerge
+    runner = click.testing.CliRunner()
+    with tmpdir.as_cwd():
+        result = runner.invoke(main, ["--output-format", "text"])
+    assert not result.exception
+    assert result.exit_code == 0
+
+    # Verify output
+    stdout = copy.deepcopy(result.output)
+    stdout = re.sub(r"Date:.+", "Date: REDACTED", stdout, re.MULTILINE)
+    assert stdout == textwrap.dedent("""\
+        >>> message 1
+        TO: to@test.com
+        FROM: My Self <myself@mydomain.com>
+        MIME-Version: 1.0
+        Content-Type: text/plain; charset="us-ascii"
+        Content-Transfer-Encoding: 7bit
+        Date: REDACTED
+
+        Hello My Name
+
+        >>> message 1 sent
+        >>> Limit was 1 message.  To remove the limit, use the --no-limit option.
+        >>> This was a dry run.  To send messages, use the --no-dry-run option.
+    """)  # noqa: E501
+
+
+def test_database_semicolon(tmpdir):
+    """Automatically detect semicolon-delimited database format."""
+    # Simple template
+    template_path = Path(tmpdir/"mailmerge_template.txt")
+    template_path.write_text(textwrap.dedent("""\
+        TO: {{email}}
+        FROM: My Self <myself@mydomain.com>
+
+        Hello {{name}}
+    """), encoding="utf8")
+
+    # Semicolon-separated format database
+    database_path = Path(tmpdir/"mailmerge_database.csv")
+    database_path.write_text(textwrap.dedent("""\
+        email;name
+        to@test.com;My Name
+    """), encoding="utf8")
+
+    # Simple unsecure server config
+    config_path = Path(tmpdir/"mailmerge_server.conf")
+    config_path.write_text(textwrap.dedent("""\
+        [smtp_server]
+        host = open-smtp.example.com
+        port = 25
+    """), encoding="utf8")
+
+    # Run mailmerge
+    runner = click.testing.CliRunner()
+    with tmpdir.as_cwd():
+        result = runner.invoke(main, ["--output-format", "text"])
+    assert not result.exception
+    assert result.exit_code == 0
+
+    # Verify output
+    stdout = copy.deepcopy(result.output)
+    stdout = re.sub(r"Date:.+", "Date: REDACTED", stdout, re.MULTILINE)
+    assert stdout == textwrap.dedent("""\
+        >>> message 1
+        TO: to@test.com
+        FROM: My Self <myself@mydomain.com>
+        MIME-Version: 1.0
+        Content-Type: text/plain; charset="us-ascii"
+        Content-Transfer-Encoding: 7bit
+        Date: REDACTED
+
+        Hello My Name
+
+        >>> message 1 sent
+        >>> Limit was 1 message.  To remove the limit, use the --no-limit option.
+        >>> This was a dry run.  To send messages, use the --no-dry-run option.
+    """)  # noqa: E501
```

### Comparing `mailmerge-2.2.1/tests/test_main_output.py` & `mailmerge-2.2.2/tests/test_main_output.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/tests/test_ratelimit.py` & `mailmerge-2.2.2/tests/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/tests/test_sendmail_client.py` & `mailmerge-2.2.2/tests/test_sendmail_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,56 @@
     smtp = mock_smtp.return_value.__enter__.return_value
     assert smtp.ehlo.call_count == 2
     assert smtp.starttls.call_count == 1
     assert smtp.login.call_count == 1
     assert smtp.sendmail.call_count == 1
 
 
+def test_security_plain(mocker, tmp_path):
+    """Verify plain security configuration."""
+    # Config for Plain SMTP server
+    config_path = tmp_path/"server.conf"
+    config_path.write_text(textwrap.dedent("""\
+        [smtp_server]
+        host = newman.eecs.umich.edu
+        port = 25
+        security = PLAIN
+        username = YOUR_USERNAME_HERE
+    """))
+
+    # Simple template
+    sendmail_client = SendmailClient(config_path, dry_run=False)
+    message = email.message_from_string("Hello world")
+
+    # Mock SMTP
+    mock_smtp = mocker.patch('smtplib.SMTP')
+    mock_smtp_ssl = mocker.patch('smtplib.SMTP_SSL')
+
+    # Mock the password entry
+    mock_getpass = mocker.patch('getpass.getpass')
+    mock_getpass.return_value = "password"
+
+    # Send a message
+    sendmail_client.sendmail(
+        sender="test@test.com",
+        recipients=["test@test.com"],
+        message=message,
+    )
+
+    # Verify SMTP library calls
+    assert mock_getpass.call_count == 1
+    assert mock_smtp.call_count == 1
+    assert mock_smtp_ssl.call_count == 0
+    smtp = mock_smtp.return_value.__enter__.return_value
+    assert smtp.ehlo.call_count == 0
+    assert smtp.starttls.call_count == 0
+    assert smtp.login.call_count == 1
+    assert smtp.sendmail.call_count == 1
+
+
 def test_security_ssl(mocker, tmp_path):
     """Verify open (Never) security configuration."""
     # Config for SSL SMTP server
     config_path = tmp_path/"server.conf"
     config_path.write_text(textwrap.dedent("""\
         [smtp_server]
         host = smtp.mail.umich.edu
```

### Comparing `mailmerge-2.2.1/tests/test_template_message.py` & `mailmerge-2.2.2/tests/test_template_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
 
     # Verify sender and recipients
     assert sender == "Bob <bob@bobdomain.com>"
     assert recipients == ["myself@mydomain.com"]
 
     # Verify message is multipart
     assert message.is_multipart()
-    assert message.get_content_subtype() == "mixed"
+    assert message.get_content_subtype() == "related"
 
     # Make sure there is a single multipart/alternative payload
     assert len(message.get_payload()) == 1
     assert message.get_payload()[0].is_multipart()
     assert message.get_payload()[0].get_content_subtype() == "alternative"
 
     # And there should be a plaintext part and an HTML part
@@ -656,18 +656,15 @@
     """), encoding="utf8")
     template_message = TemplateMessage(template_path)
     with pytest.raises(MailmergeError):
         template_message.render({})
 
 
 def test_contenttype_attachment_html_body(tmpdir):
-    """
-    Verify that the content-type of the message is correctly retained with an
-    HTML body.
-    """
+    """Content-type is preserved in HTML body."""
     # Simple attachment
     attachment_path = Path(tmpdir/"attachment.txt")
     attachment_path.write_text("Hello world\n", encoding="utf8")
 
     # HTML template
     template_path = Path(tmpdir/"template.txt")
     template_path.write_text(textwrap.dedent("""\
@@ -687,18 +684,15 @@
     # Verify that the message content type is HTML
     payload = message.get_payload()
     assert len(payload) == 2
     assert payload[0].get_content_type() == 'text/html'
 
 
 def test_contenttype_attachment_markdown_body(tmpdir):
-    """
-    Verify that the content-types of the MarkDown message are correct when
-    attachments are included.
-    """
+    """Content-type for MarkDown messages with attachments."""
     # Simple attachment
     attachment_path = Path(tmpdir/"attachment.txt")
     attachment_path.write_text("Hello world\n", encoding="utf8")
 
     # HTML template
     template_path = Path(tmpdir/"template.txt")
     template_path.write_text(textwrap.dedent("""\
@@ -781,15 +775,15 @@
     })
 
     # Verifty no duplicate headers
     assert len(message.keys()) == len(set(message.keys()))
 
 
 def test_attachment_image_in_markdown(tmp_path):
-    """Images sent as attachments should get linked correctly in images"""
+    """Images sent as attachments should get linked correctly in images."""
     shutil.copy(str(utils.TESTDATA/"attachment_3.jpg"), str(tmp_path))
 
     # Create template .txt file
     template_path = tmp_path / "template.txt"
     template_path.write_text(textwrap.dedent("""\
         TO: {{email}}
         SUBJECT: Testing mailmerge
@@ -838,15 +832,15 @@
         <body><p><img src="cid:{cid}" alt="" /></p></body>
         </html>
     """))
     assert html_docs_equal(html5lib.parse(htmltext), expected)
 
 
 def test_content_id_header_for_attachments(tmpdir):
-    """All attachments should get a content-id header"""
+    """All attachments should get a content-id header."""
     attachment_path = Path(tmpdir/"attachment.txt")
     attachment_path.write_text("Hello world\n", encoding="utf8")
 
     # Simple template
     template_path = Path(tmpdir/"template.txt")
     template_path.write_text(textwrap.dedent("""\
         TO: to@test.com
```

### Comparing `mailmerge-2.2.1/tests/test_template_message_encodings.py` & `mailmerge-2.2.2/tests/test_template_message_encodings.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/tests/testdata/attachment_2.pdf` & `mailmerge-2.2.2/tests/testdata/attachment_2.pdf`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.1/tests/testdata/attachment_3.jpg` & `mailmerge-2.2.2/tests/testdata/attachment_3.jpg`

 * *Files identical despite different names*

