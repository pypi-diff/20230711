# Comparing `tmp/mccoygroup-mcutils-0.1.1.tar.gz` & `tmp/mccoygroup-mcutils-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccoygroup-mcutils-0.1.1.tar", last modified: Wed Jul  5 17:50:18 2023, max compression
+gzip compressed data, was "mccoygroup-mcutils-0.1.1.1.tar", last modified: Tue Jul 11 18:52:59 2023, max compression
```

## Comparing `mccoygroup-mcutils-0.1.1.tar` & `mccoygroup-mcutils-0.1.1.1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.206547 mccoygroup-mcutils-0.1.1/McUtils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.206547 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/
--rw-r--r--   0 runner    (1001) docker     (123)   157171 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.206547 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/Conveniences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14789 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13283 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6157 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26533 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12958 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/DefaultConverters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8885 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3640 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1573 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/AtomData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/BondData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7160 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/CommonData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15316 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/ConstantsData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/PotentialData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7767 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/QuantityArray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/
--rwxr-xr-x   0 runner    (1001) docker     (123)   114295 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/AtomData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13861 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/BondData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61435 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/WavefunctionData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38079 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/DocWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/DocsBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/ExamplesParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/MarkdownTemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Extensions/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16442 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/ArgumentSignature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15111 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/CLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Module.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4699 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/ModuleLoader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7145 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/SharedLibraryManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/Babel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/OpenChem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7680 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/FChkDerivatives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5261 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13822 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianImporter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23349 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianLogComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/InteractiveTools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/ActiveHTMLWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.218548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   322229 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js
--rw-r--r--   0 runner    (1001) docker     (123)    43040 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js
--rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)   299473 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js
--rw-r--r--   0 runner    (1001) docker     (123)   289256 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.218548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)   750963 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2514969 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    52345 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    41729 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTML.py
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HackWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/JHTML.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/WidgetTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/MoleculeGraphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/NBExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Misc/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/DebugTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/Decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/FileMatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/NumbaTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/SBatchHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/Singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)    28255 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/Symbolics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateWriter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Numputils/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38376 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/AnalyticDerivs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3743 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/EulerSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/Misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/Options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/SetOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    95985 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/Sparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7552 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationMatrices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationTransformations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/VectorOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/
--rw-r--r--   0 runner    (1001) docker     (123)    58677 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Parallelizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/SharedMemory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/FileStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/Parsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36223 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/RegexPatterns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43416 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/StringParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48561 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/StructuredType.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Plots/
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Backends.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    71035 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12351 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Interactive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45079 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29775 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Properties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9360 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Styling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19806 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/VTKInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/CLIs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Caches.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Checkpointing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21633 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/ObjectBackers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6989 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/FittableModels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19361 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Interpolator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/LazyTensors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    81351 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/NeighborBasedInterpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Polynomials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7602 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/BaseSurface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/Surface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)    64296 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)    73503 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30417 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/Derivatives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34945 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19721 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5570 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/
+-rw-r--r--   0 runner    (1001) docker     (123)   166453 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/Conveniences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14789 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13283 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6157 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26533 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12958 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/DefaultConverters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8885 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3640 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1573 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/AtomData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/BondData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7160 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/CommonData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15316 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/ConstantsData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/PotentialData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7767 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/QuantityArray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114295 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/AtomData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13861 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/BondData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61435 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/WavefunctionData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38079 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocsBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/ExamplesParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/MarkdownTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16442 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ArgumentSignature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15111 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/CLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4699 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ModuleLoader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7145 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/SharedLibraryManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/Babel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/OpenChem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7680 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/FChkDerivatives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5261 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13822 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianImporter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23349 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianLogComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/InteractiveTools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/ActiveHTMLWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   322229 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43040 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)   299473 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js
+-rw-r--r--   0 runner    (1001) docker     (123)   289256 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.231823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)   750963 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2514969 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.231823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52345 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41729 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HackWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/JHTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/WidgetTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/MoleculeGraphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/NBExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/DebugTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/FileMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/NumbaTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/SBatchHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28255 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Symbolics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateWriter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38376 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/AnalyticDerivs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3743 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/EulerSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/SetOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    95985 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Sparse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7552 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationMatrices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationTransformations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/VectorOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    58677 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Parallelizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/SharedMemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/FileStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/Parsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36223 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/RegexPatterns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43416 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StringParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48561 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StructuredType.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Backends.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71035 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12351 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Interactive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45079 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29775 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9360 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Styling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19806 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/VTKInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/CLIs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Checkpointing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21633 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/ObjectBackers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6989 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/FittableModels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19361 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Interpolator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/LazyTensors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81351 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/NeighborBasedInterpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19119 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Polynomials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7602 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/BaseSurface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/Surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)    64296 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73503 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30417 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/Derivatives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34945 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19721 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5570 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-11 18:52:59.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/setup.py
```

### Comparing `mccoygroup-mcutils-0.1.1/LICENSE.txt` & `mccoygroup-mcutils-0.1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/MANIFEST.in` & `mccoygroup-mcutils-0.1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Permutations.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Permutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from ..Misc import jit, objmode, prange
 from ..Numputils import flatten_dtype, unflatten_dtype, difference as set_difference, unique, contained, group_by, split_by_regions, find, infer_int_dtype
 from ..Scaffolding import NullLogger
 
 __all__ = [
     "IntegerPartitioner",
     "UniquePermutations",
+    "UniqueSubsets",
+    "UniquePartitions",
     "IntegerPartitionPermutations",
     "SymmetricGroupGenerator",
     "CompleteSymmetricGroupSpace",
     "LatticePathGenerator",
     "PermutationRelationGraph"
 ]
 
@@ -438,14 +440,53 @@
 
         inds = num_before
         if smol:
             inds = inds[0]
 
         return inds
 
+class UniqueSubsets:
+    """
+    Provides unique subsets for an integer partition
+    """
+    def __init__(self, partition):
+        # self.part = np.flip(np.sort(partition))
+        self.part = partition
+        neg_part = -partition # so we can build ordered partitions
+        sorting = np.argsort(neg_part)
+        sort_part = neg_part[sorting]
+        v, idx, c = np.unique(sort_part, return_index=True, return_counts=True) # could use `nput.unique` to reuse sorting
+        self.idx = np.split(sorting, idx[1:])
+        self.vals = -v
+        self.counts = c
+        self.dim = len(partition)
+        self._vals_dim = len(self.vals)
+        self._num = None
+        self._tree = {}
+        self._otree = {} # cache ordered subsets for efficiency
+
+    def get_subsets(self, targ_len, ordered=False):
+        # TODO: use sparse encodings to speed up
+        if targ_len == 0:
+            return np.zeros((1, self._vals_dim))
+        if targ_len == 1:
+            return np.eye(self._vals_dim)
+        if targ_len not in self._tree:
+            base = self.get_subsets(targ_len-1)[np.newaxis, :, :] + np.eye(self._vals_dim)[:, np.newaxis, :]
+            base = base.reshape(-1, self._vals_dim)
+            valid_sets = np.all(base <= self.counts[np.newaxis], axis=1)
+            self._tree[targ_len] = base[valid_sets,]
+
+        subsets = self._tree[targ_len]
+        if ordered: # construct ordered subsets
+            # for each subset we need to
+            raise ValueError("ah fuck")
+
+        return subsets
+
 class UniquePermutations:
     """
     Provides permutations for a _single_ integer partition (very important)
     Also provides a classmethod interface to support the case
     where we don't want to instantiate a permutations object for every partition
     """
     def __init__(self, partition):
@@ -1573,14 +1614,204 @@
                     # now...we know what the permutation looks like in terms of the classes itself????
                     # except...I'm not totally sure how to put this
                     permutation_indices[cur_dim:] = np.arange(cur_dim, )
                     break
 
             on_visit(tree_data[cur_dim, 0], permutation_indices, tree_data)
 
+class UniquePartitions:
+    """
+    Takes partitions of a set of ints with ordering
+    """
+    def __init__(self, partition):
+        partition = np.asanyarray(partition)
+        self.part = partition
+        self.perms = UniquePermutations(np.sort(partition)).permutations()
+        neg_part = -partition  # so we can build ordered partitions
+        sorting = np.argsort(neg_part)
+        sort_part = neg_part[sorting]
+        v, idx, c = np.unique(sort_part, return_index=True,
+                              return_counts=True)  # could use `nput.unique` to reuse sorting
+        split_idx = np.split(sorting, idx[1:])
+        final_indices = [x[-1] for x in split_idx]
+        self.followers = np.array([
+            [np.sum((x - f) > 0) for x in split_idx]
+            for f in final_indices
+        ])
+
+    @classmethod
+    def _take_partitions(self, partition, sizes, take_unique=True,
+                         split=True,
+                         return_partitions=True,
+                         return_indices=None, split_indices=None,
+                         return_inverse=False, split_inverse=None
+                         ):
+        if not return_partitions and not return_indices and not return_inverse:
+            raise ValueError("need to return _something_")
+        if not return_partitions and take_unique:
+            raise ValueError("need to calculate partitions to return unique")
+        if return_inverse and return_indices is None:
+            return_indices = True
+        elif return_inverse and not return_indices:
+            raise ValueError("inverse but no indices feels wasteful")
+
+        tree_sizes = []
+        ind_blocks = []
+        n = m = len(partition)
+        for size in sizes: # we prep a bunch of data to feed to numba
+            # tree_sizes.append( # binomial terms at each size
+            #     np.math.factorial(m) / (
+            #             np.math.factorial(size) * np.math.factorial(m - size)
+            #     )
+            # )
+            if size > 0:
+                ind_blocks.append(np.array(
+                    list(itertools.combinations(range(m), size)),
+                    dtype=int
+                ))
+                tree_sizes.append(len(ind_blocks[-1]))
+                m -= size
+
+        total_terms = np.prod(tree_sizes, dtype=int)
+
+        if return_partitions:
+            subs = np.full((total_terms, n), -1, dtype=int)
+        else:
+            subs = None
+
+        if return_indices:
+            inds = np.zeros((total_terms, n), dtype=int)
+        else:
+            inds = None
+
+        N = len(subs) if subs is not None else len(inds)
+        self._populate_partitions(partition, [s for s in sizes if s > 0], tree_sizes, ind_blocks, N, subs, inds)
+
+        # TODO: find a way to handle unique masking inside numba loop
+        if take_unique:
+            uu = np.unique(partition)
+            if len(uu) <= len(partition):
+                _, _, sort_uinds = unique(subs, axis=0, return_index=True)
+                uinds = np.sort(sort_uinds)
+                subs = subs[uinds,]
+                if return_indices:
+                    inds = inds[uinds,]
+            # raise NotImplementedError(...)
+
+        if return_inverse:
+            inv = np.argsort(inds, axis=1)
+        else:
+            inv = None
+
+        if split:
+            splits = np.cumsum(sizes)
+            if return_partitions:
+                subs = np.split(subs, splits[:-1], axis=1)
+            if return_indices and (split_indices or split_indices is None):
+                inds = np.split(inds, splits[:-1], axis=1)
+            if return_inverse and (split_inverse or split_inverse is None):
+                inv = np.split(inv, splits[:-1], axis = 1)
+
+        ret = ()
+        if return_partitions:
+            ret += (subs,)
+        if return_indices:
+            ret += (inds,)
+        if return_inverse:
+            ret += (inv,)
+        return ret
+    @staticmethod
+    @jit(nopython=True, cache=True)
+    def _populate_partitions(partition, sizes, tree_sizes, blocks, N, subs, inds):
+        """
+        :param partition:
+        :param tree_sizes:
+        :param blocks: blocks of indices to sample from the partition
+        :param subs:
+        :return:
+        """
+
+        k = len(sizes)
+        p = len(partition)
+        bs = np.concatenate([[0], np.cumsum(sizes)]) # block starts
+        r = np.arange(p) # for remainder indices
+        for i in range(N): # product of tree/block shapes
+            # these assertions sometimes help numba
+            assert i >= 0
+            assert i < N
+            product_index = np.unravel_index(i, tree_sizes) # would be nicer to have a faster process...
+            mask = np.full(p, True, dtype=bool)
+            # print("????")
+            for j in range(k):
+                # print(">>>", mask)
+                block_idx = blocks[j][product_index[j]]
+                if subs is not None:
+                    subs[i][bs[j]:bs[j+1]] = partition[mask][block_idx]
+                if inds is not None:
+                    inds[i][bs[j]:bs[j + 1]] = r[mask][block_idx]
+                mask[r[mask][block_idx]] = False
+                # print(" > ", mask, block_idx)
+
+    # @classmethod
+    # def get_follower_counts(cls, partition):
+    #     followers = {}
+    #     for x in partition:
+    #         followers[x] = {}
+    #         for y in followers:
+    #             if y != x:
+    #                 followers[y][x] = followers[y].get(x, 0) + 1
+    #     return followers
+
+    def partitions(self, sizes,
+                   take_unique=True, split=True,
+                   return_partitions=True,
+                   return_indices=False, split_indices=None,
+                   return_inverse=False, split_inverse=None):
+        if np.sum(sizes) != len(self.part):
+            raise ValueError("sum of sizes must be length of partition")
+        sizes = np.asanyarray(sizes).astype(int)
+        return self._take_partitions(self.part, sizes,
+                                     take_unique=take_unique, split=split,
+                                     return_partitions=return_partitions,
+                                     return_indices=return_indices, split_indices=split_indices,
+                                     return_inverse=return_inverse, split_inverse=split_inverse)
+
+        # # O(d*N) where d is the length of the partition and
+        # #
+        # if len(sizes) == 1:
+        #     return self.part[np.newaxis]
+        # non_zs = np.where(sizes > 0)[0]
+        # if len(non_zs) == 1: # only one non-zero
+        #     return [
+        #         np.zeros((1, 0)) if s == 0 else self.part[np.newaxis]
+        #         for s in sizes
+        #     ]
+        #
+        # splits = np.cumsum(sizes)
+        # perm_splits = np.split(self.perms, splits[:-1], axis=1)
+        # good_places = np.arange(len(self.perms))
+        # mask = np.full(len(good_places), True, dtype=bool)
+        # # for i in range()
+        # for subperms in perm_splits:
+        #     if subperms.shape[1] > 1: # if len 1 or less can't be misordered...
+        #         for i,partition in enumerate(subperms[good_places]):
+        #             followers = {}
+        #             for x in partition:
+        #                 followers[x] = {}
+        #                 for y in followers:
+        #                     if y != x:
+        #                         followers[y][x] = followers[y].get(x, 0) + 1
+        #
+        #
+        #
+        #
+        # raise Exception([p.shape for p in perm_splits], self.part, sizes)
+
+
+
 class IntegerPartitionPermutations:
     """
     Provides tools for working with permutations of a given integer partition
     """
     def __init__(self, num, dim=None):
         self.int = num
         if dim is None:
@@ -2066,17 +2297,18 @@
 
         partitioners, shifts = self._get_partition_perms(usums)
         perms_inds = [p.get_partition_permutation_indices(g,
                                                  assume_standard=assume_standard,
                                                  preserve_ordering=preserve_ordering,
                                                  check_partition_counts=check_partition_counts) for p, g in zip(partitioners, groups) ]
         if dtype is None:
-        #     for i,p in enumerate(perms_inds):
-        #         if np.any(p < 0):
-        #             raise ValueError("dtype overflow on {}".format(groups[i]))
+            # for i,p in enumerate(perms_inds):
+            #     min_p = np.min(p)
+            #     if min_p < 0:
+            #         raise ValueError("dtype overflow on {}".format(groups[i]))
             dtype = _infer_dtype(np.max([np.max(p) for p in perms_inds]) + np.max(shifts))
         subinds = [ (g.astype(dtype) + s) for g,s in zip(perms_inds, shifts) ]
         indices = np.concatenate(subinds, axis=0)
 
         if preserve_ordering and sorting is not None:
             indices = indices[np.argsort(sorting)]
 
@@ -2128,14 +2360,17 @@
             self._get_partition_perms([1+len(self._partition_permutations)*2])
 
         insertion_spots = np.searchsorted(self._cumtotals - 1, indices, sorter=np.arange(len(self._cumtotals)))
         uinds, _, inds = unique(insertion_spots, sorting=np.arange(len(insertion_spots)), return_index=True)
         groups = np.split(indices, inds)[1:]
         uinds = uinds - 1
 
+        if min(uinds) < 0:
+            raise ValueError("bad indices: {}".format(np.min(indices), np.max(indices)))
+
         partitioners, shifts = self._get_partition_perms(uinds)
 
         shifted_groups = [g - s for g,s in zip(groups, shifts)]
         # raise Exception(partitioners, shifted_groups, shifts)
         # wat = partitioners[0] # type: IntegerPartitionPermutations
         perms = np.concatenate([ p.get_partition_permutations_from_indices(g, preserve_ordering=preserve_ordering) for p,g in zip(partitioners, shifted_groups)], axis=0)
 
@@ -2357,14 +2592,15 @@
                 for b, s in zip(block_dat['idx_blocs'], np.split(sort_mask, block_sizes)):
                     perm_counts[b[0]:b[1], b[2]] -= 1 - s
 
                 # filter_from_ind_spec(i, j, block_idx, block_sizes, perm_pos, full_inds_sorted, inv)
 
     @classmethod
     def changed_index_number(cls, idx, radix):
+        if len(idx) == 0: return 0
         return np.ravel_multi_index(np.sort(idx)+1, [radix+1]*len(idx))
     @classmethod
     def _compute_changed_index_numbers(cls, mask):
         # we loop for this because I'm not totally sure how to do better here...
         if not mask.any():
             return np.zeros(len(mask))
         radix = len(mask[0])
```

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Sequences.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Sequences.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/Conveniences.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/Conveniences.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/AtomData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/AtomData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/BondData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/BondData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/CommonData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/CommonData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/ConstantsData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/ConstantsData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/PotentialData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/PotentialData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/QuantityArray.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/QuantityArray.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/AtomData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/AtomData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/BondData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/BondData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/WavefunctionData.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/WavefunctionData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Data/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Docs/DocWalker.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocWalker.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Docs/DocsBuilder.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocsBuilder.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Docs/ExamplesParser.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/ExamplesParser.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Docs/MarkdownTemplates.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/MarkdownTemplates.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/ArgumentSignature.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ArgumentSignature.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/CLoader.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/CLoader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Loader.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Loader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Module.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Module.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/ModuleLoader.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ModuleLoader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/SharedLibraryManager.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/SharedLibraryManager.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Extensions/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/Babel.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/Babel.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/OpenChem.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/OpenChem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/FChkDerivatives.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/FChkDerivatives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianImporter.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianImporter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianJob.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianJob.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianLogComponents.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianLogComponents.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Apps.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Apps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Controls.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Controls.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Interfaces.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Interfaces.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Variables.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Variables.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/types.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/types.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/InteractiveTools.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/InteractiveTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Bootstrap.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Bootstrap.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Enums.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Enums.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTML.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTML.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HackWidgets.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HackWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/JHTML.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/JHTML.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/WidgetTools.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/WidgetTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/MoleculeGraphics.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/MoleculeGraphics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/NBExporter.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/NBExporter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/DebugTools.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/DebugTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/FileMatcher.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/FileMatcher.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/NumbaTools.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/NumbaTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/SBatchHelper.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/SBatchHelper.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/Symbolics.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Symbolics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateWriter.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateWriter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Misc/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/AnalyticDerivs.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/AnalyticDerivs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/EulerSystem.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/EulerSystem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/Misc.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # elif max_size < 4294967295:
     #     minimal_dtype = 'uint32'
     # else:
     #     minimal_dtype = 'uint64'
     # return minimal_dtype
 
 def infer_int_dtype(max_dim):
-    return np.min_scalar_type(-max_dim)
+    return np.min_scalar_type(-(max_dim+1))
     # max_dim = abs(max_dim)
     # if max_dim < 128:
     #     minimal_dtype = 'int8'
     # elif max_dim < 32768:
     #     minimal_dtype = 'int16'
     # elif max_dim < 2147483648:
     #     minimal_dtype = 'int32'
```

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/Options.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Options.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/SetOps.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/SetOps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/Sparse.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Sparse.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationMatrices.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationMatrices.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationTransformations.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationTransformations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/VectorOps.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/VectorOps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Numputils/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Parallelizers.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Parallelizers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Runner.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Runner.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/SharedMemory.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/SharedMemory.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parsers/FileStreamer.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/FileStreamer.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parsers/Parsers.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/Parsers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parsers/RegexPatterns.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/RegexPatterns.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parsers/StringParser.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StringParser.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parsers/StructuredType.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StructuredType.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Parsers/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Graphics.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Graphics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Image.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Image.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Interactive.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Interactive.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Plots.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Plots.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Primitives.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Primitives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Properties.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Properties.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/Styling.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Styling.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/VTKInterface.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/VTKInterface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Plots/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/CLIs.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/CLIs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Caches.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Caches.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Checkpointing.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Checkpointing.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Configurations.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Configurations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Jobs.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Jobs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Logging.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Logging.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/ObjectBackers.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/ObjectBackers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Persistence.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Persistence.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Schema.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Schema.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Serializers.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Serializers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/FittableModels.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/FittableModels.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Interpolator.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Interpolator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/LazyTensors.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/LazyTensors.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Mesh.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Mesh.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/NeighborBasedInterpolators.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/NeighborBasedInterpolators.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Polynomials.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Polynomials.py`

 * *Files 4% similar despite different names*

```diff
@@ -335,19 +335,27 @@
     A semi-symbolic representation of a polynomial of tensor
     coefficients
     """
     def __init__(self, terms:dict, prefactor=1):
         self.terms = terms
         self.prefactor = prefactor
         self._shape = None
+
+    @property
+    def scaling(self):
+        return 1 if self.prefactor is None else self.prefactor
+    @scaling.setter
+    def scaling(self, s):
+        self.prefactor = s
+
     def expand(self):
         if self.prefactor == 1:
             return self
         else:
-            return SparsePolynomial({k:self.prefactor*v for k,v in self.terms.items()}, prefactor=1)
+            return type(self)({k:self.prefactor*v for k,v in self.terms.items()}, prefactor=1)
     @classmethod
     def monomial(cls, idx, value=1):
         return cls({idx:value})
     def __repr__(self):
         return "{}({},{})".format(type(self).__name__, self.terms,self.prefactor)
 
     def __mul__(self, other):
@@ -360,17 +368,17 @@
             new_terms = {}
             for k,v in other.terms.items():
                 for k2,v2 in self.terms.items():
                     t = tuple(sorted(k + k2))
                     new_terms[t] = new_terms.get(t, 0) + v * v2
                     if new_terms[t] == 0:
                         del new_terms[t]
-            return SparsePolynomial(new_terms, prefactor=self.prefactor*other.prefactor)
+            return type(self)(new_terms, prefactor=self.prefactor*other.prefactor)
         else:
-            return SparsePolynomial(self.terms, prefactor=self.prefactor*other)
+            return type(self)(self.terms, prefactor=self.prefactor*other)
             # new_terms = {}
             # for k,v in self.terms.items():
             #     new_terms[k] = self.prefactor*other*v
             # return SparsePolynomial(new_terms)
     def __add__(self, other):
         if isinstance(other, (int, float, np.integer, np.floating)):
             if other == 0:
@@ -437,14 +445,18 @@
         raise ValueError("{} doesn't have a dense counterpart".format(type(self).__name__))
     def as_dense(self):
         raise ValueError("{} doesn't have a dense counterpart".format(type(self).__name__))
     def shift(self, shift) -> DensePolynomial:
         raise ValueError("{} doesn't have a dense counterpart".format(type(self).__name__))
 
     @classmethod
+    def monomial(cls, idx, value=1):
+        return cls({(idx,): value})
+
+    @classmethod
     def key_hash(cls, monomial_tuple):
         # hashes tuples of indices to give a fast check that the tuples
         # are the same independent of ordering
         return sum(hash(x) for x in monomial_tuple)
 
     @classmethod
     @abc.abstractmethod
@@ -452,15 +464,16 @@
         raise NotImplementedError("{} is abstract".format(cls.__name__))
 
     def __mul__(self, other):
         if isinstance(other, (int, float, np.integer, np.floating)):
             if other == 1:
                 return self
             elif other == 0:
-                return type(self)({})
+                return 0
+                # return type(self)({})
         if isinstance(other, PureMonicPolynomial):
             new_terms = {}
             term_hashes = {}
             for k,v in other.terms.items():
                 for k2,v2 in self.terms.items():
                     new_hash = self.key_hash(k) + self.key_hash(k2)
                     if new_hash in term_hashes:
@@ -487,17 +500,17 @@
         s_groups = {}
         for index_tuple in monomial_tuple:
             l = len(index_tuple)
             grp = s_groups.get(l, [])
             s_groups[l] = grp
             grp.append(index_tuple)
         t = tuple(
-            i
-            for k in sorted(s_groups.keys())
-            for i in sorted(s_groups[k])
+            grp
+            for l in sorted(s_groups.keys())
+            for grp in sorted(s_groups[l])
         )
         return t
 
 # class TensorCoeffPoly(AbstractPolynomial):
 #     """
 #     A semi-symbolic representation of a polynomial of tensor
 #     coefficients
```

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/BaseSurface.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/BaseSurface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/Surface.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/Surface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/Derivatives.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/Derivatives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/Zachary/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/McUtils/__init__.py` & `mccoygroup-mcutils-0.1.1.1/McUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/PKG-INFO` & `mccoygroup-mcutils-0.1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-mcutils
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # McUtils [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mccoygroup/binder-mcutils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmccoygroup%252FMcUtils%26urlpath%3Dlab%252Ftree%252FMcUtils%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-mcutils-0.1.1/README.md` & `mccoygroup-mcutils-0.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/PKG-INFO` & `mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-mcutils
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # McUtils [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mccoygroup/binder-mcutils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmccoygroup%252FMcUtils%26urlpath%3Dlab%252Ftree%252FMcUtils%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt` & `mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1/setup.py` & `mccoygroup-mcutils-0.1.1.1/setup.py`

 * *Files identical despite different names*

