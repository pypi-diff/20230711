# Comparing `tmp/glint_mask_tools-3.0.3.tar.gz` & `tmp/glint_mask_tools-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glint_mask_tools-3.0.3.tar", max compression
+gzip compressed data, was "glint_mask_tools-3.0.4.tar", max compression
```

## Comparing `glint_mask_tools-3.0.3.tar` & `glint_mask_tools-3.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/LICENSE
--rw-r--r--   0        0        0     7914 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/README.md
--rw-r--r--   0        0        0      369 2023-02-24 14:48:11.069033 glint_mask_tools-3.0.3/glint_mask_generator/__init__.py
--rw-r--r--   0        0        0     5914 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/glint_mask_generator/cli.py
--rw-r--r--   0        0        0     3770 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/glint_mask_generator/glint_algorithms.py
--rw-r--r--   0        0        0     7208 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/glint_mask_generator/image_loaders.py
--rw-r--r--   0        0        0     6647 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/glint_mask_generator/maskers.py
--rw-r--r--   0        0        0     1510 2023-02-24 14:47:14.061154 glint_mask_tools-3.0.3/glint_mask_generator/utils.py
--rw-r--r--   0        0        0      786 2023-02-24 14:48:11.033033 glint_mask_tools-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 glint_mask_tools-3.0.3/setup.py
--rw-r--r--   0        0        0     8809 1970-01-01 00:00:00.000000 glint_mask_tools-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/LICENSE
+-rw-r--r--   0        0        0     7911 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/README.md
+-rw-r--r--   0        0        0      369 2023-07-11 18:05:47.211939 glint_mask_tools-3.0.4/glint_mask_generator/__init__.py
+-rw-r--r--   0        0        0     5914 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/cli.py
+-rw-r--r--   0        0        0     3770 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/glint_algorithms.py
+-rw-r--r--   0        0        0     7208 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/image_loaders.py
+-rw-r--r--   0        0        0     6647 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/maskers.py
+-rw-r--r--   0        0        0     1510 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/utils.py
+-rw-r--r--   0        0        0      794 2023-07-11 18:05:47.171938 glint_mask_tools-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9132 1970-01-01 00:00:00.000000 glint_mask_tools-3.0.4/setup.py
+-rw-r--r--   0        0        0     8806 1970-01-01 00:00:00.000000 glint_mask_tools-3.0.4/PKG-INFO
```

### Comparing `glint_mask_tools-3.0.3/LICENSE` & `glint_mask_tools-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.3/README.md` & `glint_mask_tools-3.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">
 <a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">
     <img alt="Tests" src="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml/badge.svg"/>
 </a>
 
 <a href="https://github.com/HakaiInstitute/GlintMaskGenerator/blob/main/LICENSE.txt">
-    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-darkgray.svg" height="20px" />
+    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-black.svg" height="20px" />
 </a>
 
 <a href="https://badge.fury.io/py/glint-mask-tools">
     <img alt="PyPI version" src="https://badge.fury.io/py/glint-mask-tools.svg" height="20">
 </a>
 
 <a href="https://zenodo.org/badge/latestdoi/266147098">
```

### Comparing `glint_mask_tools-3.0.3/glint_mask_generator/cli.py` & `glint_mask_tools-3.0.4/glint_mask_generator/cli.py`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.3/glint_mask_generator/glint_algorithms.py` & `glint_mask_tools-3.0.4/glint_mask_generator/glint_algorithms.py`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.3/glint_mask_generator/image_loaders.py` & `glint_mask_tools-3.0.4/glint_mask_generator/image_loaders.py`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.3/glint_mask_generator/maskers.py` & `glint_mask_tools-3.0.4/glint_mask_generator/maskers.py`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.3/glint_mask_generator/utils.py` & `glint_mask_tools-3.0.4/glint_mask_generator/utils.py`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.3/pyproject.toml` & `glint_mask_tools-3.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glint-mask-tools"
-version = "3.0.3"
+version = "3.0.4"
 description = "Create masks for specular reflection in UAV and aerial imagery"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/HakaiInstitute/GlintMaskGenerator"
 packages = [
     { include = "glint_mask_generator" }
@@ -14,15 +14,15 @@
 glint-mask = 'glint_mask_generator.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 numpy = "~=1.23.5"
 fire = "~=0.4.0"
 Pillow = "~=9.3.0"
-scipy = "~=1.9.3"
+scipy = ">=1.9.3,<1.11.0"
 tqdm = "~=4.64.1"
 loguru = "~=0.6.0"
 pyqt6 = "^6.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 flake8 = "^6.0.0"
```

### Comparing `glint_mask_tools-3.0.3/setup.py` & `glint_mask_tools-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 install_requires = \
 ['Pillow>=9.3.0,<9.4.0',
  'fire>=0.4.0,<0.5.0',
  'loguru>=0.6.0,<0.7.0',
  'numpy>=1.23.5,<1.24.0',
  'pyqt6>=6.4.0,<7.0.0',
- 'scipy>=1.9.3,<1.10.0',
+ 'scipy>=1.9.3,<1.11.0',
  'tqdm>=4.64.1,<4.65.0']
 
 entry_points = \
 {'console_scripts': ['glint-mask = glint_mask_generator.cli:main']}
 
 setup_kwargs = {
     'name': 'glint-mask-tools',
-    'version': '3.0.3',
+    'version': '3.0.4',
     'description': 'Create masks for specular reflection in UAV and aerial imagery',
-    'long_description': '# Glint Mask Tools\n\n<div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">\n    <img alt="Tests" src="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml/badge.svg"/>\n</a>\n\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/blob/main/LICENSE.txt">\n    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-darkgray.svg" height="20px" />\n</a>\n\n<a href="https://badge.fury.io/py/glint-mask-tools">\n    <img alt="PyPI version" src="https://badge.fury.io/py/glint-mask-tools.svg" height="20">\n</a>\n\n<a href="https://zenodo.org/badge/latestdoi/266147098">\n    <img src="https://zenodo.org/badge/266147098.svg" alt="DOI">\n</a>\n</div>\n\n## Description\n\nGlintMaskGenerator generates image masks for regions in RGB and multispectral image files that have high levels of specular reflection.\n\nThese masks can be used in 3rd party structure-from-motion programs to replace these high glint regions with more useful data from adjacent, overlapping imagery.\n\n## Installation\n\n1. Go to the [releases page](https://github.com/HakaiInstitute/glint-mask-tools/releases)\n2. Download the latest release file for your operating system.\n3. Extract the compressed binary files from the gzipped archive.\n4. This archive contains a file named GlintMaskGenerator-v*.\\*.\\*.exe that provides a GUI interface to the glint mask generation program.\n5. You can copy these files to any location that is convenient for you.\n\n### PyPi package\n\nThere also a python package version of the code available for Python 3.8 and 3.9.\n\n1. `pip install glint-mask-tools` to install the tools.\n2. Then, `import glint_mask_generator` in your Python script.\n3. Installing with pip also installs the CLI tool, detailed below.\n\n## Usage\n\n### GUI\n\nIn Windows, launch the GUI by double clicking the executable file. In Linux, you\'ll have to launch the GUI from the\nterminal, e.g. `./GlintMaskGenerator`.\n\nFor now, generating masks by passing directory paths containing images is the supported workflow. Be sure to change the\nimage type option when processing imagery for cameras other than RGB cameras (e.g. Micasense RedEdge or DJI P4MS cameras). You will be notified of any\nprocessing errors via a pop-up dialog.\n\n### CLI\n\nFor information about the parameters expected by the CLI, run `glint-mask --help` in a bash terminal or command\nline interface. All the functionality of the CLI is documented there.\n\n#### Examples\n\n```bash\nglint-mask-v*.*.* --help\n\n# NAME\n#     glint-mask-v*.*.*\n# \n# SYNOPSIS\n#     glint-mask-v*.*.* - COMMAND | VALUE\n# \n# COMMANDS\n#     COMMAND is one of the following:\n# \n#      cir_threshold\n#        Generate masks for glint regions in 4 Band CIR imagery using Tom Bell\'s binning algorithm.\n# \n#      micasense_threshold\n#        Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell\'s algorithm on the blue image band.\n# \n#      p4ms_threshold\n#        Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell\'s algorithm on the Blue image band.\n# \n#      process\n# \n#      rgb_threshold\n#        Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# VALUES\n#     VALUE is one of the following:\n# \n#      max_workers\n#        The maximum number of threads to use for processing.\n```\n\n```bash\n# Get addition parameters for one of the cameras/methods available\nglint-mask-v*.*.* rgb_threshold --help\n\n# NAME\n#     glint-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# SYNOPSIS\n#     glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR <flags>\n# \n# DESCRIPTION\n#     Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# POSITIONAL ARGUMENTS\n#     IMG_DIR\n#         The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that directory will be # processed.\n#     OUT_DIR\n#         The path to send your out image including the file name and type. e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified as a # # # directory.\n# \n# FLAGS\n#     --thresholds=THRESHOLDS\n#         The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].\n#     --pixel_buffer=PIXEL_BUFFER\n#         The pixel distance to buffer out the mask. Defaults to 0 (off).\n# \n# NOTES\n#     You can also use flags syntax for POSITIONAL ARGUMENTS\n```\n\n```bash\n# Process rgb imagery directory with default parameters\nglint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process PhaseONE camera imagery with image bands split over multiple files\nglint-mask-v*.*.* aco_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process DJI P4MS imagery\nglint-mask-v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process Micasense RedEdge imagery \nglint-mask-v*.*.* micasense_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n```\n\n### Python package\nInstalling the PyPi package allows integrating the mask generation workflow into existing python scripts with ease.\n\n```python\nfrom glint_mask_generator import MicasenseRedEdgeThresholdMasker\n\n# Also available: P4MSThresholdMasker, RGBIntensityRatioMasker, RGBThresholdMasker\n\nmasker = MicasenseRedEdgeThresholdMasker(img_dir="path/to/micasense/images/", mask_dir="path/to/output/dir/",\n                                         thresholds=(0.875, 1, 1, 1, 1), pixel_buffer=5)\nmasker.process(max_workers=5, callback=print, err_callback=print)\n```\n\n## Notes\n\n### Directory of images processing\n\n- All files with "jpg", "jpeg", "tif", "tiff" and "png" extensions will be processed. This can be extended as needed.\n  File extension matching is case-insensitive.\n- Output mask files with be in the specified directory, and have the same name as the input file with "_mask" appended\n  to the end of the file name stem. The file type will match the input type.\n\n### Multi-band image processing\n- For imagery types where each band is spread over multiple files, a mask will be generated for all the sibling band images.\n    - For example, if a mask is generated using a threshold on the blue band image, identical masks are saved for sibling red, green, blue, nir, and red_edge bands as well.\n    - If thresholds are passed for multiple bands, these mask outputs combined with a union operator before being saved for all the sibling bands associated with that capture event.\n\n## Bugs and Feature Requests\n\nThis software is under active development. Bugs and feature requests can be filed using issues page located [here](https://github.com/HakaiInstitute/glint-mask-tools/issues).\n\n## Citation\n\nResearch using these tools or code should cite the following resources\n\n```bibtext\n@article{Cavanaugh2021,\n\ttitle        = {An Automated Method for Mapping Giant Kelp Canopy Dynamics from UAV},\n\tauthor       = {Cavanaugh, K.C. and Cavanaugh, K.C. and Bell, T.W. and Hockridge, E.G.},\n\tyear         = 2021,\n\tjournal      = {Front. Environ. Sci.},\n\tvolume       = {8:587354},\n\tdoi          = {10.3389/fenvs.2020.587354}\n}\n@misc{Denouden2021,\n\ttitle        = {GlintMaskGenerator},\n\tauthor       = {Denouden, T. and Timmer, B. and Reshitnyk, L.},\n\tyear         = 2021,\n\tjournal      = {GitHub repository},\n\tpublisher    = {GitHub},\n\tdoi          = {10.21966/3cpa-2e10},\n\thowpublished = {\\url{https://github.com/HakaiInstitute/GlintMaskGenerator}},\n\tcommit       = {8cb19e55f128da86bf0dbd312bc360ac89fe71c3}\n}\n```\n\n## Development\n\nSee [DEVELOPMENT.md](DEVELOPMENT.md) for development and software maintenance instructions.\n\n## License\nGlintMaskGenerator is released under a MIT license, as found in the [LICENSE](LICENSE) file.\n',
+    'long_description': '# Glint Mask Tools\n\n<div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">\n    <img alt="Tests" src="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml/badge.svg"/>\n</a>\n\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/blob/main/LICENSE.txt">\n    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-black.svg" height="20px" />\n</a>\n\n<a href="https://badge.fury.io/py/glint-mask-tools">\n    <img alt="PyPI version" src="https://badge.fury.io/py/glint-mask-tools.svg" height="20">\n</a>\n\n<a href="https://zenodo.org/badge/latestdoi/266147098">\n    <img src="https://zenodo.org/badge/266147098.svg" alt="DOI">\n</a>\n</div>\n\n## Description\n\nGlintMaskGenerator generates image masks for regions in RGB and multispectral image files that have high levels of specular reflection.\n\nThese masks can be used in 3rd party structure-from-motion programs to replace these high glint regions with more useful data from adjacent, overlapping imagery.\n\n## Installation\n\n1. Go to the [releases page](https://github.com/HakaiInstitute/glint-mask-tools/releases)\n2. Download the latest release file for your operating system.\n3. Extract the compressed binary files from the gzipped archive.\n4. This archive contains a file named GlintMaskGenerator-v*.\\*.\\*.exe that provides a GUI interface to the glint mask generation program.\n5. You can copy these files to any location that is convenient for you.\n\n### PyPi package\n\nThere also a python package version of the code available for Python 3.8 and 3.9.\n\n1. `pip install glint-mask-tools` to install the tools.\n2. Then, `import glint_mask_generator` in your Python script.\n3. Installing with pip also installs the CLI tool, detailed below.\n\n## Usage\n\n### GUI\n\nIn Windows, launch the GUI by double clicking the executable file. In Linux, you\'ll have to launch the GUI from the\nterminal, e.g. `./GlintMaskGenerator`.\n\nFor now, generating masks by passing directory paths containing images is the supported workflow. Be sure to change the\nimage type option when processing imagery for cameras other than RGB cameras (e.g. Micasense RedEdge or DJI P4MS cameras). You will be notified of any\nprocessing errors via a pop-up dialog.\n\n### CLI\n\nFor information about the parameters expected by the CLI, run `glint-mask --help` in a bash terminal or command\nline interface. All the functionality of the CLI is documented there.\n\n#### Examples\n\n```bash\nglint-mask-v*.*.* --help\n\n# NAME\n#     glint-mask-v*.*.*\n# \n# SYNOPSIS\n#     glint-mask-v*.*.* - COMMAND | VALUE\n# \n# COMMANDS\n#     COMMAND is one of the following:\n# \n#      cir_threshold\n#        Generate masks for glint regions in 4 Band CIR imagery using Tom Bell\'s binning algorithm.\n# \n#      micasense_threshold\n#        Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell\'s algorithm on the blue image band.\n# \n#      p4ms_threshold\n#        Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell\'s algorithm on the Blue image band.\n# \n#      process\n# \n#      rgb_threshold\n#        Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# VALUES\n#     VALUE is one of the following:\n# \n#      max_workers\n#        The maximum number of threads to use for processing.\n```\n\n```bash\n# Get addition parameters for one of the cameras/methods available\nglint-mask-v*.*.* rgb_threshold --help\n\n# NAME\n#     glint-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# SYNOPSIS\n#     glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR <flags>\n# \n# DESCRIPTION\n#     Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# POSITIONAL ARGUMENTS\n#     IMG_DIR\n#         The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that directory will be # processed.\n#     OUT_DIR\n#         The path to send your out image including the file name and type. e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified as a # # # directory.\n# \n# FLAGS\n#     --thresholds=THRESHOLDS\n#         The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].\n#     --pixel_buffer=PIXEL_BUFFER\n#         The pixel distance to buffer out the mask. Defaults to 0 (off).\n# \n# NOTES\n#     You can also use flags syntax for POSITIONAL ARGUMENTS\n```\n\n```bash\n# Process rgb imagery directory with default parameters\nglint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process PhaseONE camera imagery with image bands split over multiple files\nglint-mask-v*.*.* aco_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process DJI P4MS imagery\nglint-mask-v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process Micasense RedEdge imagery \nglint-mask-v*.*.* micasense_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n```\n\n### Python package\nInstalling the PyPi package allows integrating the mask generation workflow into existing python scripts with ease.\n\n```python\nfrom glint_mask_generator import MicasenseRedEdgeThresholdMasker\n\n# Also available: P4MSThresholdMasker, RGBIntensityRatioMasker, RGBThresholdMasker\n\nmasker = MicasenseRedEdgeThresholdMasker(img_dir="path/to/micasense/images/", mask_dir="path/to/output/dir/",\n                                         thresholds=(0.875, 1, 1, 1, 1), pixel_buffer=5)\nmasker.process(max_workers=5, callback=print, err_callback=print)\n```\n\n## Notes\n\n### Directory of images processing\n\n- All files with "jpg", "jpeg", "tif", "tiff" and "png" extensions will be processed. This can be extended as needed.\n  File extension matching is case-insensitive.\n- Output mask files with be in the specified directory, and have the same name as the input file with "_mask" appended\n  to the end of the file name stem. The file type will match the input type.\n\n### Multi-band image processing\n- For imagery types where each band is spread over multiple files, a mask will be generated for all the sibling band images.\n    - For example, if a mask is generated using a threshold on the blue band image, identical masks are saved for sibling red, green, blue, nir, and red_edge bands as well.\n    - If thresholds are passed for multiple bands, these mask outputs combined with a union operator before being saved for all the sibling bands associated with that capture event.\n\n## Bugs and Feature Requests\n\nThis software is under active development. Bugs and feature requests can be filed using issues page located [here](https://github.com/HakaiInstitute/glint-mask-tools/issues).\n\n## Citation\n\nResearch using these tools or code should cite the following resources\n\n```bibtext\n@article{Cavanaugh2021,\n\ttitle        = {An Automated Method for Mapping Giant Kelp Canopy Dynamics from UAV},\n\tauthor       = {Cavanaugh, K.C. and Cavanaugh, K.C. and Bell, T.W. and Hockridge, E.G.},\n\tyear         = 2021,\n\tjournal      = {Front. Environ. Sci.},\n\tvolume       = {8:587354},\n\tdoi          = {10.3389/fenvs.2020.587354}\n}\n@misc{Denouden2021,\n\ttitle        = {GlintMaskGenerator},\n\tauthor       = {Denouden, T. and Timmer, B. and Reshitnyk, L.},\n\tyear         = 2021,\n\tjournal      = {GitHub repository},\n\tpublisher    = {GitHub},\n\tdoi          = {10.21966/3cpa-2e10},\n\thowpublished = {\\url{https://github.com/HakaiInstitute/GlintMaskGenerator}},\n\tcommit       = {8cb19e55f128da86bf0dbd312bc360ac89fe71c3}\n}\n```\n\n## Development\n\nSee [DEVELOPMENT.md](DEVELOPMENT.md) for development and software maintenance instructions.\n\n## License\nGlintMaskGenerator is released under a MIT license, as found in the [LICENSE](LICENSE) file.\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/HakaiInstitute/GlintMaskGenerator',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['glint_mask_generator'] package_data = \ {'': ['*']} install_requires = \
 ['Pillow>=9.3.0,<9.4.0', 'fire>=0.4.0,<0.5.0', 'loguru>=0.6.0,<0.7.0',
-'numpy>=1.23.5,<1.24.0', 'pyqt6>=6.4.0,<7.0.0', 'scipy>=1.9.3,<1.10.0',
+'numpy>=1.23.5,<1.24.0', 'pyqt6>=6.4.0,<7.0.0', 'scipy>=1.9.3,<1.11.0',
 'tqdm>=4.64.1,<4.65.0'] entry_points = \ {'console_scripts': ['glint-mask =
 glint_mask_generator.cli:main']} setup_kwargs = { 'name': 'glint-mask-tools',
-'version': '3.0.3', 'description': 'Create masks for specular reflection in UAV
+'version': '3.0.4', 'description': 'Create masks for specular reflection in UAV
 and aerial imagery', 'long_description': '# Glint Mask Tools\n\n
 \n\n_[Tests]\n\n\n\n_[License:_MIT]\n\n\n\n_[PyPI_version]\n\n\n\n_[DOI]\n\n
 \n\n## Description\n\nGlintMaskGenerator generates image masks for regions in
 RGB and multispectral image files that have high levels of specular
 reflection.\n\nThese masks can be used in 3rd party structure-from-motion
 programs to replace these high glint regions with more useful data from
 adjacent, overlapping imagery.\n\n## Installation\n\n1. Go to the [releases
```

### Comparing `glint_mask_tools-3.0.3/PKG-INFO` & `glint_mask_tools-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glint-mask-tools
-Version: 3.0.3
+Version: 3.0.4
 Summary: Create masks for specular reflection in UAV and aerial imagery
 Home-page: https://github.com/HakaiInstitute/GlintMaskGenerator
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,28 +12,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=9.3.0,<9.4.0)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: pyqt6 (>=6.4.0,<7.0.0)
-Requires-Dist: scipy (>=1.9.3,<1.10.0)
+Requires-Dist: scipy (>=1.9.3,<1.11.0)
 Requires-Dist: tqdm (>=4.64.1,<4.65.0)
 Project-URL: Repository, https://github.com/HakaiInstitute/GlintMaskGenerator
 Description-Content-Type: text/markdown
 
 # Glint Mask Tools
 
 <div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">
 <a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">
     <img alt="Tests" src="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml/badge.svg"/>
 </a>
 
 <a href="https://github.com/HakaiInstitute/GlintMaskGenerator/blob/main/LICENSE.txt">
-    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-darkgray.svg" height="20px" />
+    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-black.svg" height="20px" />
 </a>
 
 <a href="https://badge.fury.io/py/glint-mask-tools">
     <img alt="PyPI version" src="https://badge.fury.io/py/glint-mask-tools.svg" height="20">
 </a>
 
 <a href="https://zenodo.org/badge/latestdoi/266147098">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: glint-mask-tools Version: 3.0.3 Summary: Create
+Metadata-Version: 2.1 Name: glint-mask-tools Version: 3.0.4 Summary: Create
 masks for specular reflection in UAV and aerial imagery Home-page: https://
 github.com/HakaiInstitute/GlintMaskGenerator License: MIT Author: Taylor
 Denouden Author-email: taylor.denouden@hakai.org Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Pillow
 (>=9.3.0,<9.4.0) Requires-Dist: fire (>=0.4.0,<0.5.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: numpy (>=1.23.5,<1.24.0) Requires-Dist: pyqt6
-(>=6.4.0,<7.0.0) Requires-Dist: scipy (>=1.9.3,<1.10.0) Requires-Dist: tqdm
+(>=6.4.0,<7.0.0) Requires-Dist: scipy (>=1.9.3,<1.11.0) Requires-Dist: tqdm
 (>=4.64.1,<4.65.0) Project-URL: Repository, https://github.com/HakaiInstitute/
 GlintMaskGenerator Description-Content-Type: text/markdown # Glint Mask Tools
 [Tests] [License:_MIT] [PyPI_version] [DOI]
 ## Description GlintMaskGenerator generates image masks for regions in RGB and
 multispectral image files that have high levels of specular reflection. These
 masks can be used in 3rd party structure-from-motion programs to replace these
 high glint regions with more useful data from adjacent, overlapping imagery. ##
```

