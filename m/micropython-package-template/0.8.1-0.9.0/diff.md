# Comparing `tmp/micropython-package-template-0.8.1.tar.gz` & `tmp/micropython-package-template-0.9.0.tar.gz`

## Comparing `micropython-package-template-0.8.1.tar` & `micropython-package-template-0.9.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 19:27:22.000000 micropython-package-template-0.8.1/be_upy_blink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-12 19:27:22.000000 micropython-package-template-0.8.1/be_upy_blink/blink.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 19:27:34.000000 micropython-package-template-0.8.1/be_upy_blink/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-06-12 19:27:35.000000 micropython-package-template-0.8.1/micropython_package_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 21:12:34.000000 micropython-package-template-0.9.0/be_upy_blink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 21:12:34.000000 micropython-package-template-0.9.0/be_upy_blink/blink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 21:12:42.000000 micropython-package-template-0.9.0/be_upy_blink/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-11 21:12:43.000000 micropython-package-template-0.9.0/micropython_package_template.egg-info/PKG-INFO
```

### Comparing `micropython-package-template-0.8.1/be_upy_blink/blink.py` & `micropython-package-template-0.9.0/be_upy_blink/blink.py`

 * *Files identical despite different names*

### Comparing `micropython-package-template-0.8.1/micropython_package_template.egg-info/PKG-INFO` & `micropython-package-template-0.9.0/micropython_package_template.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-package-template
-Version: 0.8.1
+Version: 0.9.0
 Summary: MicroPython PyPi package template project with auto deploy
 Home-page: https://github.com/brainelectronics/micropython-package-template
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-template/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-template
@@ -38,15 +38,15 @@
 [MicroPython Package Template ReadTheDocs][ref-rtd-micropython-package-template] 📚
 
 <!-- MarkdownTOC -->
 
 - [Installation](#installation)
 	- [Install required tools](#install-required-tools)
 - [Setup](#setup)
-	- [Install package with upip](#install-package-with-upip)
+	- [Install package](#install-package)
 		- [General](#general)
 		- [Specific version](#specific-version)
 		- [Test version](#test-version)
 	- [Manually](#manually)
 		- [Upload files to board](#upload-files-to-board)
 - [Usage](#usage)
 - [Create a PyPi \(micropython\) package](#create-a-pypi-micropython-package)
@@ -80,15 +80,15 @@
 source .venv/bin/activate
 
 pip install -r requirements.txt
 ```
 
 ## Setup
 
-### Install package with upip
+### Install package
 
 Connect the MicroPython device to a network (if possible)
 
 ```python
 import network
 station = network.WLAN(network.STA_IF)
 station.active(True)
@@ -245,25 +245,29 @@
 
 ### Unittests
 
 Run the unittests locally with the following command after installing this
 package in a virtual environment
 
 ```bash
+# create a report directory where all generated report files are placed
+python create_report_dirs.py
+```
+
+```bash
 # run all tests
 nose2 --config tests/unittest.cfg
 
 # run only one specific tests
 nose2 tests.test_blink.TestBlink.test_flash_led
 ```
 
 Generate the coverage files with
 
 ```bash
-python create_report_dirs.py
 coverage html
 ```
 
 The coverage report is placed at `reports/coverage/html/index.html`
 
 ## Steps after using this template
 
@@ -273,14 +277,15 @@
 | File | Changes | More details |
 | ---- | ------- | -------------|
 | `.coveragerc` | Path to `version.py` file | Omit version file from coverage |
 | `.coveragerc` | Path to `include` folder | Include the package folder for coverage |
 | `.github/workflows/release.yml` | Path to `version.py` file | Use package version file to set changelog based version |
 | `.github/workflows/test-release.yml` | Path to `version.py` file | Use package version file to set changelog based version |
 | `.github/workflows/test.yml` | Path to `version.py` file | Use package version file to set changelog based version |
+| `.pre-commit-config.yaml` | Path to `version.py` file | Use package version file for validation against latest changelog based version |
 | `README.md` | Links in header section and installation instructions | |
 | `changelog.md` | Cleanup changelog from informations of template | Keep usage of SemVer |
 | `docs/DOCUMENTATION.md` | Kink to ReadTheDocs | |
 | `docs/conf.py` | List to modules to be mocked, package import, path to `version.py` file, update `author`, `project` and `linkcheck_ignore` | |
 | `docs/index.rst` | Header name and included modules | Replace `be_upy_blink` with new `.rst` file of new package |
 | `docs/NEW_MODULE_NAME.rst` | Create a new `.rst` file  named as the package | Use `docs/be_upy_blink.rst` as template |
 | `package.json` | Files and paths to new package and repo | Used by `mip` |
```

