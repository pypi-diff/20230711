# Comparing `tmp/safeway_coupons-0.2.3.tar.gz` & `tmp/safeway_coupons-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeway_coupons-0.2.3.tar", max compression
+gzip compressed data, was "safeway_coupons-0.2.4.tar", max compression
```

## Comparing `safeway_coupons-0.2.3.tar` & `safeway_coupons-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/LICENSE
--rw-r--r--   0        0        0     5424 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/README.md
--rw-r--r--   0        0        0     2457 2023-07-10 06:34:28.120574 safeway_coupons-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      166 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/__init__.py
--rw-r--r--   0        0        0       22 2023-07-10 06:34:28.124574 safeway_coupons-0.2.3/safeway_coupons/__version__.py
--rw-r--r--   0        0        0      161 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/accounts.py
--rw-r--r--   0        0        0     2889 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/app.py
--rw-r--r--   0        0        0     2129 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/client.py
--rw-r--r--   0        0        0     2138 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/config.py
--rw-r--r--   0        0        0     2960 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/email.py
--rw-r--r--   0        0        0     1025 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/errors.py
--rw-r--r--   0        0        0     1029 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/methods.py
--rw-r--r--   0        0        0     2103 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/models.py
--rw-r--r--   0        0        0        0 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/py.typed
--rw-r--r--   0        0        0     3528 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/safeway.py
--rw-r--r--   0        0        0     6067 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/session.py
--rw-r--r--   0        0        0      846 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/utils.py
--rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 safeway_coupons-0.2.3/setup.py
--rw-r--r--   0        0        0     6559 1970-01-01 00:00:00.000000 safeway_coupons-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5662 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/README.md
+-rw-r--r--   0        0        0     2496 2023-07-11 05:17:33.307485 safeway_coupons-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 05:17:33.323485 safeway_coupons-0.2.4/safeway_coupons/__version__.py
+-rw-r--r--   0        0        0      161 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/accounts.py
+-rw-r--r--   0        0        0     3837 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/app.py
+-rw-r--r--   0        0        0     2129 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/client.py
+-rw-r--r--   0        0        0     2138 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/config.py
+-rw-r--r--   0        0        0     3057 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/email.py
+-rw-r--r--   0        0        0     1025 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/errors.py
+-rw-r--r--   0        0        0     1029 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/methods.py
+-rw-r--r--   0        0        0     2103 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/models.py
+-rw-r--r--   0        0        0        0 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/py.typed
+-rw-r--r--   0        0        0     3695 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/safeway.py
+-rw-r--r--   0        0        0     6067 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/session.py
+-rw-r--r--   0        0        0      846 2023-07-11 05:17:02.698915 safeway_coupons-0.2.4/safeway_coupons/utils.py
+-rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 safeway_coupons-0.2.4/setup.py
+-rw-r--r--   0        0        0     6797 1970-01-01 00:00:00.000000 safeway_coupons-0.2.4/PKG-INFO
```

### Comparing `safeway_coupons-0.2.3/LICENSE` & `safeway_coupons-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/README.md` & `safeway_coupons-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,35 +32,39 @@
 ```yaml
 version: "3.7"
 
 services:
   safeway-coupons:
     image: ghcr.io/smkent/safeway-coupons:latest
     environment:
-      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day
+      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM UTC each day
+      # TZ: Antarctica/McMurdo  # Optional time zone to use instead of UTC
       SMTPHOST: your.smtp.host
       SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com
       SAFEWAY_ACCOUNT_PASSWORD: very_secret
       SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com
       SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com
+      # EXTRA_ARGS: --debug  # Optional
     restart: unless-stopped
 ```
 
 Example `docker-compose.yaml` with configuration via accounts file:
 
 ```yaml
 version: "3.7"
 
 services:
   safeway-coupons:
     image: ghcr.io/smkent/safeway-coupons:latest
     environment:
-      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day
+      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM UTC each day
+      # TZ: Antarctica/McMurdo  # Optional time zone to use instead of UTC
       SMTPHOST: your.smtp.host
       SAFEWAY_ACCOUNTS_FILE: /accounts_file
+      # EXTRA_ARGS: --debug  # Optional
     restart: unless-stopped
     volumes:
       - path/to/safeway_accounts_file:/accounts_file:ro
 ```
 
 Start the container by running:
```

### Comparing `safeway_coupons-0.2.3/pyproject.toml` & `safeway_coupons-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "safeway-coupons"
-version = "0.2.3"
+version = "0.2.4"
 description = "Automatic coupon clipper for Safeway's online \"Safeway for U\" coupons"
 license = "GPL-3.0-or-later"
 authors = ["Stephen Kent <smkent@smkent.net>"]
 readme = "README.md"
 repository = "https://github.com/smkent/safeway-coupons"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -65,14 +65,15 @@
 [tool.poe.tasks.test]
 sequence = ["lint", "pytest"]
 help = "Run all tests"
 
 [tool.bandit]
 skips = [
     "B101",  # assert_used
+    "B113",  # request_without_timeout
     "B311",  # blacklist_random
     "B404",  # blacklist_subprocess
     "B603",  # subprocess_without_shell_equals_true
 ]
 
 [tool.black]
 line-length = 79
```

### Comparing `safeway_coupons-0.2.3/safeway_coupons/app.py` & `safeway_coupons-0.2.4/safeway_coupons/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import argparse
+import shlex
 import sys
+import traceback
 from http.client import HTTPConnection
 from pathlib import Path
 
 from .config import Config
+from .errors import Error
 from .safeway import SafewayCoupons
 
 
 def _parse_args() -> argparse.Namespace:
     description = 'Automatic coupon clipper for "Safeway for U" coupons'
     arg_parser = argparse.ArgumentParser(description=description)
     arg_parser.add_argument(
@@ -48,14 +51,25 @@
         dest="max_clip_count",
         type=int,
         default=0,
         metavar="number",
         help="Maximum number of coupons to clip (default: all)",
     )
     arg_parser.add_argument(
+        "--sendmail",
+        metavar="path/to/sendmail",
+        dest="sendmail",
+        type=shlex.split,
+        default="/usr/sbin/sendmail",
+        help=(
+            "Path to sendmail and any additional arguments to use when "
+            "sending email (default: %(default)s)"
+        ),
+    )
+    arg_parser.add_argument(
         "-n",
         "--no-email",
         dest="send_email",
         action="store_false",
         help="Don't send results email",
     )
     arg_parser.add_argument(
@@ -73,34 +87,52 @@
         dest="sleep_level",
         action="count",
         default=0,
         help=(
             "Don't wait between long requests. Specify twice to never wait."
         ),
     )
+    arg_parser.add_argument(
+        "-E",
+        "--continue-on-error",
+        dest="continue_on_error",
+        action="store_true",
+        help="Continue clipping coupons for the next account on error",
+    )
     return arg_parser.parse_args()
 
 
 def main() -> None:
     args = _parse_args()
     accounts = Config.load_accounts(config_file=args.accounts_config)
     if not accounts:
         print("Error: No Safeway account(s) configured", file=sys.stderr)
         sys.exit(1)
     if args.debug_level >= 2:
         HTTPConnection.debuglevel = 1
     sc = SafewayCoupons(
         send_email=args.send_email,
+        sendmail=args.sendmail,
         debug_level=args.debug_level,
         debug_dir=Path(args.debug_dir) if args.debug_dir else None,
         sleep_level=args.sleep_level,
         dry_run=args.dry_run,
         max_clip_count=args.max_clip_count,
     )
+    errors = 0
     try:
         for account in accounts:
-            sc.clip_for_account(account)
+            try:
+                sc.clip_for_account(account)
+            except Error:
+                if not args.continue_on_error:
+                    raise
+                traceback.print_exc()
+                errors += 1
+        if errors:
+            print(f"Error clipping coupons for {errors} account(s)")
+            sys.exit(1)
     except Exception as e:
         if args.debug_level:
             raise
         print(f"Error: {e}", file=sys.stderr)
         sys.exit(1)
```

### Comparing `safeway_coupons-0.2.3/safeway_coupons/client.py` & `safeway_coupons-0.2.4/safeway_coupons/client.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/safeway_coupons/config.py` & `safeway_coupons-0.2.4/safeway_coupons/config.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/safeway_coupons/email.py` & `safeway_coupons-0.2.4/safeway_coupons/email.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .accounts import Account
 from .errors import ClipError, Error, TooManyClipErrors
 from .models import Offer
 
 
 def _send_email(
+    sendmail: List[str],
     account: Account,
     subject: str,
     mail_message: List[str],
     debug_level: int,
     send_email: bool,
     attachments: Optional[List[Path]] = None,
 ) -> None:
@@ -42,21 +43,21 @@
         msg.add_attachment(
             attachment.read_bytes(),
             filename=attachment.name,
             maintype=main,
             subtype=sub,
         )
     p = subprocess.Popen(
-        ["/usr/sbin/sendmail", "-f", account.mail_to, "-t"],
-        stdin=subprocess.PIPE,
+        sendmail + ["-f", account.mail_to, "-t"], stdin=subprocess.PIPE
     )
     p.communicate(bytes(msg.as_string(), "UTF-8"))
 
 
 def email_clip_results(
+    sendmail: List[str],
     account: Account,
     offers: List[Offer],
     error: Optional[Error],
     clip_errors: Optional[List[ClipError]],
     debug_level: int,
     send_email: bool,
 ) -> None:
@@ -68,18 +69,21 @@
         f"Safeway account: {account.username}",
         f"Clipped {len(offers)} total:",
     ]
     for offer_type, offers_this_type in offers_by_type.items():
         mail_message.append(
             f"    {offer_type.name}: {len(offers_this_type)} coupons"
         )
-    _send_email(account, mail_subject, mail_message, debug_level, send_email)
+    _send_email(
+        sendmail, account, mail_subject, mail_message, debug_level, send_email
+    )
 
 
 def email_error(
+    sendmail: List[str],
     account: Account,
     error: Error,
     debug_level: int,
     send_email: bool,
 ) -> None:
     mail_subject = f"Safeway coupons: {error.__class__.__name__} error"
     mail_message: List[str] = [
@@ -87,14 +91,15 @@
         f"Error: {error}",
     ]
     if isinstance(error, TooManyClipErrors) and error.clipped_offers:
         mail_message += ["Clipped coupons:", ""]
         for offer in error.clipped_offers:
             mail_message += str(offer)
     _send_email(
+        sendmail,
         account,
         mail_subject,
         mail_message,
         debug_level,
         send_email,
         attachments=getattr(error, "attachments", None),
     )
```

### Comparing `safeway_coupons-0.2.3/safeway_coupons/errors.py` & `safeway_coupons-0.2.4/safeway_coupons/errors.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/safeway_coupons/methods.py` & `safeway_coupons-0.2.4/safeway_coupons/methods.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/safeway_coupons/models.py` & `safeway_coupons-0.2.4/safeway_coupons/models.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/safeway_coupons/safeway.py` & `safeway_coupons-0.2.4/safeway_coupons/safeway.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 CLIP_ERROR_MAX = 5
 
 
 class SafewayCoupons:
     def __init__(
         self,
         send_email: bool = True,
+        sendmail: Optional[List[str]] = None,
         debug_level: int = 0,
         debug_dir: Optional[Path] = None,
         sleep_level: int = 0,
         dry_run: bool = False,
         max_clip_count: int = 0,
         max_clip_errors: int = CLIP_ERROR_MAX,
     ) -> None:
         self.send_email = send_email
+        self.sendmail = sendmail or ["/usr/sbin/sendmail"]
         self.debug_level = debug_level
         self.debug_dir = debug_dir
         self.sleep_level = sleep_level
         self.dry_run = dry_run
         self.max_clip_count = max_clip_count
         self.max_clip_errors = max_clip_errors
 
@@ -78,22 +80,24 @@
                             e,
                             clipped_offers=clipped_offers,
                             errors=clip_errors,
                         )
 
             print(f"Clipped {len(clipped_offers)} coupons")
             email_clip_results(
+                self.sendmail,
                 account,
                 clipped_offers,
                 error=None,
                 clip_errors=clip_errors,
                 debug_level=self.debug_level,
                 send_email=self.send_email and not self.dry_run,
             )
         except Error as e:
             email_error(
+                self.sendmail,
                 account,
                 error=e,
                 debug_level=self.debug_level,
                 send_email=self.send_email and not self.dry_run,
             )
             raise
```

### Comparing `safeway_coupons-0.2.3/safeway_coupons/session.py` & `safeway_coupons-0.2.4/safeway_coupons/session.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/safeway_coupons/utils.py` & `safeway_coupons-0.2.4/safeway_coupons/utils.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.3/setup.py` & `safeway_coupons-0.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'webdriver-manager>=3.8.6,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['safeway-coupons = safeway_coupons.app:main']}
 
 setup_kwargs = {
     'name': 'safeway-coupons',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'Automatic coupon clipper for Safeway\'s online "Safeway for U" coupons',
-    'long_description': '# Automatic Safeway coupon clipper\n\n[![PyPI](https://img.shields.io/pypi/v/safeway-coupons)][pypi]\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/safeway-coupons)][pypi]\n[![Build](https://img.shields.io/github/checks-status/smkent/safeway-coupons/main?label=build)][gh-actions]\n[![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]\n[![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]\n\n**safeway-coupons** is a script that will log in to an account on safeway.com,\nand attempt to select all of the "Safeway for U" electronic coupons on the site\nso they don\'t have to each be clicked manually.\n\n## Design notes\n\nSafeway\'s sign in page is protected by a web application firewall (WAF).\nsafeway-coupons performs authentication using a headless instance of Google\nChrome. Authentication may fail based on your IP\'s reputation, either by\npresenting a CAPTCHA or denying sign in attempts altogether. safeway-coupons\ncurrently does not have support for prompting the user to solve CAPTCHAs.\n\nOnce a signed in session is established, coupon clipping is performed using HTTP\nrequests via [requests][requests].\n\n## Installation and usage with Docker\n\nA Docker container is provided which runs safeway-coupons with cron. The cron\nschedule and your Safeway account details may be configured using environment\nvariables, or with an accounts file.\n\nExample `docker-compose.yaml` with configuration via environment variables:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com\n      SAFEWAY_ACCOUNT_PASSWORD: very_secret\n      SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com\n      SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com\n    restart: unless-stopped\n```\n\nExample `docker-compose.yaml` with configuration via accounts file:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNTS_FILE: /accounts_file\n    restart: unless-stopped\n    volumes:\n      - path/to/safeway_accounts_file:/accounts_file:ro\n```\n\nStart the container by running:\n\n```console\ndocker-compose up -d\n```\n\nDebugging information can be viewed in the container log:\n\n```console\ndocker-compose logs -f\n```\n\n## Installation from PyPI\n\n### Prerequisites\n\n* Google Chrome (for authentication performed via Selenium).\n* Optional: `sendmail` (for email support)\n\n### Installation\n\n[safeway-coupons is available on PyPI][pypi]:\n\n```console\npip install safeway-coupons\n```\n\n### Usage\n\nFor best results, run this program once a day or so with a cron daemon.\n\nFor full usage options, run\n\n```console\nsafeway-coupons --help\n```\n\n### Configuration\n\n**safeway-coupons** can clip coupons for one or more Safeway accounts in a\nsingle run, depending on the configuration method used.\n\nIf a sender email address is configured, a summary email will be sent for each\nSafeway account via `sendmail`. The email recipient defaults to the Safeway\naccount email address, but can be overridden for each account.\n\nAccounts are searched via the following methods in the listed order. Only one\naccount configuration method may be used at a time.\n\n#### With environment variables\n\nA single Safeway account can be configured with environment variables:\n\n* `SAFEWAY_ACCOUNT_USERNAME`: Account email address (required)\n* `SAFEWAY_ACCOUNT_PASSWORD`: Account password (required)\n* `SAFEWAY_ACCOUNT_MAIL_FROM`: Sender address for email summary\n* `SAFEWAY_ACCOUNT_MAIL_TO`: Recipient address for email summary\n\n#### With config file\n\nMultiple Safeway accounts can be provided in an ini-style config file, with a\nsection for each account. For example:\n\n```ini\nemail_sender = sender@example.com   ; optional\n\n[safeway.account@example.com]       ; required\npassword = 12345                    ; required\nnotify = your.email@example.com     ; optional\n```\n\nProvide the path to your config file using the `-c` or `--accounts-config`\noption:\n\n```console\nsafeway-coupons -c path/to/config/file\n```\n\n## Development\n\n### [Poetry][poetry] installation\n\nVia [`pipx`][pipx]:\n\n```console\npip install pipx\npipx install poetry\npipx inject poetry poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\nVia `pip`:\n\n```console\npip install poetry\npoetry self add poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\n### Development tasks\n\n* Setup: `poetry install`\n* Run static checks: `poetry run poe lint` or\n  `poetry run pre-commit run --all-files`\n* Run static checks and tests: `poetry run poe test`\n\n---\n\nCreated from [smkent/cookie-python][cookie-python] using\n[cookiecutter][cookiecutter]\n\n[codecov]: https://codecov.io/gh/smkent/safeway-coupons\n[cookie-python]: https://github.com/smkent/cookie-python\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain\n[pipx]: https://pypa.github.io/pipx/\n[poetry]: https://python-poetry.org/docs/#installation\n[pypi]: https://pypi.org/project/safeway-coupons/\n[repo]: https://github.com/smkent/safeway-coupons\n[requests]: https://requests.readthedocs.io/en/latest/\n',
+    'long_description': '# Automatic Safeway coupon clipper\n\n[![PyPI](https://img.shields.io/pypi/v/safeway-coupons)][pypi]\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/safeway-coupons)][pypi]\n[![Build](https://img.shields.io/github/checks-status/smkent/safeway-coupons/main?label=build)][gh-actions]\n[![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]\n[![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]\n\n**safeway-coupons** is a script that will log in to an account on safeway.com,\nand attempt to select all of the "Safeway for U" electronic coupons on the site\nso they don\'t have to each be clicked manually.\n\n## Design notes\n\nSafeway\'s sign in page is protected by a web application firewall (WAF).\nsafeway-coupons performs authentication using a headless instance of Google\nChrome. Authentication may fail based on your IP\'s reputation, either by\npresenting a CAPTCHA or denying sign in attempts altogether. safeway-coupons\ncurrently does not have support for prompting the user to solve CAPTCHAs.\n\nOnce a signed in session is established, coupon clipping is performed using HTTP\nrequests via [requests][requests].\n\n## Installation and usage with Docker\n\nA Docker container is provided which runs safeway-coupons with cron. The cron\nschedule and your Safeway account details may be configured using environment\nvariables, or with an accounts file.\n\nExample `docker-compose.yaml` with configuration via environment variables:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM UTC each day\n      # TZ: Antarctica/McMurdo  # Optional time zone to use instead of UTC\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com\n      SAFEWAY_ACCOUNT_PASSWORD: very_secret\n      SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com\n      SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com\n      # EXTRA_ARGS: --debug  # Optional\n    restart: unless-stopped\n```\n\nExample `docker-compose.yaml` with configuration via accounts file:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM UTC each day\n      # TZ: Antarctica/McMurdo  # Optional time zone to use instead of UTC\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNTS_FILE: /accounts_file\n      # EXTRA_ARGS: --debug  # Optional\n    restart: unless-stopped\n    volumes:\n      - path/to/safeway_accounts_file:/accounts_file:ro\n```\n\nStart the container by running:\n\n```console\ndocker-compose up -d\n```\n\nDebugging information can be viewed in the container log:\n\n```console\ndocker-compose logs -f\n```\n\n## Installation from PyPI\n\n### Prerequisites\n\n* Google Chrome (for authentication performed via Selenium).\n* Optional: `sendmail` (for email support)\n\n### Installation\n\n[safeway-coupons is available on PyPI][pypi]:\n\n```console\npip install safeway-coupons\n```\n\n### Usage\n\nFor best results, run this program once a day or so with a cron daemon.\n\nFor full usage options, run\n\n```console\nsafeway-coupons --help\n```\n\n### Configuration\n\n**safeway-coupons** can clip coupons for one or more Safeway accounts in a\nsingle run, depending on the configuration method used.\n\nIf a sender email address is configured, a summary email will be sent for each\nSafeway account via `sendmail`. The email recipient defaults to the Safeway\naccount email address, but can be overridden for each account.\n\nAccounts are searched via the following methods in the listed order. Only one\naccount configuration method may be used at a time.\n\n#### With environment variables\n\nA single Safeway account can be configured with environment variables:\n\n* `SAFEWAY_ACCOUNT_USERNAME`: Account email address (required)\n* `SAFEWAY_ACCOUNT_PASSWORD`: Account password (required)\n* `SAFEWAY_ACCOUNT_MAIL_FROM`: Sender address for email summary\n* `SAFEWAY_ACCOUNT_MAIL_TO`: Recipient address for email summary\n\n#### With config file\n\nMultiple Safeway accounts can be provided in an ini-style config file, with a\nsection for each account. For example:\n\n```ini\nemail_sender = sender@example.com   ; optional\n\n[safeway.account@example.com]       ; required\npassword = 12345                    ; required\nnotify = your.email@example.com     ; optional\n```\n\nProvide the path to your config file using the `-c` or `--accounts-config`\noption:\n\n```console\nsafeway-coupons -c path/to/config/file\n```\n\n## Development\n\n### [Poetry][poetry] installation\n\nVia [`pipx`][pipx]:\n\n```console\npip install pipx\npipx install poetry\npipx inject poetry poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\nVia `pip`:\n\n```console\npip install poetry\npoetry self add poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\n### Development tasks\n\n* Setup: `poetry install`\n* Run static checks: `poetry run poe lint` or\n  `poetry run pre-commit run --all-files`\n* Run static checks and tests: `poetry run poe test`\n\n---\n\nCreated from [smkent/cookie-python][cookie-python] using\n[cookiecutter][cookiecutter]\n\n[codecov]: https://codecov.io/gh/smkent/safeway-coupons\n[cookie-python]: https://github.com/smkent/cookie-python\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain\n[pipx]: https://pypa.github.io/pipx/\n[poetry]: https://python-poetry.org/docs/#installation\n[pypi]: https://pypi.org/project/safeway-coupons/\n[repo]: https://github.com/smkent/safeway-coupons\n[requests]: https://requests.readthedocs.io/en/latest/\n',
     'author': 'Stephen Kent',
     'author_email': 'smkent@smkent.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smkent/safeway-coupons',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `safeway_coupons-0.2.3/PKG-INFO` & `safeway_coupons-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safeway-coupons
-Version: 0.2.3
+Version: 0.2.4
 Summary: Automatic coupon clipper for Safeway's online "Safeway for U" coupons
 Home-page: https://github.com/smkent/safeway-coupons
 License: GPL-3.0-or-later
 Author: Stephen Kent
 Author-email: smkent@smkent.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -59,35 +59,39 @@
 ```yaml
 version: "3.7"
 
 services:
   safeway-coupons:
     image: ghcr.io/smkent/safeway-coupons:latest
     environment:
-      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day
+      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM UTC each day
+      # TZ: Antarctica/McMurdo  # Optional time zone to use instead of UTC
       SMTPHOST: your.smtp.host
       SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com
       SAFEWAY_ACCOUNT_PASSWORD: very_secret
       SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com
       SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com
+      # EXTRA_ARGS: --debug  # Optional
     restart: unless-stopped
 ```
 
 Example `docker-compose.yaml` with configuration via accounts file:
 
 ```yaml
 version: "3.7"
 
 services:
   safeway-coupons:
     image: ghcr.io/smkent/safeway-coupons:latest
     environment:
-      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day
+      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM UTC each day
+      # TZ: Antarctica/McMurdo  # Optional time zone to use instead of UTC
       SMTPHOST: your.smtp.host
       SAFEWAY_ACCOUNTS_FILE: /accounts_file
+      # EXTRA_ARGS: --debug  # Optional
     restart: unless-stopped
     volumes:
       - path/to/safeway_accounts_file:/accounts_file:ro
 ```
 
 Start the container by running:
```

