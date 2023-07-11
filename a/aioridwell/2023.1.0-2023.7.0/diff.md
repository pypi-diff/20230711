# Comparing `tmp/aioridwell-2023.1.0.tar.gz` & `tmp/aioridwell-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioridwell-2023.1.0.tar", max compression
+gzip compressed data, was "aioridwell-2023.7.0.tar", max compression
```

## Comparing `aioridwell-2023.1.0.tar` & `aioridwell-2023.7.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-01-09 04:21:03.611616 aioridwell-2023.1.0/LICENSE
--rw-r--r--   0        0        0     7089 2023-01-09 04:21:03.611616 aioridwell-2023.1.0/README.md
--rw-r--r--   0        0        0       83 2023-01-09 04:21:03.611616 aioridwell-2023.1.0/aioridwell/__init__.py
--rw-r--r--   0        0        0     6991 2023-01-09 04:21:03.611616 aioridwell-2023.1.0/aioridwell/client.py
--rw-r--r--   0        0        0       88 2023-01-09 04:21:03.611616 aioridwell-2023.1.0/aioridwell/const.py
--rw-r--r--   0        0        0     1212 2023-01-09 04:21:03.615616 aioridwell-2023.1.0/aioridwell/errors.py
--rw-r--r--   0        0        0     7879 2023-01-09 04:21:03.615616 aioridwell-2023.1.0/aioridwell/model.py
--rw-r--r--   0        0        0        0 2023-01-09 04:21:03.615616 aioridwell-2023.1.0/aioridwell/py.typed
--rw-r--r--   0        0        0     1384 2023-01-09 04:21:03.615616 aioridwell-2023.1.0/aioridwell/query.py
--rw-r--r--   0        0        0     3847 2023-01-09 04:21:03.615616 aioridwell-2023.1.0/pyproject.toml
--rw-r--r--   0        0        0     8088 1970-01-01 00:00:00.000000 aioridwell-2023.1.0/setup.py
--rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 aioridwell-2023.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     7089 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/README.md
+-rw-r--r--   0        0        0       83 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/__init__.py
+-rw-r--r--   0        0        0     7062 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/client.py
+-rw-r--r--   0        0        0       88 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/const.py
+-rw-r--r--   0        0        0     1212 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/errors.py
+-rw-r--r--   0        0        0     7911 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/model.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/py.typed
+-rw-r--r--   0        0        0     1384 2023-07-11 15:19:19.897130 aioridwell-2023.7.0/aioridwell/query.py
+-rw-r--r--   0        0        0     3657 2023-07-11 15:19:19.901130 aioridwell-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8188 1970-01-01 00:00:00.000000 aioridwell-2023.7.0/PKG-INFO
```

### Comparing `aioridwell-2023.1.0/LICENSE` & `aioridwell-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioridwell-2023.1.0/README.md` & `aioridwell-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aioridwell-2023.1.0/aioridwell/client.py` & `aioridwell-2023.7.0/aioridwell/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Define an API client."""
 from __future__ import annotations
 
 import asyncio
-from typing import Any
+from typing import Any, cast
 
 import jwt
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientError
 
 from .const import LOGGER
 from .errors import (
@@ -30,19 +30,22 @@
 
     Args:
         encoded_jwt: An encoded JWT.
 
     Returns:
         A decoded JWT.
     """
-    return jwt.decode(
-        encoded_jwt,
-        "secret",
-        algorithms=["HS256"],
-        options={"verify_signature": False},
+    return cast(
+        dict[str, Any],
+        jwt.decode(
+            encoded_jwt,
+            "secret",
+            algorithms=["HS256"],
+            options={"verify_signature": False},
+        ),
     )
 
 
 class Client:
     """Define the client."""
 
     def __init__(
```

### Comparing `aioridwell-2023.1.0/aioridwell/errors.py` & `aioridwell-2023.7.0/aioridwell/errors.py`

 * *Files identical despite different names*

### Comparing `aioridwell-2023.1.0/aioridwell/model.py` & `aioridwell-2023.7.0/aioridwell/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 PICKUP_CATEGORIES_MAP = {
     "Batteries": PickupCategory.STANDARD,
     "Beyond the Bin": PickupCategory.ADD_ON,
     "Fluorescent Light Tubes": PickupCategory.ADD_ON,
     "Latex Paint": PickupCategory.ADD_ON,
     "Light Bulbs": PickupCategory.STANDARD,
+    "Multi-Layer Plastic": PickupCategory.STANDARD,
     "Paint": PickupCategory.ADD_ON,
     "Plastic Film": PickupCategory.STANDARD,
     "Styrofoam": PickupCategory.ADD_ON,
     "Threads": PickupCategory.STANDARD,
 }
 
 
@@ -155,20 +156,19 @@
     category: PickupCategory = field(init=False)
 
     def __post_init__(self) -> None:
         """Perform some post-init init."""
         category = PICKUP_CATEGORIES_MAP.get(self.name, PickupCategory.ROTATING)
 
         if category == PickupCategory.ROTATING:
-            # Since our method of detecting rotating pickups is pretty "loose" (i.e.,
-            # if a category isn't a known standard or add-on, we assume it's rotating).
-            # This could lead to future issues if Ridwell introduces a new standard
-            # or add-on type that isn't mapped here. We try to be unintrusive and
-            # merely log that we've found a "rotating" pickup so that it can later tell
-            # the full story:
+            # Our method of detecting rotating pickups is pretty "loose" (i.e., if a
+            # category isn't a known standard or add-on, we assume it's rotating). This
+            # could lead to future issues if Ridwell introduces a new standard or add-on
+            # type that isn't mapped here. We try to be unintrusive and merely log that
+            # we've found a "rotating" pickup so that it can later tell the full story:
             LOGGER.info("Detected assumed rotating pickup: %s", self.name)
 
         object.__setattr__(
             self,
             "category",
             PICKUP_CATEGORIES_MAP.get(self.name, PickupCategory.ROTATING),
         )
```

### Comparing `aioridwell-2023.1.0/aioridwell/query.py` & `aioridwell-2023.7.0/aioridwell/query.py`

 * *Files identical despite different names*

### Comparing `aioridwell-2023.1.0/pyproject.toml` & `aioridwell-2023.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "aioridwell"
-version = "2023.01.0"
+version = "2023.07.0"
 description = "A Python3, asyncio-based API for interacting with Ridwell waste recycling"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/aioridwell"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -64,41 +64,33 @@
 python = "^3.9.0"
 pytz = ">=2021.3"
 titlecase = "^2.3"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "^2.1.6"
 bandit = "^1.7.4"
-black = "^22.10.0"
+black = ">=22.10,<24.0"
 blacken-docs = "^1.12.1"
 codespell = "^2.2.2"
-coverage = {version = "^6.5", extras = ["toml"]}
+coverage = {version = ">=6.5,<8.0", extras = ["toml"]}
 darglint = "^1.8.1"
-flake8 = "^4.0.1"
-flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.10.27"
-flake8-builtins = "^2.0.0"
-flake8-comprehensions = "^3.10.0"
-flake8-docstrings = "^1.5.0"
-flake8-eradicate = "^1.4.0"
-flake8-markdown = "^0.3.0"
-flake8-simplify = "^0.19.3"
 freezegun = "^1.1.0"
 isort = "^5.10.1"
-mypy = "^0.982"
-pre-commit = "^2.20.0"
+mypy = "^1.2.0"
+pre-commit = ">=2.20,<4.0"
 pre-commit-hooks = "^4.3.0"
 pylint = "^2.15.5"
 pytest = "^7.2.0"
 pytest-aiohttp = "^1.0.0"
-pytest-asyncio = "^0.20.1"
+pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-cov = "^4.0.0"
 pyupgrade = "^3.1.0"
+ruff = ">=0.0.261,<0.0.278"
 safety = "^2.3.1"
-types-pytz = "^2022.0.0"
+types-pytz = ">=2022,<2024"
 vulture = "^2.6"
 yamllint = "^1.28.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/bachya/aioridwell/issues"
 Changelog = "https://github.com/bachya/aioridwell/releases"
```

### Comparing `aioridwell-2023.1.0/setup.py` & `aioridwell-2023.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,270 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aioridwell
+Version: 2023.7.0
+Summary: A Python3, asyncio-based API for interacting with Ridwell waste recycling
+Home-page: https://github.com/bachya/aioridwell
+License: MIT
+Author: Aaron Bach
+Author-email: bachya1208@gmail.com
+Requires-Python: >=3.9.0,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: PyJWT (>=2.4.0)
+Requires-Dist: aiohttp (>=3.8.0)
+Requires-Dist: pytz (>=2021.3)
+Requires-Dist: titlecase (>=2.3,<3.0)
+Project-URL: Bug Tracker, https://github.com/bachya/aioridwell/issues
+Project-URL: Changelog, https://github.com/bachya/aioridwell/releases
+Project-URL: Repository, https://github.com/bachya/aioridwell
+Description-Content-Type: text/markdown
 
-packages = \
-['aioridwell']
+# ♻️ aioridwell: A Python3, asyncio-based API for interacting with Ridwell
 
-package_data = \
-{'': ['*']}
+[![CI][ci-badge]][ci]
+[![PyPI][pypi-badge]][pypi]
+[![Version][version-badge]][version]
+[![License][license-badge]][license]
+[![Code Coverage][codecov-badge]][codecov]
+[![Maintainability][maintainability-badge]][maintainability]
 
-install_requires = \
-['PyJWT>=2.4.0', 'aiohttp>=3.8.0', 'pytz>=2021.3', 'titlecase>=2.3,<3.0']
-
-setup_kwargs = {
-    'name': 'aioridwell',
-    'version': '2023.1.0',
-    'description': 'A Python3, asyncio-based API for interacting with Ridwell waste recycling',
-    'long_description': '# ♻️ aioridwell: A Python3, asyncio-based API for interacting with Ridwell\n\n[![CI][ci-badge]][ci]\n[![PyPI][pypi-badge]][pypi]\n[![Version][version-badge]][version]\n[![License][license-badge]][license]\n[![Code Coverage][codecov-badge]][codecov]\n[![Maintainability][maintainability-badge]][maintainability]\n\n<a href="https://www.buymeacoffee.com/bachya1208P" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>\n\n`aioridwell` is a Python 3, asyncio-friendly library for interacting with\n[Ridwell][ridwell] to view information on upcoming recycling pickups.\n\n- [Installation](#installation)\n- [Python Versions](#python-versions)\n- [Usage](#usage)\n- [Contributing](#contributing)\n\n# Installation\n\n```bash\npip install aioridwell\n```\n\n# Python Versions\n\n`aioridwell` is currently supported on:\n\n- Python 3.9\n- Python 3.10\n- Python 3.11\n\n# Usage\n\n## Creating and Using a Client\n\nThe `Client` is the primary method of interacting with the API:\n\n```python\nimport asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -> None:\n    client = await async_get_client("<EMAIL>", "<PASSWORD>")\n    # ...\n\n\nasyncio.run(main())\n```\n\nBy default, the library creates a new connection to the API with each coroutine. If\nyou are calling a large number of coroutines (or merely want to squeeze out every second\nof runtime savings possible), an [`aiohttp`][aiohttp] `ClientSession` can be used for\nconnection pooling:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom aiowatttime import Client\n\n\nasync def main() -> None:\n    async with ClientSession() as session:\n        client = await async_get_client("<EMAIL>", "<PASSWORD>", session=session)\n        # ...\n\n\nasyncio.run(main())\n```\n\n## Getting the User\'s Dashboard URL\n\n```python\nimport asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -> None:\n    client = await async_get_client("<EMAIL>", "<PASSWORD>")\n    client.get_dashboard_url()\n    # >>> https://www.ridwell.com/users/userId1/dashboard\n\n\nasyncio.run(main())\n```\n\n## Getting Accounts\n\nGetting all accounts associated with this email address is easy:\n\n```python\nimport asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -> None:\n    client = await async_get_client("<EMAIL>", "<PASSWORD>")\n\n    accounts = await client.async_get_accounts()\n    # >>> {"account_id_1": RidwellAccount(...), ...}\n\n\nasyncio.run(main())\n```\n\nThe `RidwellAccount` object comes with some useful properties:\n\n- `account_id`: the Ridwell ID for the account\n- `address`: the address being serviced\n- `email`: the email address on the account\n- `full_name`: the full name of the account owner\n- `phone`: the phone number of the account owner\n- `subscription_id`: the Ridwell ID for the primary subscription\n- `subscription_active`: whether the primary subscription is active\n\n## Getting Pickup Events\n\nGetting pickup events associated with an account is easy, too:\n\n```python\nimport asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -> None:\n    client = await async_get_client("<EMAIL>", "<PASSWORD>")\n\n    accounts = await client.async_get_accounts()\n    for account in accounts.values():\n        events = await account.async_get_pickup_events()\n        # >>> [RidwellPickupEvent(...), ...]\n\n        # You can also get just the next pickup event from today\'s date:\n        next_event = await account.async_get_next_pickup_event()\n        # >>> RidwellPickupEvent(...)\n\n\nasyncio.run(main())\n```\n\nThe `RidwellPickupEvent` object comes with some useful properties:\n\n- `pickup_date`: the date of the pickup (in `datetime.date` format)\n- `pickups`: a list of `RidwellPickup` objects\n- `state`: an `EventState` enum whose name represents the current state of the pickup event\n\nLikewise, the `RidwellPickup` object comes with some useful properties:\n\n- `category`: a `PickupCategory` enum whose name represents the type of pickup\n- `name`: the name of the item being picked up\n- `offer_id`: the Ridwell ID for this particular offer\n- `priority`: the pickup priority\n- `product_id`: the Ridwell ID for this particular product\n- `quantity`: the amount of the product being picked up\n\n### Opting Into or Out Of a Pickup Event\n\n```python\nimport asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -> None:\n    client = await async_get_client("<EMAIL>", "<PASSWORD>")\n\n    accounts = await client.async_get_accounts()\n    for account in accounts.values():\n        events = await account.async_get_pickup_events()\n        # >>> [RidwellPickupEvent(...), ...]\n\n        await events[0].async_opt_in()\n        await events[0].async_opt_out()\n\n\nasyncio.run(main())\n```\n\n### Calculating a Pickup Event\'s Estimated Cost\n\n```python\nimport asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -> None:\n    client = await async_get_client("<EMAIL>", "<PASSWORD>")\n\n    accounts = await client.async_get_accounts()\n    for account in accounts.values():\n        events = await account.async_get_pickup_events()\n        # >>> [RidwellPickupEvent(...), ...]\n\n        event_1_cost = await events[0].async_get_estimated_cost()\n        # >>> 22.00\n\n\nasyncio.run(main())\n```\n\n# Contributing\n\nThanks to all of [our contributors][contributors] so far!\n\n1. [Check for open features/bugs][issues] or [initiate a discussion on one][new-issue].\n2. [Fork the repository][fork].\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix on a new branch.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `poetry run pytest --cov aioridwell tests`\n9. Update `README.md` with any new documentation.\n10. Submit a pull request!\n\n[aiohttp]: https://github.com/aio-libs/aiohttp\n[ci-badge]: https://github.com/bachya/aioridwell/workflows/CI/badge.svg\n[ci]: https://github.com/bachya/aioridwell/actions\n[codecov-badge]: https://codecov.io/gh/bachya/aioridwell/branch/dev/graph/badge.svg\n[codecov]: https://codecov.io/gh/bachya/aioridwell\n[contributors]: https://github.com/bachya/aioridwell/graphs/contributors\n[fork]: https://github.com/bachya/aioridwell/fork\n[issues]: https://github.com/bachya/aioridwell/issues\n[license-badge]: https://img.shields.io/pypi/l/aioridwell.svg\n[license]: https://github.com/bachya/aioridwell/blob/main/LICENSE\n[maintainability-badge]: https://api.codeclimate.com/v1/badges/9c1dcc1c991cecb06eda/maintainability\n[maintainability]: https://codeclimate.com/github/bachya/aioridwell/maintainability\n[new-issue]: https://github.com/bachya/aioridwell/issues/new\n[new-issue]: https://github.com/bachya/aioridwell/issues/new\n[pypi-badge]: https://img.shields.io/pypi/v/aioridwell.svg\n[pypi]: https://pypi.python.org/pypi/aioridwell\n[ridwell]: https://ridwell.com\n[version-badge]: https://img.shields.io/pypi/pyversions/aioridwell.svg\n[version]: https://pypi.python.org/pypi/aioridwell\n',
-    'author': 'Aaron Bach',
-    'author_email': 'bachya1208@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/bachya/aioridwell',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9.0,<4.0.0',
-}
+<a href="https://www.buymeacoffee.com/bachya1208P" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
+`aioridwell` is a Python 3, asyncio-friendly library for interacting with
+[Ridwell][ridwell] to view information on upcoming recycling pickups.
+
+- [Installation](#installation)
+- [Python Versions](#python-versions)
+- [Usage](#usage)
+- [Contributing](#contributing)
+
+# Installation
+
+```bash
+pip install aioridwell
+```
+
+# Python Versions
+
+`aioridwell` is currently supported on:
+
+- Python 3.9
+- Python 3.10
+- Python 3.11
+
+# Usage
+
+## Creating and Using a Client
+
+The `Client` is the primary method of interacting with the API:
+
+```python
+import asyncio
+
+from aioridwell import async_get_client
+
+
+async def main() -> None:
+    client = await async_get_client("<EMAIL>", "<PASSWORD>")
+    # ...
+
+
+asyncio.run(main())
+```
+
+By default, the library creates a new connection to the API with each coroutine. If
+you are calling a large number of coroutines (or merely want to squeeze out every second
+of runtime savings possible), an [`aiohttp`][aiohttp] `ClientSession` can be used for
+connection pooling:
+
+```python
+import asyncio
+
+from aiohttp import ClientSession
+
+from aiowatttime import Client
+
+
+async def main() -> None:
+    async with ClientSession() as session:
+        client = await async_get_client("<EMAIL>", "<PASSWORD>", session=session)
+        # ...
+
+
+asyncio.run(main())
+```
+
+## Getting the User's Dashboard URL
+
+```python
+import asyncio
+
+from aioridwell import async_get_client
+
+
+async def main() -> None:
+    client = await async_get_client("<EMAIL>", "<PASSWORD>")
+    client.get_dashboard_url()
+    # >>> https://www.ridwell.com/users/userId1/dashboard
+
+
+asyncio.run(main())
+```
+
+## Getting Accounts
+
+Getting all accounts associated with this email address is easy:
+
+```python
+import asyncio
+
+from aioridwell import async_get_client
+
+
+async def main() -> None:
+    client = await async_get_client("<EMAIL>", "<PASSWORD>")
+
+    accounts = await client.async_get_accounts()
+    # >>> {"account_id_1": RidwellAccount(...), ...}
+
+
+asyncio.run(main())
+```
+
+The `RidwellAccount` object comes with some useful properties:
+
+- `account_id`: the Ridwell ID for the account
+- `address`: the address being serviced
+- `email`: the email address on the account
+- `full_name`: the full name of the account owner
+- `phone`: the phone number of the account owner
+- `subscription_id`: the Ridwell ID for the primary subscription
+- `subscription_active`: whether the primary subscription is active
+
+## Getting Pickup Events
+
+Getting pickup events associated with an account is easy, too:
+
+```python
+import asyncio
+
+from aioridwell import async_get_client
+
+
+async def main() -> None:
+    client = await async_get_client("<EMAIL>", "<PASSWORD>")
+
+    accounts = await client.async_get_accounts()
+    for account in accounts.values():
+        events = await account.async_get_pickup_events()
+        # >>> [RidwellPickupEvent(...), ...]
+
+        # You can also get just the next pickup event from today's date:
+        next_event = await account.async_get_next_pickup_event()
+        # >>> RidwellPickupEvent(...)
+
+
+asyncio.run(main())
+```
+
+The `RidwellPickupEvent` object comes with some useful properties:
+
+- `pickup_date`: the date of the pickup (in `datetime.date` format)
+- `pickups`: a list of `RidwellPickup` objects
+- `state`: an `EventState` enum whose name represents the current state of the pickup event
+
+Likewise, the `RidwellPickup` object comes with some useful properties:
+
+- `category`: a `PickupCategory` enum whose name represents the type of pickup
+- `name`: the name of the item being picked up
+- `offer_id`: the Ridwell ID for this particular offer
+- `priority`: the pickup priority
+- `product_id`: the Ridwell ID for this particular product
+- `quantity`: the amount of the product being picked up
+
+### Opting Into or Out Of a Pickup Event
+
+```python
+import asyncio
+
+from aioridwell import async_get_client
+
+
+async def main() -> None:
+    client = await async_get_client("<EMAIL>", "<PASSWORD>")
+
+    accounts = await client.async_get_accounts()
+    for account in accounts.values():
+        events = await account.async_get_pickup_events()
+        # >>> [RidwellPickupEvent(...), ...]
+
+        await events[0].async_opt_in()
+        await events[0].async_opt_out()
+
+
+asyncio.run(main())
+```
+
+### Calculating a Pickup Event's Estimated Cost
+
+```python
+import asyncio
+
+from aioridwell import async_get_client
+
+
+async def main() -> None:
+    client = await async_get_client("<EMAIL>", "<PASSWORD>")
+
+    accounts = await client.async_get_accounts()
+    for account in accounts.values():
+        events = await account.async_get_pickup_events()
+        # >>> [RidwellPickupEvent(...), ...]
+
+        event_1_cost = await events[0].async_get_estimated_cost()
+        # >>> 22.00
+
+
+asyncio.run(main())
+```
+
+# Contributing
+
+Thanks to all of [our contributors][contributors] so far!
+
+1. [Check for open features/bugs][issues] or [initiate a discussion on one][new-issue].
+2. [Fork the repository][fork].
+3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`
+4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`
+5. Install the dev environment: `script/setup`
+6. Code your new feature or bug fix on a new branch.
+7. Write tests that cover your new functionality.
+8. Run tests and ensure 100% code coverage: `poetry run pytest --cov aioridwell tests`
+9. Update `README.md` with any new documentation.
+10. Submit a pull request!
+
+[aiohttp]: https://github.com/aio-libs/aiohttp
+[ci-badge]: https://github.com/bachya/aioridwell/workflows/CI/badge.svg
+[ci]: https://github.com/bachya/aioridwell/actions
+[codecov-badge]: https://codecov.io/gh/bachya/aioridwell/branch/dev/graph/badge.svg
+[codecov]: https://codecov.io/gh/bachya/aioridwell
+[contributors]: https://github.com/bachya/aioridwell/graphs/contributors
+[fork]: https://github.com/bachya/aioridwell/fork
+[issues]: https://github.com/bachya/aioridwell/issues
+[license-badge]: https://img.shields.io/pypi/l/aioridwell.svg
+[license]: https://github.com/bachya/aioridwell/blob/main/LICENSE
+[maintainability-badge]: https://api.codeclimate.com/v1/badges/9c1dcc1c991cecb06eda/maintainability
+[maintainability]: https://codeclimate.com/github/bachya/aioridwell/maintainability
+[new-issue]: https://github.com/bachya/aioridwell/issues/new
+[new-issue]: https://github.com/bachya/aioridwell/issues/new
+[pypi-badge]: https://img.shields.io/pypi/v/aioridwell.svg
+[pypi]: https://pypi.python.org/pypi/aioridwell
+[ridwell]: https://ridwell.com
+[version-badge]: https://img.shields.io/pypi/pyversions/aioridwell.svg
+[version]: https://pypi.python.org/pypi/aioridwell
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,103 +1,102 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['aioridwell'] package_data = \ {'': ['*']} install_requires = \
-['PyJWT>=2.4.0', 'aiohttp>=3.8.0', 'pytz>=2021.3', 'titlecase>=2.3,<3.0']
-setup_kwargs = { 'name': 'aioridwell', 'version': '2023.1.0', 'description': 'A
-Python3, asyncio-based API for interacting with Ridwell waste recycling',
-'long_description': '# â»ï¸ aioridwell: A Python3, asyncio-based API for
-interacting with Ridwell\n\n[![CI][ci-badge]][ci]\n[![PyPI][pypi-badge]]
-[pypi]\n[![Version][version-badge]][version]\n[![License][license-badge]]
-[license]\n[![Code Coverage][codecov-badge]][codecov]\n[![Maintainability]
-[maintainability-badge]][maintainability]\n\n[Buy_Me_A_Coffee]\n\n`aioridwell`
-is a Python 3, asyncio-friendly library for interacting with\n[Ridwell]
-[ridwell] to view information on upcoming recycling pickups.\n\n-
-[Installation](#installation)\n- [Python Versions](#python-versions)\n- [Usage]
-(#usage)\n- [Contributing](#contributing)\n\n# Installation\n\n```bash\npip
-install aioridwell\n```\n\n# Python Versions\n\n`aioridwell` is currently
-supported on:\n\n- Python 3.9\n- Python 3.10\n- Python 3.11\n\n# Usage\n\n##
-Creating and Using a Client\n\nThe `Client` is the primary method of
-interacting with the API:\n\n```python\nimport asyncio\n\nfrom aioridwell
-import async_get_client\n\n\nasync def main() -> None:\n client = await
-async_get_client("", "")\n # ...\n\n\nasyncio.run(main())\n```\n\nBy default,
-the library creates a new connection to the API with each coroutine. If\nyou
-are calling a large number of coroutines (or merely want to squeeze out every
-second\nof runtime savings possible), an [`aiohttp`][aiohttp] `ClientSession`
-can be used for\nconnection pooling:\n\n```python\nimport asyncio\n\nfrom
-aiohttp import ClientSession\n\nfrom aiowatttime import Client\n\n\nasync def
-main() -> None:\n async with ClientSession() as session:\n client = await
-async_get_client("", "", session=session)\n # ...\n\n\nasyncio.run(main
-())\n```\n\n## Getting the User\'s Dashboard URL\n\n```python\nimport
-asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -
-> None:\n client = await async_get_client("", "")\n client.get_dashboard_url
-()\n # >>> https://www.ridwell.com/users/userId1/dashboard\n\n\nasyncio.run
-(main())\n```\n\n## Getting Accounts\n\nGetting all accounts associated with
-this email address is easy:\n\n```python\nimport asyncio\n\nfrom aioridwell
-import async_get_client\n\n\nasync def main() -> None:\n client = await
-async_get_client("", "")\n\n accounts = await client.async_get_accounts()\n #
->>> {"account_id_1": RidwellAccount(...), ...}\n\n\nasyncio.run(main
-())\n```\n\nThe `RidwellAccount` object comes with some useful properties:\n\n-
-`account_id`: the Ridwell ID for the account\n- `address`: the address being
-serviced\n- `email`: the email address on the account\n- `full_name`: the full
-name of the account owner\n- `phone`: the phone number of the account owner\n-
-`subscription_id`: the Ridwell ID for the primary subscription\n-
-`subscription_active`: whether the primary subscription is active\n\n## Getting
-Pickup Events\n\nGetting pickup events associated with an account is easy, too:
-\n\n```python\nimport asyncio\n\nfrom aioridwell import
-async_get_client\n\n\nasync def main() -> None:\n client = await
-async_get_client("", "")\n\n accounts = await client.async_get_accounts()\n for
-account in accounts.values():\n events = await account.async_get_pickup_events
-()\n # >>> [RidwellPickupEvent(...), ...]\n\n # You can also get just the next
-pickup event from today\'s date:\n next_event = await
-account.async_get_next_pickup_event()\n # >>> RidwellPickupEvent
-(...)\n\n\nasyncio.run(main())\n```\n\nThe `RidwellPickupEvent` object comes
-with some useful properties:\n\n- `pickup_date`: the date of the pickup (in
-`datetime.date` format)\n- `pickups`: a list of `RidwellPickup` objects\n-
-`state`: an `EventState` enum whose name represents the current state of the
-pickup event\n\nLikewise, the `RidwellPickup` object comes with some useful
-properties:\n\n- `category`: a `PickupCategory` enum whose name represents the
-type of pickup\n- `name`: the name of the item being picked up\n- `offer_id`:
-the Ridwell ID for this particular offer\n- `priority`: the pickup priority\n-
-`product_id`: the Ridwell ID for this particular product\n- `quantity`: the
-amount of the product being picked up\n\n### Opting Into or Out Of a Pickup
-Event\n\n```python\nimport asyncio\n\nfrom aioridwell import
-async_get_client\n\n\nasync def main() -> None:\n client = await
-async_get_client("", "")\n\n accounts = await client.async_get_accounts()\n for
-account in accounts.values():\n events = await account.async_get_pickup_events
-()\n # >>> [RidwellPickupEvent(...), ...]\n\n await events[0].async_opt_in()\n
-await events[0].async_opt_out()\n\n\nasyncio.run(main())\n```\n\n###
-Calculating a Pickup Event\'s Estimated Cost\n\n```python\nimport
-asyncio\n\nfrom aioridwell import async_get_client\n\n\nasync def main() -
-> None:\n client = await async_get_client("", "")\n\n accounts = await
-client.async_get_accounts()\n for account in accounts.values():\n events =
-await account.async_get_pickup_events()\n # >>> [RidwellPickupEvent(...),
-...]\n\n event_1_cost = await events[0].async_get_estimated_cost()\n # >>>
-22.00\n\n\nasyncio.run(main())\n```\n\n# Contributing\n\nThanks to all of [our
-contributors][contributors] so far!\n\n1. [Check for open features/bugs]
-[issues] or [initiate a discussion on one][new-issue].\n2. [Fork the
-repository][fork].\n3. (_optional, but highly recommended_) Create a virtual
-environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_)
-Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the
-dev environment: `script/setup`\n6. Code your new feature or bug fix on a new
-branch.\n7. Write tests that cover your new functionality.\n8. Run tests and
-ensure 100% code coverage: `poetry run pytest --cov aioridwell tests`\n9.
-Update `README.md` with any new documentation.\n10. Submit a pull request!\n\n
-[aiohttp]: https://github.com/aio-libs/aiohttp\n[ci-badge]: https://github.com/
-bachya/aioridwell/workflows/CI/badge.svg\n[ci]: https://github.com/bachya/
-aioridwell/actions\n[codecov-badge]: https://codecov.io/gh/bachya/aioridwell/
-branch/dev/graph/badge.svg\n[codecov]: https://codecov.io/gh/bachya/
-aioridwell\n[contributors]: https://github.com/bachya/aioridwell/graphs/
-contributors\n[fork]: https://github.com/bachya/aioridwell/fork\n[issues]:
-https://github.com/bachya/aioridwell/issues\n[license-badge]: https://
-img.shields.io/pypi/l/aioridwell.svg\n[license]: https://github.com/bachya/
-aioridwell/blob/main/LICENSE\n[maintainability-badge]: https://
-api.codeclimate.com/v1/badges/9c1dcc1c991cecb06eda/maintainability\n
+Metadata-Version: 2.1 Name: aioridwell Version: 2023.7.0 Summary: A Python3,
+asyncio-based API for interacting with Ridwell waste recycling Home-page:
+https://github.com/bachya/aioridwell License: MIT Author: Aaron Bach Author-
+email: bachya1208@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Requires-Dist: PyJWT (>=2.4.0)
+Requires-Dist: aiohttp (>=3.8.0) Requires-Dist: pytz (>=2021.3) Requires-Dist:
+titlecase (>=2.3,<3.0) Project-URL: Bug Tracker, https://github.com/bachya/
+aioridwell/issues Project-URL: Changelog, https://github.com/bachya/aioridwell/
+releases Project-URL: Repository, https://github.com/bachya/aioridwell
+Description-Content-Type: text/markdown # â»ï¸ aioridwell: A Python3,
+asyncio-based API for interacting with Ridwell [![CI][ci-badge]][ci] [![PyPI]
+[pypi-badge]][pypi] [![Version][version-badge]][version] [![License][license-
+badge]][license] [![Code Coverage][codecov-badge]][codecov] [![Maintainability]
+[maintainability-badge]][maintainability] [Buy_Me_A_Coffee] `aioridwell` is a
+Python 3, asyncio-friendly library for interacting with [Ridwell][ridwell] to
+view information on upcoming recycling pickups. - [Installation](#installation)
+- [Python Versions](#python-versions) - [Usage](#usage) - [Contributing]
+(#contributing) # Installation ```bash pip install aioridwell ``` # Python
+Versions `aioridwell` is currently supported on: - Python 3.9 - Python 3.10 -
+Python 3.11 # Usage ## Creating and Using a Client The `Client` is the primary
+method of interacting with the API: ```python import asyncio from aioridwell
+import async_get_client async def main() -> None: client = await
+async_get_client("", "") # ... asyncio.run(main()) ``` By default, the library
+creates a new connection to the API with each coroutine. If you are calling a
+large number of coroutines (or merely want to squeeze out every second of
+runtime savings possible), an [`aiohttp`][aiohttp] `ClientSession` can be used
+for connection pooling: ```python import asyncio from aiohttp import
+ClientSession from aiowatttime import Client async def main() -> None: async
+with ClientSession() as session: client = await async_get_client("", "",
+session=session) # ... asyncio.run(main()) ``` ## Getting the User's Dashboard
+URL ```python import asyncio from aioridwell import async_get_client async def
+main() -> None: client = await async_get_client("", "")
+client.get_dashboard_url() # >>> https://www.ridwell.com/users/userId1/
+dashboard asyncio.run(main()) ``` ## Getting Accounts Getting all accounts
+associated with this email address is easy: ```python import asyncio from
+aioridwell import async_get_client async def main() -> None: client = await
+async_get_client("", "") accounts = await client.async_get_accounts() # >>>
+{"account_id_1": RidwellAccount(...), ...} asyncio.run(main()) ``` The
+`RidwellAccount` object comes with some useful properties: - `account_id`: the
+Ridwell ID for the account - `address`: the address being serviced - `email`:
+the email address on the account - `full_name`: the full name of the account
+owner - `phone`: the phone number of the account owner - `subscription_id`: the
+Ridwell ID for the primary subscription - `subscription_active`: whether the
+primary subscription is active ## Getting Pickup Events Getting pickup events
+associated with an account is easy, too: ```python import asyncio from
+aioridwell import async_get_client async def main() -> None: client = await
+async_get_client("", "") accounts = await client.async_get_accounts() for
+account in accounts.values(): events = await account.async_get_pickup_events()
+# >>> [RidwellPickupEvent(...), ...] # You can also get just the next pickup
+event from today's date: next_event = await account.async_get_next_pickup_event
+() # >>> RidwellPickupEvent(...) asyncio.run(main()) ``` The
+`RidwellPickupEvent` object comes with some useful properties: - `pickup_date`:
+the date of the pickup (in `datetime.date` format) - `pickups`: a list of
+`RidwellPickup` objects - `state`: an `EventState` enum whose name represents
+the current state of the pickup event Likewise, the `RidwellPickup` object
+comes with some useful properties: - `category`: a `PickupCategory` enum whose
+name represents the type of pickup - `name`: the name of the item being picked
+up - `offer_id`: the Ridwell ID for this particular offer - `priority`: the
+pickup priority - `product_id`: the Ridwell ID for this particular product -
+`quantity`: the amount of the product being picked up ### Opting Into or Out Of
+a Pickup Event ```python import asyncio from aioridwell import async_get_client
+async def main() -> None: client = await async_get_client("", "") accounts =
+await client.async_get_accounts() for account in accounts.values(): events =
+await account.async_get_pickup_events() # >>> [RidwellPickupEvent(...), ...]
+await events[0].async_opt_in() await events[0].async_opt_out() asyncio.run(main
+()) ``` ### Calculating a Pickup Event's Estimated Cost ```python import
+asyncio from aioridwell import async_get_client async def main() -> None:
+client = await async_get_client("", "") accounts = await
+client.async_get_accounts() for account in accounts.values(): events = await
+account.async_get_pickup_events() # >>> [RidwellPickupEvent(...), ...]
+event_1_cost = await events[0].async_get_estimated_cost() # >>> 22.00
+asyncio.run(main()) ``` # Contributing Thanks to all of [our contributors]
+[contributors] so far! 1. [Check for open features/bugs][issues] or [initiate a
+discussion on one][new-issue]. 2. [Fork the repository][fork]. 3. (_optional,
+but highly recommended_) Create a virtual environment: `python3 -m venv .venv`
+4. (_optional, but highly recommended_) Enter the virtual environment: `source
+./.venv/bin/activate` 5. Install the dev environment: `script/setup` 6. Code
+your new feature or bug fix on a new branch. 7. Write tests that cover your new
+functionality. 8. Run tests and ensure 100% code coverage: `poetry run pytest -
+-cov aioridwell tests` 9. Update `README.md` with any new documentation. 10.
+Submit a pull request! [aiohttp]: https://github.com/aio-libs/aiohttp [ci-
+badge]: https://github.com/bachya/aioridwell/workflows/CI/badge.svg [ci]:
+https://github.com/bachya/aioridwell/actions [codecov-badge]: https://
+codecov.io/gh/bachya/aioridwell/branch/dev/graph/badge.svg [codecov]: https://
+codecov.io/gh/bachya/aioridwell [contributors]: https://github.com/bachya/
+aioridwell/graphs/contributors [fork]: https://github.com/bachya/aioridwell/
+fork [issues]: https://github.com/bachya/aioridwell/issues [license-badge]:
+https://img.shields.io/pypi/l/aioridwell.svg [license]: https://github.com/
+bachya/aioridwell/blob/main/LICENSE [maintainability-badge]: https://
+api.codeclimate.com/v1/badges/9c1dcc1c991cecb06eda/maintainability
 [maintainability]: https://codeclimate.com/github/bachya/aioridwell/
-maintainability\n[new-issue]: https://github.com/bachya/aioridwell/issues/new\n
-[new-issue]: https://github.com/bachya/aioridwell/issues/new\n[pypi-badge]:
-https://img.shields.io/pypi/v/aioridwell.svg\n[pypi]: https://pypi.python.org/
-pypi/aioridwell\n[ridwell]: https://ridwell.com\n[version-badge]: https://
-img.shields.io/pypi/pyversions/aioridwell.svg\n[version]: https://
-pypi.python.org/pypi/aioridwell\n', 'author': 'Aaron Bach', 'author_email':
-'bachya1208@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/bachya/aioridwell', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9.0,<4.0.0', } setup(**setup_kwargs)
+maintainability [new-issue]: https://github.com/bachya/aioridwell/issues/new
+[new-issue]: https://github.com/bachya/aioridwell/issues/new [pypi-badge]:
+https://img.shields.io/pypi/v/aioridwell.svg [pypi]: https://pypi.python.org/
+pypi/aioridwell [ridwell]: https://ridwell.com [version-badge]: https://
+img.shields.io/pypi/pyversions/aioridwell.svg [version]: https://
+pypi.python.org/pypi/aioridwell
```

