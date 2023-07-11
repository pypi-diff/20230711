# Comparing `tmp/buildingsync-asset-extractor-0.1.8.tar.gz` & `tmp/buildingsync-asset-extractor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildingsync-asset-extractor-0.1.8.tar", max compression
+gzip compressed data, was "buildingsync-asset-extractor-0.1.9.tar", max compression
```

## Comparing `buildingsync-asset-extractor-0.1.8.tar` & `buildingsync-asset-extractor-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1988 2022-06-16 03:58:51.507111 buildingsync-asset-extractor-0.1.8/LICENSE
--rw-r--r--   0        0        0     4736 2022-06-16 03:58:51.507268 buildingsync-asset-extractor-0.1.8/README.md
--rw-r--r--   0        0        0        0 2022-06-16 03:58:51.507417 buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/__init__.py
--rw-r--r--   0        0        0     1664 2022-06-16 03:58:51.507635 buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/config/asset_definitions.json
--rw-r--r--   0        0        0     2870 2022-06-16 03:58:51.507805 buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/main.py
--rw-r--r--   0        0        0    17419 2022-06-16 04:17:22.270284 buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/processor.py
--rw-r--r--   0        0        0     2191 2022-06-16 03:58:51.508302 buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/schemas/asset_definitions_schema.json
--rw-r--r--   0        0        0      998 2022-06-16 03:58:51.508438 buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/schemas/extracted_assets_schema.json
--rw-r--r--   0        0        0      722 2022-06-16 04:17:22.271525 buildingsync-asset-extractor-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5663 2022-06-16 04:18:56.792071 buildingsync-asset-extractor-0.1.8/setup.py
--rw-r--r--   0        0        0     5540 2022-06-16 04:18:56.792580 buildingsync-asset-extractor-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1988 2022-06-29 19:51:14.019804 buildingsync-asset-extractor-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5459 2022-06-29 19:51:14.020271 buildingsync-asset-extractor-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2022-06-29 19:51:14.020397 buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/__init__.py
+-rw-r--r--   0        0        0     3848 2022-06-29 19:51:14.021179 buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/config/asset_definitions.json
+-rw-r--r--   0        0        0     3930 2022-06-29 19:51:14.021532 buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/main.py
+-rw-r--r--   0        0        0    40903 2022-06-29 19:51:14.022065 buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/processor.py
+-rw-r--r--   0        0        0     2191 2022-06-29 19:51:14.022866 buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/schemas/asset_definitions_schema.json
+-rw-r--r--   0        0        0      998 2022-06-29 19:51:14.023443 buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/schemas/extracted_assets_schema.json
+-rw-r--r--   0        0        0      722 2022-06-29 19:56:34.531845 buildingsync-asset-extractor-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6402 2022-06-29 19:57:41.715005 buildingsync-asset-extractor-0.1.9/setup.py
+-rw-r--r--   0        0        0     6263 2022-06-29 19:57:41.715406 buildingsync-asset-extractor-0.1.9/PKG-INFO
```

### Comparing `buildingsync-asset-extractor-0.1.8/LICENSE` & `buildingsync-asset-extractor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `buildingsync-asset-extractor-0.1.8/README.md` & `buildingsync-asset-extractor-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,29 +33,32 @@
 
 1. `num`. The num method will sum up all assets of the specified type and return a single overall number.
 
 1. `avg`. The avg method will return an average value for all assets of the specified type found.
 
 1. `avg_sqft`. The avg_sqft method will return a weighted average value for all assets of the specified type found based on the area they serve.
 
-1. `age_oldest` and `age_newest`. The age method will retrieve the 'YearInstalled' element of a specified equipment type and return either the oldest or newest, as specified.
+1. `age_oldest`, `age_newest`, `age_average`. The age method will retrieve the 'YearOfManufacture' (or 'YearInstalled' if not present) element of a specified equipment type and return either the oldest or newest, or average age (year) as specified. Average age is calculated by a weighted average using the following (in order): capacity, served space area, regular average.
+
+1. `custom`. Use this method for particular asset that do not fit in the other categories; i.e. Heating Efficiency. Note that a dedicated method may need to be written to support this type of asset.
 
 To test usage:
 
 ```bash
 	python buildingsync_asset_extractor/main.py
 ```
 
 This will extract assets from `tests/files/testfile.xml` and save the results to `assets_output.json`
 
 There are 2 methods of initializing the Processor: with either a filename or data
 
 ```bash
 bp = BSyncProcessor(filename=filename)
 ```
+or
 
 ```bash
 bp = BSyncProcessor(data=file_data)
 ```
 
 ## Assumptions
 1. Assuming 1 building per file
@@ -72,31 +75,37 @@
 
 1. sqft: Sqft assets take into account the floor area served by a specific asset and returns 'Primary' and 'Secondary' values.  For example: Primary HVAC System and Secondary HVAC System.
 
 1. avg_sqft: Avg_sqft assets compute a weighted average to get the an average asset value.  For example:  Average Heating Setpoint.
 
 1. num: Num assets count the total number of the specified asset found.  For example, Total number of lighting systems.
 
-1. age_oldest and age_newest: These types return the oldest or newest asset of a specific type.  For example: Oldest Boiler.
+1. age_oldest, age_newest, and age_average: These types return the oldest or newest asset, or average age of a specific type.  For example: Oldest Boiler.
+
+1. custom: For asset that need particular handling, such as Heating Efficiency. The current assets that have custom methods are:
+	- Heating System Efficiency
+	- Cooling System Efficiency
+	- Lighting System Efficiency
+	- Water Heater Efficiency
+	- Heating Fuel Type
 
 The schema for the assets definition JSON file is in `schemas/asset_definitions_schema.json`.
 
 ## Extracted Assets File
 
 The schema for the extracted assets JSON file is in `schemas/extracted_assets_schema.json`.
 
 This file lists the extracted assets information in name, value, units triples.  Names will match the `export_name` listed in the asset_definitions JSON file, except for assets of type 'sqft', which will be prepended by 'Primary' and 'Secondary'.
 
 ## Developing
 
 ### Pre-commit
 
 This project uses `pre-commit <https://pre-commit.com/>`_ to ensure code consistency.
-To enable pre-commit on every commit run the following from the command line from within the git checkout of the
-GMT:
+To enable pre-commit on every commit run the following from the command line from within the git checkout of the BuildingSync-asset-extractor
 
 ```bash
   pre-commit install
 ```
 
 To run pre-commit against the files without calling git commit, then run the following. This is useful when cleaning up the repo before committing.
```

### Comparing `buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/main.py` & `buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,24 +33,52 @@
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 *********************************************************************************************************
 """
 import os
 
 from buildingsync_asset_extractor.processor import BSyncProcessor
 
-filename = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'tests/files/testfile.xml')
+# import glob
+# from pathlib import Path
+
+
+# # 1: regular test
+filename = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'tests/files/completetest.xml')
 out_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'assets_output.json')
 out_file2 = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'assets_output2.json')
 
 print("filename: {}".format(filename))
 
+# bp = BSyncProcessor(filename=filename, logger_level='DEBUG')
 bp = BSyncProcessor(filename=filename)
 bp.extract()
 bp.save(out_file)
 
 # does it work when already loaded?
 with open(filename, mode='rb') as file:
     file_data = file.read()
 
 bp = BSyncProcessor(data=file_data)
 bp.extract()
 bp.save(out_file2)
+
+# 2: bigger test
+# bae_tester_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', '..', '..', 'Desktop/BAE-tester/20220519_AT_BSXML')
+# find_path = os.path.join(bae_tester_dir, '*', '*.xml')
+
+# for file in glob.glob(find_path):
+# 	print(file)
+# 	out_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'output', Path(file).stem + '.json')
+# 	bp = BSyncProcessor(filename=file, logger_level='DEBUG')
+# 	bp.extract()
+# 	bp.save(out_file)
+
+# 3: schema examples test
+# bae_tester_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', '..', 'bsync-schema', 'examples')
+# find_path = os.path.join(bae_tester_dir, '*.xml')
+
+# for file in glob.glob(find_path):
+# 	print(file)
+# 	out_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'output', Path(file).stem + '.json')
+# 	bp = BSyncProcessor(filename=file, logger_level='DEBUG')
+# 	bp.extract()
+# 	bp.save(out_file)
```

### Comparing `buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/schemas/asset_definitions_schema.json` & `buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/schemas/asset_definitions_schema.json`

 * *Files identical despite different names*

### Comparing `buildingsync-asset-extractor-0.1.8/buildingsync_asset_extractor/schemas/extracted_assets_schema.json` & `buildingsync-asset-extractor-0.1.9/buildingsync_asset_extractor/schemas/extracted_assets_schema.json`

 * *Files identical despite different names*

### Comparing `buildingsync-asset-extractor-0.1.8/pyproject.toml` & `buildingsync-asset-extractor-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "buildingsync-asset-extractor"
-version = "0.1.8"
+version = "0.1.9"
 description = "BuildingSync Asset Extractor (BAE)"
 authors = ["Katherine Fleming <katherine.fleming@nrel.gov>"]
 license = "BSD4"
 
 readme = "README.md"
 
 homepage = "https://buildingsync.net"
```

### Comparing `buildingsync-asset-extractor-0.1.8/setup.py` & `buildingsync-asset-extractor-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'buildingsync_asset_extractor': ['config/*', 'schemas/*']}
 
 install_requires = \
 ['importlib-resources>=5.7.0,<6.0.0', 'lxml==4.7.1']
 
 setup_kwargs = {
     'name': 'buildingsync-asset-extractor',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'BuildingSync Asset Extractor (BAE)',
-    'long_description': '# BuildingSync Asset Extractor (BAE)\n\nThis package processes a BuildingSync file to extract asset information that can then be imported into SEED\n\n## Installation\n\n### Install from PyPI\n\n```bash\npip install buildingsync-asset-extractor\n```\n### Install from source\n[Poetry](https://python-poetry.org/) is required to install buildingsync-asset-extractor.\n```bash\n# Copy repo\ngit clone https://github.com/BuildingSync/BuildingSync-asset-extractor.git\n\n# install the package\ncd BuildingSync-asset-extractor\npoetry install\n\n# Test that it works, you should see a message describing the usage\npoetry run buildingsync_asset_extractor\n```\n\n## Usage\n\nBuildingSync version 2.4.0.\n\nThe pre-importer will identify assets defined in the `asset_definitions.json` file stored in the `config` directory.  There are various methods of calculating assets:\n\n1. `sqft`.  The sqft method will calculate a \'primary\' and \'secondary\' value for the asset based on the area it serves. This is calculated from the floor areas defined in each `Section` element.  `Conditioned` floor area values will be used if present; `Gross` otherwise.\n\n1. `num`. The num method will sum up all assets of the specified type and return a single overall number.\n\n1. `avg`. The avg method will return an average value for all assets of the specified type found.\n\n1. `avg_sqft`. The avg_sqft method will return a weighted average value for all assets of the specified type found based on the area they serve.\n\n1. `age_oldest` and `age_newest`. The age method will retrieve the \'YearInstalled\' element of a specified equipment type and return either the oldest or newest, as specified.\n\nTo test usage:\n\n```bash\n\tpython buildingsync_asset_extractor/main.py\n```\n\nThis will extract assets from `tests/files/testfile.xml` and save the results to `assets_output.json`\n\nThere are 2 methods of initializing the Processor: with either a filename or data\n\n```bash\nbp = BSyncProcessor(filename=filename)\n```\n\n```bash\nbp = BSyncProcessor(data=file_data)\n```\n\n## Assumptions\n1. Assuming 1 building per file\n1. Assuming sqft method uses "Conditioned" floor area for calculations. If not present, uses "Gross"\n\n## TODO\n1. thermal zones: when spaces are listed within them with spaces (or multiple thermal zones), this would change the average setpoint calculations. Is this an exception or a normal case to handle?\n\n## Assets Definitions File\n\nThis file is used to specify what assets to extract from a BuildingSync XML file. By default, the file found in `config/asset_definitions.json` is used, but a custom file can be specified with the `set_asset_defs_file` method in the `BSyncProcessor` class.\n\nThere are currently 5 types of assets that can be extracted:\n\n1. sqft: Sqft assets take into account the floor area served by a specific asset and returns \'Primary\' and \'Secondary\' values.  For example: Primary HVAC System and Secondary HVAC System.\n\n1. avg_sqft: Avg_sqft assets compute a weighted average to get the an average asset value.  For example:  Average Heating Setpoint.\n\n1. num: Num assets count the total number of the specified asset found.  For example, Total number of lighting systems.\n\n1. age_oldest and age_newest: These types return the oldest or newest asset of a specific type.  For example: Oldest Boiler.\n\nThe schema for the assets definition JSON file is in `schemas/asset_definitions_schema.json`.\n\n## Extracted Assets File\n\nThe schema for the extracted assets JSON file is in `schemas/extracted_assets_schema.json`.\n\nThis file lists the extracted assets information in name, value, units triples.  Names will match the `export_name` listed in the asset_definitions JSON file, except for assets of type \'sqft\', which will be prepended by \'Primary\' and \'Secondary\'.\n\n## Developing\n\n### Pre-commit\n\nThis project uses `pre-commit <https://pre-commit.com/>`_ to ensure code consistency.\nTo enable pre-commit on every commit run the following from the command line from within the git checkout of the\nGMT:\n\n```bash\n  pre-commit install\n```\n\nTo run pre-commit against the files without calling git commit, then run the following. This is useful when cleaning up the repo before committing.\n\n```bash\n  pre-commit run --all-files\n```\n### Testing\n\n\tpoetry run pytest\n\n## Releasing\n\n```bash\npoetry build\n\n# config and push to testpypi\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry publish -r testpypi\n\n# install from testpypi\npip install --index-url https://test.pypi.org/simple/ buildingsync-asset-extractor\n```\nIf everything looks good, publish to pypi:\n```bash\npoetry publish\n```\n\nIf you have environment variables setup for PYPI token username and password:\n\n```bash\npoetry publish --build --username $PYPI_USERNAME --password $PYPI_PASSWORD\n```\n',
+    'long_description': '# BuildingSync Asset Extractor (BAE)\n\nThis package processes a BuildingSync file to extract asset information that can then be imported into SEED\n\n## Installation\n\n### Install from PyPI\n\n```bash\npip install buildingsync-asset-extractor\n```\n### Install from source\n[Poetry](https://python-poetry.org/) is required to install buildingsync-asset-extractor.\n```bash\n# Copy repo\ngit clone https://github.com/BuildingSync/BuildingSync-asset-extractor.git\n\n# install the package\ncd BuildingSync-asset-extractor\npoetry install\n\n# Test that it works, you should see a message describing the usage\npoetry run buildingsync_asset_extractor\n```\n\n## Usage\n\nBuildingSync version 2.4.0.\n\nThe pre-importer will identify assets defined in the `asset_definitions.json` file stored in the `config` directory.  There are various methods of calculating assets:\n\n1. `sqft`.  The sqft method will calculate a \'primary\' and \'secondary\' value for the asset based on the area it serves. This is calculated from the floor areas defined in each `Section` element.  `Conditioned` floor area values will be used if present; `Gross` otherwise.\n\n1. `num`. The num method will sum up all assets of the specified type and return a single overall number.\n\n1. `avg`. The avg method will return an average value for all assets of the specified type found.\n\n1. `avg_sqft`. The avg_sqft method will return a weighted average value for all assets of the specified type found based on the area they serve.\n\n1. `age_oldest`, `age_newest`, `age_average`. The age method will retrieve the \'YearOfManufacture\' (or \'YearInstalled\' if not present) element of a specified equipment type and return either the oldest or newest, or average age (year) as specified. Average age is calculated by a weighted average using the following (in order): capacity, served space area, regular average.\n\n1. `custom`. Use this method for particular asset that do not fit in the other categories; i.e. Heating Efficiency. Note that a dedicated method may need to be written to support this type of asset.\n\nTo test usage:\n\n```bash\n\tpython buildingsync_asset_extractor/main.py\n```\n\nThis will extract assets from `tests/files/testfile.xml` and save the results to `assets_output.json`\n\nThere are 2 methods of initializing the Processor: with either a filename or data\n\n```bash\nbp = BSyncProcessor(filename=filename)\n```\nor\n\n```bash\nbp = BSyncProcessor(data=file_data)\n```\n\n## Assumptions\n1. Assuming 1 building per file\n1. Assuming sqft method uses "Conditioned" floor area for calculations. If not present, uses "Gross"\n\n## TODO\n1. thermal zones: when spaces are listed within them with spaces (or multiple thermal zones), this would change the average setpoint calculations. Is this an exception or a normal case to handle?\n\n## Assets Definitions File\n\nThis file is used to specify what assets to extract from a BuildingSync XML file. By default, the file found in `config/asset_definitions.json` is used, but a custom file can be specified with the `set_asset_defs_file` method in the `BSyncProcessor` class.\n\nThere are currently 5 types of assets that can be extracted:\n\n1. sqft: Sqft assets take into account the floor area served by a specific asset and returns \'Primary\' and \'Secondary\' values.  For example: Primary HVAC System and Secondary HVAC System.\n\n1. avg_sqft: Avg_sqft assets compute a weighted average to get the an average asset value.  For example:  Average Heating Setpoint.\n\n1. num: Num assets count the total number of the specified asset found.  For example, Total number of lighting systems.\n\n1. age_oldest, age_newest, and age_average: These types return the oldest or newest asset, or average age of a specific type.  For example: Oldest Boiler.\n\n1. custom: For asset that need particular handling, such as Heating Efficiency. The current assets that have custom methods are:\n\t- Heating System Efficiency\n\t- Cooling System Efficiency\n\t- Lighting System Efficiency\n\t- Water Heater Efficiency\n\t- Heating Fuel Type\n\nThe schema for the assets definition JSON file is in `schemas/asset_definitions_schema.json`.\n\n## Extracted Assets File\n\nThe schema for the extracted assets JSON file is in `schemas/extracted_assets_schema.json`.\n\nThis file lists the extracted assets information in name, value, units triples.  Names will match the `export_name` listed in the asset_definitions JSON file, except for assets of type \'sqft\', which will be prepended by \'Primary\' and \'Secondary\'.\n\n## Developing\n\n### Pre-commit\n\nThis project uses `pre-commit <https://pre-commit.com/>`_ to ensure code consistency.\nTo enable pre-commit on every commit run the following from the command line from within the git checkout of the BuildingSync-asset-extractor\n\n```bash\n  pre-commit install\n```\n\nTo run pre-commit against the files without calling git commit, then run the following. This is useful when cleaning up the repo before committing.\n\n```bash\n  pre-commit run --all-files\n```\n### Testing\n\n\tpoetry run pytest\n\n## Releasing\n\n```bash\npoetry build\n\n# config and push to testpypi\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry publish -r testpypi\n\n# install from testpypi\npip install --index-url https://test.pypi.org/simple/ buildingsync-asset-extractor\n```\nIf everything looks good, publish to pypi:\n```bash\npoetry publish\n```\n\nIf you have environment variables setup for PYPI token username and password:\n\n```bash\npoetry publish --build --username $PYPI_USERNAME --password $PYPI_PASSWORD\n```\n',
     'author': 'Katherine Fleming',
     'author_email': 'katherine.fleming@nrel.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://buildingsync.net',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `buildingsync-asset-extractor-0.1.8/PKG-INFO` & `buildingsync-asset-extractor-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildingsync-asset-extractor
-Version: 0.1.8
+Version: 0.1.9
 Summary: BuildingSync Asset Extractor (BAE)
 Home-page: https://buildingsync.net
 License: BSD4
 Keywords: BuildingSync,Building Data Exchange
 Author: Katherine Fleming
 Author-email: katherine.fleming@nrel.gov
 Requires-Python: >=3.9,<4.0
@@ -53,29 +53,32 @@
 
 1. `num`. The num method will sum up all assets of the specified type and return a single overall number.
 
 1. `avg`. The avg method will return an average value for all assets of the specified type found.
 
 1. `avg_sqft`. The avg_sqft method will return a weighted average value for all assets of the specified type found based on the area they serve.
 
-1. `age_oldest` and `age_newest`. The age method will retrieve the 'YearInstalled' element of a specified equipment type and return either the oldest or newest, as specified.
+1. `age_oldest`, `age_newest`, `age_average`. The age method will retrieve the 'YearOfManufacture' (or 'YearInstalled' if not present) element of a specified equipment type and return either the oldest or newest, or average age (year) as specified. Average age is calculated by a weighted average using the following (in order): capacity, served space area, regular average.
+
+1. `custom`. Use this method for particular asset that do not fit in the other categories; i.e. Heating Efficiency. Note that a dedicated method may need to be written to support this type of asset.
 
 To test usage:
 
 ```bash
 	python buildingsync_asset_extractor/main.py
 ```
 
 This will extract assets from `tests/files/testfile.xml` and save the results to `assets_output.json`
 
 There are 2 methods of initializing the Processor: with either a filename or data
 
 ```bash
 bp = BSyncProcessor(filename=filename)
 ```
+or
 
 ```bash
 bp = BSyncProcessor(data=file_data)
 ```
 
 ## Assumptions
 1. Assuming 1 building per file
@@ -92,31 +95,37 @@
 
 1. sqft: Sqft assets take into account the floor area served by a specific asset and returns 'Primary' and 'Secondary' values.  For example: Primary HVAC System and Secondary HVAC System.
 
 1. avg_sqft: Avg_sqft assets compute a weighted average to get the an average asset value.  For example:  Average Heating Setpoint.
 
 1. num: Num assets count the total number of the specified asset found.  For example, Total number of lighting systems.
 
-1. age_oldest and age_newest: These types return the oldest or newest asset of a specific type.  For example: Oldest Boiler.
+1. age_oldest, age_newest, and age_average: These types return the oldest or newest asset, or average age of a specific type.  For example: Oldest Boiler.
+
+1. custom: For asset that need particular handling, such as Heating Efficiency. The current assets that have custom methods are:
+	- Heating System Efficiency
+	- Cooling System Efficiency
+	- Lighting System Efficiency
+	- Water Heater Efficiency
+	- Heating Fuel Type
 
 The schema for the assets definition JSON file is in `schemas/asset_definitions_schema.json`.
 
 ## Extracted Assets File
 
 The schema for the extracted assets JSON file is in `schemas/extracted_assets_schema.json`.
 
 This file lists the extracted assets information in name, value, units triples.  Names will match the `export_name` listed in the asset_definitions JSON file, except for assets of type 'sqft', which will be prepended by 'Primary' and 'Secondary'.
 
 ## Developing
 
 ### Pre-commit
 
 This project uses `pre-commit <https://pre-commit.com/>`_ to ensure code consistency.
-To enable pre-commit on every commit run the following from the command line from within the git checkout of the
-GMT:
+To enable pre-commit on every commit run the following from the command line from within the git checkout of the BuildingSync-asset-extractor
 
 ```bash
   pre-commit install
 ```
 
 To run pre-commit against the files without calling git commit, then run the following. This is useful when cleaning up the repo before committing.
```

