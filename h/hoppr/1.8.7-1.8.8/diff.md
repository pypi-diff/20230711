# Comparing `tmp/hoppr-1.8.7.tar.gz` & `tmp/hoppr-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.7.tar", max compression
+gzip compressed data, was "hoppr-1.8.8.tar", max compression
```

## Comparing `hoppr-1.8.7.tar` & `hoppr-1.8.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-06-21 21:07:06.000000 hoppr-1.8.7/LICENSE
--rw-r--r--   0        0        0     1214 2023-06-21 21:07:06.000000 hoppr-1.8.7/README.md
--rw-r--r--   0        0        0     1035 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11010 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10697 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10932 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     4387 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     4113 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6368 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7961 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4833 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5673 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4606 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/in_toto.py
--rw-r--r--   0        0        0     3357 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17448 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/py.typed
--rw-r--r--   0        0        0     4018 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5023 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    27309 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/result.py
--rw-r--r--   0        0        0     5791 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-06-21 21:07:06.000000 hoppr-1.8.7/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-11 18:05:35.000000 hoppr-1.8.8/LICENSE
+-rw-r--r--   0        0        0     1214 2023-07-11 18:05:35.000000 hoppr-1.8.8/README.md
+-rw-r--r--   0        0        0     1035 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11010 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10697 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10932 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     4305 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     4113 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6368 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7961 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4833 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5673 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4606 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3357 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17448 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/py.typed
+-rw-r--r--   0        0        0     4018 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5023 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    27309 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/result.py
+-rw-r--r--   0        0        0     5791 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-07-11 18:05:35.000000 hoppr-1.8.8/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.8/PKG-INFO
```

### Comparing `hoppr-1.8.7/LICENSE` & `hoppr-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/README.md` & `hoppr-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/__init__.py` & `hoppr-1.8.8/hoppr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.7"
+__version__ = "1.8.8"
```

### Comparing `hoppr-1.8.7/hoppr/base_plugins/collector.py` & `hoppr-1.8.8/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.8/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/cli/hopctl.py` & `hoppr-1.8.8/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/constants.py` & `hoppr-1.8.8/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.8/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,40 +74,39 @@
             image_name = f"{purl.name}@{purl.version}"
         else:
             image_name = f"{purl.name}@sha256:{purl.version}"
             version_path = f"sha256:{purl.version}"
 
         version_path = urllib.parse.quote_plus(re.sub(r'^https?://', '', version_path))
         target_dir = self.directory_for(purl.type, repo_url, subdir=purl.namespace)
-        target_path = target_dir / f"{urllib.parse.unquote(purl.name)}_{purl.version}"
-        destination = f"docker-archive:{target_dir / purl.name}@{version_path}"
+        target_path = target_dir / f"{purl.name}@{version_path}"
 
         source_image = self.get_image(url=repo_url, purl=purl, image_name=image_name)
 
         self.get_logger().info(msg="Copying docker image:", indent_level=2)
         self.get_logger().info(msg=f"source: {source_image}", indent_level=3)
-        self.get_logger().info(msg=f"destination: {destination}", indent_level=3)
+        self.get_logger().info(msg=f"destination: {target_path}", indent_level=3)
 
         command = [self.required_commands[0], "copy"]
 
         password_list = []
 
         if creds is not None:
             password_list = [creds.password.get_secret_value()]
             command.extend(["--src-creds", f"{creds.username}:{creds.password.get_secret_value()}"])
 
         if re.match("^http://", repo_url):
             command = [*command, "--src-tls-verify=false"]
 
-        command = [*command, urllib.parse.unquote(str(source_image)), destination]
+        command = [*command, urllib.parse.unquote(str(source_image)), f"docker-archive:{target_path}"]
 
         proc = self.run_command(command, password_list)
 
         if proc.returncode != 0:
-            msg = f"Skopeo failed to copy docker image to {destination}, " + f"return_code={proc.returncode}"
+            msg = f"Skopeo failed to copy docker image to {target_path}, " + f"return_code={proc.returncode}"
             self.get_logger().debug(msg=msg, indent_level=2)
 
             if target_path.exists():
                 self.get_logger().info(msg="Artifact collection failed, deleting file and retrying", indent_level=2)
                 target_path.unlink()
 
             return Result.retry(message=msg)
```

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.8/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.8/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.8/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.8/hoppr/core_plugins/oras_bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             HopprPluginError: Hoppr plugin error
         """
         total_components = len(components)
         self.get_logger().info(f"Total components: {total_components}")
         self.get_logger().info(f"Total archives: {len(archives)}")
         self.get_logger().flush()
         for component in components:
-            pattern = f"{component.name}[-|_]{component.version}"
+            pattern = f"{component.name}(-|_){component.version}"
             scope = str(component.scope)
             for archive in archives:
                 result = re.match(pattern, archive['path'])
                 if result:
                     if 'excluded' in scope:
                         self.get_logger().info(f"Found scope {component.scope}, removing component from archive.")
                         self.get_logger().flush()
```

### Comparing `hoppr-1.8.7/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.8/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/in_toto.py` & `hoppr-1.8.8/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/main.py` & `hoppr-1.8.8/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/mem_logger.py` & `hoppr-1.8.8/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/__init__.py` & `hoppr-1.8.8/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/__main__.py` & `hoppr-1.8.8/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/base.py` & `hoppr-1.8.8/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/credentials.py` & `hoppr-1.8.8/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/manifest.py` & `hoppr-1.8.8/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/transfer.py` & `hoppr-1.8.8/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/models/types.py` & `hoppr-1.8.8/hoppr/models/types.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/net.py` & `hoppr-1.8.8/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/oci_artifacts.py` & `hoppr-1.8.8/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/plugin_utils.py` & `hoppr-1.8.8/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/processor.py` & `hoppr-1.8.8/hoppr/processor.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.8/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.8/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/result.py` & `hoppr-1.8.8/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/hoppr/utils.py` & `hoppr-1.8.8/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.7/pyproject.toml` & `hoppr-1.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.7"
+version = "1.8.8"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.7/PKG-INFO` & `hoppr-1.8.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.7
+Version: 1.8.8
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

