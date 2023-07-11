# Comparing `tmp/scw_gateway-0.4.0.tar.gz` & `tmp/scw_gateway-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.4.0.tar", max compression
+gzip compressed data, was "scw_gateway-0.5.0.tar", max compression
```

## Comparing `scw_gateway-0.4.0.tar` & `scw_gateway-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0     2979 2023-07-03 14:54:01.781895 scw_gateway-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/__init__.py
--rw-r--r--   0        0        0      825 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/cli.py
--rw-r--r--   0        0        0      352 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/client.py
--rw-r--r--   0        0        0      616 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/consumer.py
--rw-r--r--   0        0        0      758 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/dev.py
--rw-r--r--   0        0        0     2958 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/infra.py
--rw-r--r--   0        0        0      538 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/jwt.py
--rw-r--r--   0        0        0     1575 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/route.py
--rw-r--r--   0        0        0     2465 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/conf.py
--rw-r--r--   0        0        0     8041 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/gateway.py
--rw-r--r--   0        0        0      281 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/__init__.py
--rw-r--r--   0        0        0     1978 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/cockpit.py
--rw-r--r--   0        0        0     6009 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/container.py
--rw-r--r--   0        0        0      519 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/function.py
--rw-r--r--   0        0        0      317 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/image.py
--rw-r--r--   0        0        0    15463 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/manager.py
--rw-r--r--   0        0        0      999 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/rdb.py
--rw-r--r--   0        0        0     2515 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/secrets.py
--rw-r--r--   0        0        0     1901 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/model.py
--rw-r--r--   0        0        0      940 2023-07-03 14:53:22.505477 scw_gateway-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 scw_gateway-0.4.0/setup.py
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 scw_gateway-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3221 2023-07-11 09:51:56.814417 scw_gateway-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/cli.py
+-rw-r--r--   0        0        0      352 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/client.py
+-rw-r--r--   0        0        0      616 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/consumer.py
+-rw-r--r--   0        0        0      758 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/dev.py
+-rw-r--r--   0        0        0      815 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/domain.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/human/__init__.py
+-rw-r--r--   0        0        0     2618 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/human/progress.py
+-rw-r--r--   0        0        0     4101 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/infra.py
+-rw-r--r--   0        0        0      538 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/jwt.py
+-rw-r--r--   0        0        0     1312 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/route.py
+-rw-r--r--   0        0        0     2465 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/conf.py
+-rw-r--r--   0        0        0       54 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/console.py
+-rw-r--r--   0        0        0     8157 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/__init__.py
+-rw-r--r--   0        0        0     4968 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6009 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/function.py
+-rw-r--r--   0        0        0      317 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/image.py
+-rw-r--r--   0        0        0    19375 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2515 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1901 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/model.py
+-rw-r--r--   0        0        0     1185 2023-07-11 09:51:20.466042 scw_gateway-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 scw_gateway-0.5.0/setup.py
+-rw-r--r--   0        0        0     3882 1970-01-01 00:00:00.000000 scw_gateway-0.5.0/PKG-INFO
```

### Comparing `scw_gateway-0.4.0/README.md` & `scw_gateway-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-# Scaleway Serverless Gateway :door:
+# Scaleway Serverless Gateway :spider_web:
+
+[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)
+[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)
+[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)
 
 The Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).
 
 It lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.
 
 It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.
 
 ## :page_with_curl: Contents
 
 - [:rocket: Features](#rocket-features)
 - [:computer: Quick-start](#computer-quick-start)
-- [Observability](docs/observability.md)
-- [Custom domains](docs/domains.md)
-- [Adding authnetication](docs/auth.md)
-- [Adding CORS](docs/cors.md)
-- [Accessing Kong directly](docs/kong.md)
-- [Serverless functions](docs/serverless.md)
-- [Modifying the gateway](docs/custom.md)
-- [:hammer: Architecture](docs/architecture.md)
 - [:mortar\_board: Contributing](#mortar_board-contributing)
 - [:mailbox: Reach Us](#mailbox-reach-us)
 
+Please see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.
+
 ## :computer: Quick-start
 
 To deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):
 
 ```console
 pip install scw-gateway
 ```
```

### Comparing `scw_gateway-0.4.0/cli/cli.py` & `scw_gateway-0.5.0/cli/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 
 import click
 from loguru import logger
 
 from cli.commands.consumer import consumer as consumer_commands
 from cli.commands.dev import dev as dev_commands
+from cli.commands.domain import domain as domain_commands
 from cli.commands.infra import infra as infra_commands
 from cli.commands.jwt import jwt as jwt_commands
 from cli.commands.route import route as route_commands
 
 
 @click.group()
 def cli():
@@ -27,10 +28,11 @@
     # Set log level
     logger.remove()
     logger.add(sys.stderr, level="INFO")
 
 
 cli.add_command(consumer_commands)
 cli.add_command(dev_commands)
+cli.add_command(domain_commands)
 cli.add_command(infra_commands)
 cli.add_command(jwt_commands)
 cli.add_command(route_commands)
```

### Comparing `scw_gateway-0.4.0/cli/commands/consumer.py` & `scw_gateway-0.5.0/cli/commands/consumer.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/commands/dev.py` & `scw_gateway-0.5.0/cli/commands/dev.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/commands/jwt.py` & `scw_gateway-0.5.0/cli/commands/jwt.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/commands/route.py` & `scw_gateway-0.5.0/cli/commands/route.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import click
 
-from cli import client
 from cli.gateway import GatewayManager
-from cli.infra import InfraManager
 from cli.model import Route
 
 
 @click.group()
 def route():
     """Manage gateway routes"""
     pass
@@ -51,15 +49,7 @@
 @click.argument("target")
 def delete(relative_url, target):
     """Delete a route from the gateway"""
     manager = GatewayManager()
 
     route = Route(relative_url, target)
     manager.delete_route(route)
-
-
-@route.command()
-def custom_domain():
-    """Set the custom domain for the gateway"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.set_custom_domain()
```

### Comparing `scw_gateway-0.4.0/cli/conf.py` & `scw_gateway-0.5.0/cli/conf.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/gateway.py` & `scw_gateway-0.5.0/cli/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 
-import click
 import requests
 from loguru import logger
 from requests.adapters import HTTPAdapter
+from rich.table import Table
 from urllib3 import Retry
 
 from cli import conf
+from cli.console import console
 from cli.model import Consumer, JwtCredential, Route
 
 MAX_RETRIES = 5
 
 
 def response_hook(response: requests.Response, *_args, **_kwargs):
     """Response hook to log request and call raise_for_status."""
@@ -115,20 +116,19 @@
         resp = self.session.delete(url=f"{self.services_url}/{route.name}")
         return resp
 
     def print_routes(self) -> None:
         routes: list[Route] = self.get_routes()
         routes.sort(key=lambda r: r.relative_url)
 
-        click.secho(
-            f"{'RELATIVE URL':<25} {'TARGET':<40} {'HTTP_METHODS':<10}", bold=True
-        )
+        table = Table("RELATIVE URL", "TARGET", "HTTP METHODS", title="Gateway Routes")
         for r in routes:
-            http_methods = r.http_methods if r.http_methods else "All"
-            click.secho(f"{r.relative_url:<25} {r.target:<40} {http_methods:<10}")
+            http_methods = " ".join(r.http_methods) if r.http_methods else "All"
+            table.add_row(r.relative_url, r.target, http_methods)
+        console.print(table)
 
     def get_routes(self) -> list[Route]:
         resp = self.session.get(url=self.routes_url)
         route_data = {r.get("name"): r for r in resp.json().get("data")}
 
         resp = self.session.get(url=self.services_url)
         service_data = {s.get("name"): s for s in resp.json().get("data")}
@@ -164,17 +164,18 @@
         consumer_data.sort(key=lambda x: x["username"])
 
         return [Consumer.from_json(c) for c in consumer_data]
 
     def print_consumers(self) -> None:
         consumers: list[Consumer] = self.get_consumers()
 
-        click.secho(f"{'USERNAME':<20}", bold=True)
+        table = Table("CONSUMER", title="Consumers")
         for c in consumers:
-            click.secho(f"{c.username:<20}")
+            table.add_row(c.username)
+        console.print(table)
 
     def delete_consumer(self, consumer_name: str):
         consumer_url = f"{self.consumers_url}/{consumer_name}"
         resp = self.session.delete(url=consumer_url)
         resp.raise_for_status()
 
     def add_consumer(self, consumer_name):
@@ -198,18 +199,21 @@
 
         resp = self.session.get(url=jwt_url)
         resp.raise_for_status()
 
         creds_data = resp.json()["data"]
         return [JwtCredential.from_json(d) for d in creds_data]
 
-    def print_jwt_creds(self, creds: list[JwtCredential], header=True):
-        click.secho(f"{'ALGORITHM':<15} {'SECRET':<40} {'ISS':<40}", bold=True)
+    def print_jwt_creds(self, creds: list[JwtCredential]):
+        """Print JWT credentials for a consumer."""
+
+        table = Table("ALGORITHM", "SECRET", "ISS", title="JWT Credentials")
         for c in creds:
-            click.secho(f"{c.algorithm:<15} {c.secret:<40} {c.iss:<40}")
+            table.add_row(c.algorithm, c.secret, c.iss)
+        console.print(table)
 
     def print_jwt_creds_for_consumer(self, consumer_name):
         creds = self.get_jwt_creds(consumer_name)
         self.print_jwt_creds(creds)
 
     def setup_global_kong_statsd_plugin(self) -> str:
         """Install the kong statsd plugin on the kong admin API.
```

### Comparing `scw_gateway-0.4.0/cli/infra/container.py` & `scw_gateway-0.5.0/cli/infra/container.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/infra/function.py` & `scw_gateway-0.5.0/cli/infra/function.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/infra/rdb.py` & `scw_gateway-0.5.0/cli/infra/rdb.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/infra/secrets.py` & `scw_gateway-0.5.0/cli/infra/secrets.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/cli/model.py` & `scw_gateway-0.5.0/cli/model.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.4.0/pyproject.toml` & `scw_gateway-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.4.0"
+version = "0.5.0"
 description = "CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem"
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
 packages = [{ include = "cli" }]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
 python = "^3.10"
 requests = "^2.28.2"
 click = "^8.1.3"
 pyyaml = "^6.0"
 scaleway = "^0.12.0"
+rich = "^13.4.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pyjwt = "^2.7.0"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 responses = "^0.23.1"
 types-pyyaml = "^6.0.12.9"
 types-requests = "^2.29.0.0"
 
+[tool.poetry.group.doc]
+optional = true
+
+[tool.poetry.group.doc.dependencies]
+myst-parser = "^2.0.0"
+sphinx = "^6.1.0"
+sphinx_rtd_theme = "^1.2.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 scwgw = "cli.cli:cli"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 testpaths = ["tests"]
+markers = [
+  "deployed: Integration tests for a fully deployed environment",
+]
 
 [tool.mypy]
 exclude = ["venv", "endpoints"]
```

### Comparing `scw_gateway-0.4.0/setup.py` & `scw_gateway-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['cli', 'cli.commands', 'cli.infra']
+['cli', 'cli.commands', 'cli.commands.human', 'cli.infra']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'loguru==0.6.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
+ 'rich>=13.4.2,<14.0.0',
  'scaleway>=0.12.0,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['scwgw = cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'scw-gateway',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem',
-    'long_description': "# Scaleway Serverless Gateway :door:\n\nThe Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).\n\nIt lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.\n\nIt is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.\n\n## :page_with_curl: Contents\n\n- [:rocket: Features](#rocket-features)\n- [:computer: Quick-start](#computer-quick-start)\n- [Observability](docs/observability.md)\n- [Custom domains](docs/domains.md)\n- [Adding authnetication](docs/auth.md)\n- [Adding CORS](docs/cors.md)\n- [Accessing Kong directly](docs/kong.md)\n- [Serverless functions](docs/serverless.md)\n- [Modifying the gateway](docs/custom.md)\n- [:hammer: Architecture](docs/architecture.md)\n- [:mortar\\_board: Contributing](#mortar_board-contributing)\n- [:mailbox: Reach Us](#mailbox-reach-us)\n\n## :computer: Quick-start\n\nTo deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):\n\n```console\npip install scw-gateway\n```\n\nOnce done, the following steps can be run from the root of the project, and will deploy the gateway as a Serverless Container in your Scaleway account.\n\nThe gateway image itself is packaged via our public [Serverless Gateway Docker image](https://hub.docker.com/r/scaleway/serverless-gateway).\n\n### Deploy your gateway\n\nTo deploy your gateway, you can run:\n\n```console\nscwgw infra deploy\n```\n\n### Add a route\n\nTo check your gateway is working, you can add and remove a route:\n\n```console\n# Check no routes are configured initially\nscwgw route ls\n\n# Check the response directly from a given URL\nTARGET_URL=http://worldtimeapi.org/api/timezone/Europe/Paris\ncurl $TARGET_URL\n\n# Add a route to this URL in your gateway\nscwgw route add /time $TARGET_URL\n\n# List routes to see that it's been configured\nscwgw route ls\n\n# Curl the URL via the gateway\nGATEWAY_ENDPOINT=$(scwgw infra endpoint)\ncurl https://${GATEWAY_ENDPOINT}/time\n```\n\n### Delete your gateway\n\nTo delete your gateway, you can run:\n\n```console\nscwgw infra delete\n```\n\n## :mortar_board: Contributing\n\nWe welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).\n\nDo not hesitate to raise issues and pull requests we will have a look at them.\n\n## :mailbox: Reach us\n\nWe love feedback. Feel free to:\n\n- Open a [Github issue](https://github.com/scaleway/serverless-functions-python/issues/new)\n- Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.\n",
+    'long_description': "# Scaleway Serverless Gateway :spider_web:\n\n[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)\n[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)\n[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)\n\nThe Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).\n\nIt lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.\n\nIt is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.\n\n## :page_with_curl: Contents\n\n- [:rocket: Features](#rocket-features)\n- [:computer: Quick-start](#computer-quick-start)\n- [:mortar\\_board: Contributing](#mortar_board-contributing)\n- [:mailbox: Reach Us](#mailbox-reach-us)\n\nPlease see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.\n\n## :computer: Quick-start\n\nTo deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):\n\n```console\npip install scw-gateway\n```\n\nOnce done, the following steps can be run from the root of the project, and will deploy the gateway as a Serverless Container in your Scaleway account.\n\nThe gateway image itself is packaged via our public [Serverless Gateway Docker image](https://hub.docker.com/r/scaleway/serverless-gateway).\n\n### Deploy your gateway\n\nTo deploy your gateway, you can run:\n\n```console\nscwgw infra deploy\n```\n\n### Add a route\n\nTo check your gateway is working, you can add and remove a route:\n\n```console\n# Check no routes are configured initially\nscwgw route ls\n\n# Check the response directly from a given URL\nTARGET_URL=http://worldtimeapi.org/api/timezone/Europe/Paris\ncurl $TARGET_URL\n\n# Add a route to this URL in your gateway\nscwgw route add /time $TARGET_URL\n\n# List routes to see that it's been configured\nscwgw route ls\n\n# Curl the URL via the gateway\nGATEWAY_ENDPOINT=$(scwgw infra endpoint)\ncurl https://${GATEWAY_ENDPOINT}/time\n```\n\n### Delete your gateway\n\nTo delete your gateway, you can run:\n\n```console\nscwgw infra delete\n```\n\n## :mortar_board: Contributing\n\nWe welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).\n\nDo not hesitate to raise issues and pull requests we will have a look at them.\n\n## :mailbox: Reach us\n\nWe love feedback. Feel free to:\n\n- Open a [Github issue](https://github.com/scaleway/serverless-functions-python/issues/new)\n- Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.\n",
     'author': 'Simon Shillaker',
     'author_email': 'sshillaker@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `scw_gateway-0.4.0/PKG-INFO` & `scw_gateway-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.4.0
+Version: 0.5.0
 Summary: CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scaleway (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
 
-# Scaleway Serverless Gateway :door:
+# Scaleway Serverless Gateway :spider_web:
+
+[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)
+[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)
+[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)
 
 The Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).
 
 It lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.
 
 It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.
 
 ## :page_with_curl: Contents
 
 - [:rocket: Features](#rocket-features)
 - [:computer: Quick-start](#computer-quick-start)
-- [Observability](docs/observability.md)
-- [Custom domains](docs/domains.md)
-- [Adding authnetication](docs/auth.md)
-- [Adding CORS](docs/cors.md)
-- [Accessing Kong directly](docs/kong.md)
-- [Serverless functions](docs/serverless.md)
-- [Modifying the gateway](docs/custom.md)
-- [:hammer: Architecture](docs/architecture.md)
 - [:mortar\_board: Contributing](#mortar_board-contributing)
 - [:mailbox: Reach Us](#mailbox-reach-us)
 
+Please see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.
+
 ## :computer: Quick-start
 
 To deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):
 
 ```console
 pip install scw-gateway
 ```
```

