# Comparing `tmp/ScriptCollection-3.4.2-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 62325 bytes, number of entries: 14
+Zip file size: 62381 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    19068 b- defN 23-Jul-09 10:07 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    96083 b- defN 23-Jul-09 20:14 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   144098 b- defN 23-Jul-09 20:14 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    96083 b- defN 23-Jul-11 10:23 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   144215 b- defN 23-Jul-11 10:23 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7649 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/RECORD
-14 files, 323916 bytes uncompressed, 60143 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-11 10:23 ScriptCollection-3.4.3.dist-info/RECORD
+14 files, 324034 bytes uncompressed, 60199 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.2.dist-info/METADATA
+Filename: ScriptCollection-3.4.3.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.2.dist-info/WHEEL
+Filename: ScriptCollection-3.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.2.dist-info/entry_points.txt
+Filename: ScriptCollection-3.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.2.dist-info/top_level.txt
+Filename: ScriptCollection-3.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.2.dist-info/RECORD
+Filename: ScriptCollection-3.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -25,15 +25,15 @@
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.2"
+version = "3.4.3"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -268,15 +268,16 @@
         # gpg_identity-value when wheel-file should not be signed: None
         folder = os.path.dirname(wheel_file)
         filename = os.path.basename(wheel_file)
 
         if gpg_identity is None:
             gpg_identity_argument = ""
         else:
-            gpg_identity_argument = f" --sign --identity {gpg_identity}"
+            pass  # gpg_identity_argument = f" --sign --identity {gpg_identity}"
+            # disabled due to https://blog.pypi.org/posts/2023-05-23-removing-pgp/
 
         if verbosity > 2:
             verbose_argument = " --verbose"
         else:
             verbose_argument = ""
 
         twine_argument = f"upload{gpg_identity_argument} --repository {repository} --non-interactive {filename} --disable-progress-bar"
@@ -1104,15 +1105,15 @@
 
         self.__sc.git_commit(createReleaseInformation.reference_repository, f"Added reference of {createRelease_configuration.projectname} v{new_project_version}")
         if createRelease_configuration.reference_repository_remote_name is not None:
             self.__sc.git_push(createReleaseInformation.reference_repository, createRelease_configuration.reference_repository_remote_name,
                                createRelease_configuration.reference_repository_branch_name, createRelease_configuration.reference_repository_branch_name,
                                verbosity=createRelease_configuration.verbosity)
         self.__sc.git_commit(build_repository_folder, f"Added {createRelease_configuration.projectname} release v{new_project_version}")
-        GeneralUtilities.write_message_to_stdout(f"Finished release for project {createRelease_configuration.projectname} successfully.")
+        GeneralUtilities.write_message_to_stdout(f"Finished release for project {createRelease_configuration.projectname} v{new_project_version} successfully.")
         return new_project_version
 
     @GeneralUtilities.check_arguments
     def create_release_starter_for_repository_in_standardized_format(self, create_release_file: str, logfile: str, verbosity: int, addLogOverhead: bool,
                                                                      commandline_arguments: list[str]):
         # hint: arguments can be overwritten by commandline_arguments
         folder_of_this_file = os.path.dirname(create_release_file)
@@ -1530,15 +1531,15 @@
         self.set_constant(codeunit_folder, source_constant_name+"PublicKey", certificate_publickey)
 
     @GeneralUtilities.check_arguments
     def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "DevelopmentCertificate", domain: str = None):
         """Expects a certificate-resource and generates a constant for its sensitive information in hex-format"""
         if domain is None:
             codeunit_name = os.path.basename(codeunit_folder)
-            domain=codeunit_name
+            domain = codeunit_name
         self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.pfx", "PFX")
         self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.password", "Password")
 
     @GeneralUtilities.check_arguments
     def generate_constant_from_resource_by_filename(self, codeunit_folder: str, resource_name: str, filename: str, constant_name: str):
         certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         resource_file = os.path.join(certificate_resource_folder, filename)
```

## Comparing `ScriptCollection-3.4.2.dist-info/METADATA` & `ScriptCollection-3.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.2
+Version: 3.4.3
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
@@ -18,32 +18,32 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: coverage (>=7.2.5)
+Requires-Dist: coverage (>=7.2.7)
 Requires-Dist: cyclonedx-bom (>=3.11.0)
 Requires-Dist: defusedxml (>=0.7.1)
 Requires-Dist: keyboard (>=0.13.5)
-Requires-Dist: lxml (>=4.9.2)
+Requires-Dist: lxml (>=4.9.3)
 Requires-Dist: ntplib (>=0.4.0)
-Requires-Dist: Pillow (>=9.5.0)
+Requires-Dist: Pillow (>=10.0.0)
 Requires-Dist: pycdlib (>=1.14.0)
 Requires-Dist: Pygments (>=2.15.1)
 Requires-Dist: pylint (>=2.17.4)
-Requires-Dist: pyOpenSSL (>=23.1.1)
-Requires-Dist: PyMuPDF (>=1.22.3)
+Requires-Dist: pyOpenSSL (>=23.2.0)
+Requires-Dist: PyMuPDF (>=1.22.5)
 Requires-Dist: PyPDF2 (>=3.0.1)
-Requires-Dist: pytest (>=7.3.1)
+Requires-Dist: pytest (>=7.4.0)
 Requires-Dist: qrcode (>=7.4.2)
 Requires-Dist: send2trash (>=1.8.2)
 Requires-Dist: twine (>=4.0.2)
-Requires-Dist: xmlschema (>=2.3.0)
+Requires-Dist: xmlschema (>=2.3.1)
 
 # ScriptCollection
 
 ## General
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/ScriptCollection.svg)](https://pypi.org/project/ScriptCollection/)
 ![PyPI](https://img.shields.io/pypi/v/ScriptCollection)
```

## Comparing `ScriptCollection-3.4.2.dist-info/entry_points.txt` & `ScriptCollection-3.4.3.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.4.2.dist-info/RECORD` & `ScriptCollection-3.4.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=BanfD3ls0ov3ECnsbuyzNstdYjqz_HplreQYJxrB8Ag,19068
 ScriptCollection/GeneralUtilities.py,sha256=vZDiW5lWJRCrIZVs1bTCZ-O5slQnM5dv4GcJ-RTMowY,34378
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=6qa2zBQSbxkIBwMZ4heulf6dDhtrMN7gkanutNxeHhk,96083
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=aDhyppnfEgaiLxo4H04fZVJfAjsGisUeexCkq6LyEHo,144098
+ScriptCollection/ScriptCollectionCore.py,sha256=f-nUf0mVi4GfCOS83VWqLvRqfbCZXEODacBxeacD4pw,96083
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=R2a1LKlWrdp5TMjQSvdTsGv-F_3v7EpKidYZflxHJv4,144215
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.4.2.dist-info/METADATA,sha256=evfc3SpJ8Vv-CaWAdN61NruiT4me5XscExweMZkxWUw,7649
-ScriptCollection-3.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.4.2.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
-ScriptCollection-3.4.2.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.4.2.dist-info/RECORD,,
+ScriptCollection-3.4.3.dist-info/METADATA,sha256=lGelemdj5ymuM5sEHWH_aBfjGDWenkohDcNovW9FCZU,7650
+ScriptCollection-3.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.4.3.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
+ScriptCollection-3.4.3.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.4.3.dist-info/RECORD,,
```

