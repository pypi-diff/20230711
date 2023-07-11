# Comparing `tmp/sydeploy-0.3.0-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7490 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 12:33 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-10 12:33 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-10 12:33 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 12:33 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 12:33 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2326 b- defN 23-Jul-10 12:33 sydeploy/commands/authenticate/codeartifact.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 12:33 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-10 12:33 sydeploy/commands/build/python_package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-10 12:33 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-10 12:33 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 12:33 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx      807 b- defN 23-Jul-10 12:33 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-10 12:34 sydeploy-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-10 12:34 sydeploy-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 12:34 sydeploy-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-10 12:34 sydeploy-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-10 12:34 sydeploy-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-10 12:34 sydeploy-0.3.0.dist-info/RECORD
-18 files, 12023 bytes uncompressed, 4968 bytes compressed:  58.7%
+Zip file size: 7541 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-11 12:25 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-11 12:25 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2326 b- defN 23-Jul-11 12:25 sydeploy/commands/authenticate/codeartifact.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     5227 b- defN 23-Jul-11 12:25 sydeploy/commands/build/python_package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-11 12:25 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-11 12:25 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx      807 b- defN 23-Jul-11 12:25 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/RECORD
+18 files, 12328 bytes uncompressed, 5019 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.0.dist-info/LICENSE
+Filename: sydeploy-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.0.dist-info/METADATA
+Filename: sydeploy-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.0.dist-info/WHEEL
+Filename: sydeploy-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.0.dist-info/entry_points.txt
+Filename: sydeploy-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.0.dist-info/top_level.txt
+Filename: sydeploy-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.0.dist-info/RECORD
+Filename: sydeploy-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/build/python_package.py

```diff
@@ -1,12 +1,13 @@
 import sys
 import os
 import shutil
 import importlib
 import json
+import pathlib
 from impose_cli.decorators import impose
 from yaml import safe_load
 from os import listdir
 from pip._internal.req import parse_requirements
 from subprocess import run
 from os.path import join, exists, basename, dirname, abspath, isdir
 from inspect import getfullargspec
@@ -65,31 +66,36 @@
     package_name = basename(package_directory)
     if exists(join(package_directory, "README.rst")):
         long_description = open(join(package_directory, "README.rst"), "r").read()
     else:
         print("No README was found for the package -- the description will be empty.")
         long_description = ""
 
-    setup_file = open(join(dirname(abspath(__file__)), "../templates/setup.py.dist"), "r").read()
+    setup_file = open("{}/{}".format(pathlib.Path(__file__).parent.parent.parent, "templates/setup.py.dist"), "r").read()
     requirements_path = join(package_directory, "requirements.txt")
+
     requirements = [] if not exists(requirements_path) \
         else [str(ir.requirement) for ir in parse_requirements(requirements_path, session='build')]
     requirements = "[{}]".format(', '.join(f'"{s}"' for s in requirements))
 
+    extra_requirements_dict = {}
+    extra_requirements = [basename(file) for file in os.listdir(package_directory) if "requirements" in basename(file) and basename(file).endswith(".txt") and basename(file) != "requirements.txt"]
+    for extra_requirement in extra_requirements:
+        name = extra_requirement.replace("requirements-", "").replace("requirements.", "").replace(".txt", "")
+        extra_requirements_dict[name] = [str(ir.requirement) for ir in parse_requirements(join(package_directory, extra_requirement), session="build")]
+
+
     # Now we look for directories within the package directory and include them in the package data
-    directories = listdir(join(package_directory, package_name))
-    directories = ["{}/*".format(x) for x in directories if x[0] != "." and isdir(join(package_directory, "{}/{}".format(package_name, x)))]
-    package_data = json.dumps({package_name: directories}) if len(directories) > 0 else json.dumps({})
 
     setup_file = setup_file.format(
         name=package_name,
         long_description=long_description,
         version=version,
         requirements=requirements,
-        package_data=package_data
+        extra_requires=json.dumps(extra_requirements_dict),
     )
 
     print("Finished formatting the setup.py file.")
     open(join(package_directory, "setup.py"), "w").write(setup_file)
 
     # Now we build the wheel file
     run(args=f"{python_type} setup.py bdist_wheel", shell=True, cwd=package_directory)
```

## sydeploy/templates/setup.py.dist

```diff
@@ -2,10 +2,10 @@
 
 setuptools.setup(
     name="{name}",
     version="{version}",
     long_description="{long_description}",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    package_data={package_data},
+    extra_requires={extra_requires},
     install_requires={requirements}
 )
```

## Comparing `sydeploy-0.3.0.dist-info/LICENSE` & `sydeploy-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.0.dist-info/RECORD` & `sydeploy-0.3.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/codeartifact.py,sha256=1cILeh4sMS9aeB50Mit2QE5k_6JvVcEOQvuWw0w-sxM,2326
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/build/python_package.py,sha256=7CjSWINfmm8HykBBsgipnQl81cbuabAbiVvkOqYPYL8,4926
+sydeploy/commands/build/python_package.py,sha256=6YnLodZ6NyrszcbBOcmA9MTDF_h_VxmzttW9kJWkOGE,5227
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
-sydeploy/templates/setup.py.dist,sha256=kN0BaVS5hPiiASND6SXelU40c5JdDnJ8z2XXRJDxsE0,287
+sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
-sydeploy-0.3.0.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.0.dist-info/METADATA,sha256=PwYQAMwKQRomPHT3Gf0MBahaASl1qZmq6LIY7Agf1uQ,282
-sydeploy-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.0.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.0.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.0.dist-info/RECORD,,
+sydeploy-0.3.1.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.1.dist-info/METADATA,sha256=nT1gn4PhRztciobbPeaK06BZ6i4A_48RDUYX-xoZYZU,282
+sydeploy-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.1.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.1.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.1.dist-info/RECORD,,
```

