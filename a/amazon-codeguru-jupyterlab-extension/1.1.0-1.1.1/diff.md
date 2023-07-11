# Comparing `tmp/amazon_codeguru_jupyterlab_extension-1.1.0.tar.gz` & `tmp/amazon_codeguru_jupyterlab_extension-1.1.1.tar.gz`

## Comparing `amazon_codeguru_jupyterlab_extension-1.1.0.tar` & `amazon_codeguru_jupyterlab_extension-1.1.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.eslintrc.js
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.stylelintrc
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/SECURITY.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/babel.config.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/jest.config.js
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/package.json
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/setup.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tsconfig.json
--rw-r--r--   0        0        0   456516 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/yarn.lock
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/cfg.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/codeguru.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/constants.py
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/diagnostics.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/plugin.py
--rw-r--r--   0        0        0    22393 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/build_log.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/install.json
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json
--rw-r--r--   0        0        0    42849 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js
--rw-r--r--   0        0        0    37569 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js.map
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js.map
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.b23847fa632c515c4b3e.js
--rw-r--r--   0        0        0    33982 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.b23847fa632c515c4b3e.js.map
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js.map
--rw-r--r--   0        0        0   593989 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js
--rw-r--r--   0        0        0   632582 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js.map
--rw-r--r--   0        0        0  6116687 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js
--rw-r--r--   0        0        0  6281464 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js.map
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js
--rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js.map
--rw-r--r--   0        0        0   848306 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js
--rw-r--r--   0        0        0   836060 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js.map
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/schema/plugin.json
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/index.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/svg.d.ts
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/About.tsx
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanButton.tsx
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanErrorPopup.tsx
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanStatus.tsx
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/icons.ts
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/index.ts
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/interface.ts
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/policy.ts
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/region.ts
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/utils/index.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/index.css
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/index.js
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/icons/cg-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0    11122 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_diagnostics.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_plugin.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/converted.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/finding.json
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/simple.ipynb
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/simple.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   125819 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/NOTICE
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/README.md
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/.eslintrc.js
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/.stylelintrc
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/SECURITY.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/babel.config.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/jest.config.js
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/package.json
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/setup.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tsconfig.json
+-rw-r--r--   0        0        0   456516 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/yarn.lock
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/cfg.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/codeguru.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/constants.py
+-rw-r--r--   0        0        0     8642 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/diagnostics.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/plugin.py
+-rw-r--r--   0        0        0    22393 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/build_log.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/install.json
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json
+-rw-r--r--   0        0        0    42849 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js
+-rw-r--r--   0        0        0    37569 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js.map
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js.map
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.68c99e6e8ba4eb207444.js
+-rw-r--r--   0        0        0    33982 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.68c99e6e8ba4eb207444.js.map
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js.map
+-rw-r--r--   0        0        0   593989 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js
+-rw-r--r--   0        0        0   632582 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js.map
+-rw-r--r--   0        0        0  6116687 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js
+-rw-r--r--   0        0        0  6281464 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js.map
+-rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js
+-rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js.map
+-rw-r--r--   0        0        0   848306 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js
+-rw-r--r--   0        0        0   836060 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js.map
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/schema/plugin.json
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/svg.d.ts
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/components/About.tsx
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/components/CodeScanButton.tsx
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/components/CodeScanErrorPopup.tsx
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/components/CodeScanStatus.tsx
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/constants/icons.ts
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/constants/index.ts
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/constants/interface.ts
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/constants/policy.ts
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/constants/region.ts
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/src/utils/index.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/style/index.css
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/style/index.js
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/style/icons/cg-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    11122 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/test_diagnostics.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/fixtures/converted.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/fixtures/finding.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/fixtures/simple.ipynb
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/tests/fixtures/simple.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   125819 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/NOTICE
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/README.md
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.1/PKG-INFO
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/.eslintrc.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/CONTRIBUTING.md` & `amazon_codeguru_jupyterlab_extension-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/jest.config.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/package.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/tsconfig.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/yarn.lock` & `amazon_codeguru_jupyterlab_extension-1.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/codeguru.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/codeguru.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/diagnostics.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,26 +171,28 @@
             "start": {"line": actual_start_line, "character": start_char},
             "end": {"line": actual_end_line, "character": end_char}
         },
         "severity": lsp.DiagnosticSeverity.Information if severity == 'Info' else lsp.DiagnosticSeverity.Warning
     }
 
 
-def get_diagnostics(workspace: Workspace, document: Document, overridden_region: str):
+def get_diagnostics(workspace: Workspace, document: Document, overridden_region: str, platform: str):
     codeguru_security = get_codeguru_security_client(overridden_region)
 
     with workspace.report_progress("command: runScan") as send_notification:
         send_notification({"status": CommandStatus.PENDING})
         is_nb_file = document.filename.endswith(".ipynb")
         path_to_nb = document.path.replace(".virtual_documents/", "")
         py_filepath = create_python_from_notebook(
             path_to_nb) if is_nb_file else document.path
         zip_filepath = create_zip_from_python(py_filepath)
-        scan_name = "{}-{}".format(os.path.basename(zip_filepath),
-                                   datetime.now().isoformat())
+        scan_name = "{}-{}-{}".format(platform, os.path.basename(zip_filepath),
+                                      datetime.now().isoformat())
+        # truncating scan name to avoid scan failure due to scan name character limit
+        scan_name = scan_name[:140]
         code_artifact_id = upload_file(
             zip_filepath, scan_name, codeguru_security, send_notification)
         run_id = create_scan(code_artifact_id, scan_name,
                              codeguru_security, send_notification)
         poll_scan_status(scan_name, run_id,
                          codeguru_security, send_notification)
         findings = get_scan_findings(
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/plugin.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,20 +31,25 @@
 @hookimpl
 def pylsp_execute_command(config: Config, workspace: Workspace, command: str, arguments: List[str]):
     logger.info("workspace/executeCommand: %s %s", command, arguments)
 
     if command == "cgs.runScan":
         doc_uri = arguments[0]
         overridden_region = arguments[1]
+        platform = arguments[2]
         document = workspace.get_document(doc_uri)
-        execute_run_scan(config, workspace, document, overridden_region)
+        execute_run_scan(config, workspace, document,
+                         overridden_region, platform)
 
 
 @hookimpl
 def pylsp_lint(config: Config, workspace: Workspace, document: Document, is_saved: bool):
     return cfg.diagnostics_by_document.get(document.uri)
 
 
-def execute_run_scan(config: Config, workspace: Workspace, document: Document, overridden_region: str):
-    other_diagnostics = get_diagnostics_from_other_sources(config, workspace, document)
-    cfg.diagnostics_by_document[document.uri] = get_diagnostics(workspace, document, overridden_region)
-    workspace.publish_diagnostics(doc_uri=document.uri, diagnostics=other_diagnostics + cfg.diagnostics_by_document.get(document.uri))
+def execute_run_scan(config: Config, workspace: Workspace, document: Document, overridden_region: str, platform: str):
+    other_diagnostics = get_diagnostics_from_other_sources(
+        config, workspace, document)
+    cfg.diagnostics_by_document[document.uri] = get_diagnostics(
+        workspace, document, overridden_region, platform)
+    workspace.publish_diagnostics(
+        doc_uri=document.uri, diagnostics=other_diagnostics + cfg.diagnostics_by_document.get(document.uri))
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/build_log.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/build_log.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999165743378706%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^3.6.5'}, '@jupyterlab/application-extension': {'requiredVersion': '^3.6.5'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^3.6.5'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^3.6.5'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^3.6.5'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^3.6.5'}, "*

 * *      "'@jupyterlab/colla […]*

```diff
@@ -120,442 +120,442 @@
                         "type": "var"
                     },
                     "name": "@aws/amazon-codeguru-extension",
                     "shared": {
                         "@aws/amazon-codeguru-extension": {
                             "import": "/Users/patmanth/workplace/sageMaker/amazon-codeguru-jupyterlab-extension/lib/index.js",
                             "singleton": true,
-                            "version": "1.0.0"
+                            "version": "1.1.0"
                         },
                         "@cloudscape-design/components": {},
                         "@cloudscape-design/global-styles": {},
                         "@jupyter-lsp/jupyterlab-lsp": {
                             "import": false,
                             "singleton": true
                         },
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^0.2.3",
+                            "requiredVersion": "^0.2.4",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/collaboration": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/collaboration-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.6.3",
+                            "requiredVersion": "^5.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.6.3"
+                            "requiredVersion": "^4.6.5"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.6.3",
+                            "requiredVersion": "^6.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/shared-models": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.6.3",
+                            "requiredVersion": "^5.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.6.3"
+                            "requiredVersion": "^5.6.5"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.5",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.5"
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/package.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9733187134502925%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.68c99e6e8ba4eb207444.js'}}",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -54,15 +54,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/aws/amazon-codeguru-jupyterlab-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b23847fa632c515c4b3e.js",
+            "load": "static/remoteEntry.68c99e6e8ba4eb207444.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "amazon-codeguru-jupyterlab-extension"
                 },
@@ -132,9 +132,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig` & `amazon_codeguru_jupyterlab_extension-1.1.1/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.1"
 }
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.b23847fa632c515c4b3e.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.68c99e6e8ba4eb207444.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -454,15 +454,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@aws/amazon-codeguru-extension", "1.0.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555"), __webpack_require__.e("vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516"), __webpack_require__.e("webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("@aws/amazon-codeguru-extension", "1.1.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555"), __webpack_require__.e("vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516"), __webpack_require__.e("webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                     register("@cloudscape-design/components", "3.0.264", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("vendors-node_modules_cloudscape-design_components_index_js"), __webpack_require__.e("vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555"), __webpack_require__.e("webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/@cloudscape-design/components/index.js */ "./node_modules/@cloudscape-design/components/index.js"))))));
                     /******/
                     register("@cloudscape-design/global-styles", "1.0.9", () => (__webpack_require__.e("node_modules_cloudscape-design_global-styles_dist_index_js").then(() => (() => (__webpack_require__( /*! ./node_modules/@cloudscape-design/global-styles/dist/index.js */ "./node_modules/@cloudscape-design/global-styles/dist/index.js"))))));
                     /******/
                 }
                 /******/
@@ -865,25 +865,25 @@
             /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1])),
             /******/
             "webpack/sharing/consume/default/react-dom": () => (loadSingletonVersionCheck("default", "react-dom", [1, 17, 0, 1])),
             /******/
             "webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp": () => (loadSingletonVersionCheck("default", "@jupyter-lsp/jupyterlab-lsp", [1, 4, 0, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 6, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 3, 6, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/statusbar": () => (loadSingletonVersionCheck("default", "@jupyterlab/statusbar", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/statusbar": () => (loadSingletonVersionCheck("default", "@jupyterlab/statusbar", [1, 3, 6, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 6, 5])),
             /******/
             "webpack/sharing/consume/default/@lumino/disposable": () => (loadSingletonVersionCheck("default", "@lumino/disposable", [1, 1, 10, 0])),
             /******/
             "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 10, 0])),
             /******/
             "webpack/sharing/consume/default/@cloudscape-design/components/@cloudscape-design/components": () => (loadStrictVersionCheckFallback("default", "@cloudscape-design/components", [1, 3, 0, 264], () => (__webpack_require__.e("vendors-node_modules_cloudscape-design_components_index_js").then(() => (() => (__webpack_require__( /*! @cloudscape-design/components */ "./node_modules/@cloudscape-design/components/index.js"))))))),
             /******/
@@ -1159,8 +1159,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@aws/amazon-codeguru-extension");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@aws/amazon-codeguru-extension"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.b23847fa632c515c4b3e.js.map
+//# sourceMappingURL=remoteEntry.68c99e6e8ba4eb207444.js.map
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.b23847fa632c515c4b3e.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.68c99e6e8ba4eb207444.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9149659863945578%*

 * *Differences: {"'file'": "'remoteEntry.68c99e6e8ba4eb207444.js'",*

 * * "'sourcesContent'": "{insert: [(11, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.b23847fa632c515c4b3e.js",
+    "file": "remoteEntry.68c99e6e8ba4eb207444.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC/BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8wBAA8wB;WAC5yB;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;;;;;WCJA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC/CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtMA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@aws/amazon-codeguru-extension/webpack/container-entry",
         "webpack://@aws/amazon-codeguru-extension/webpack/bootstrap",
         "webpack://@aws/amazon-codeguru-extension/webpack/runtime/compat get default export",
@@ -32,17 +32,17 @@
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"e6996744cc53a2504dda\",\"vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555\":\"b6fe59bfb98ab1ea02c7\",\"vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516\":\"faab484a03b81bb9ac8b\",\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\":\"2af4e6ad019522577bb2\",\"lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils\":\"c4c5385e7a8c0c90533a\",\"style_index_js\":\"cc72af7097c34762d4b6\",\"vendors-node_modules_cloudscape-design_components_index_js\":\"6c9ca9a4c8f822138168\",\"node_modules_cloudscape-design_global-styles_dist_index_js\":\"49bd81ccb2dba12e6001\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@aws/amazon-codeguru-extension:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.nmd = (module) => {\n\tmodule.paths = [];\n\tif (!module.children) module.children = [];\n\treturn module;\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@aws/amazon-codeguru-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@aws/amazon-codeguru-extension\", \"1.0.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555\"), __webpack_require__.e(\"vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"@cloudscape-design/components\", \"3.0.264\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_index_js\"), __webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@cloudscape-design/components/index.js */ \"./node_modules/@cloudscape-design/components/index.js\"))))));\n\t\t\tregister(\"@cloudscape-design/global-styles\", \"1.0.9\", () => (__webpack_require__.e(\"node_modules_cloudscape-design_global-styles_dist_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/@cloudscape-design/global-styles/dist/index.js */ \"./node_modules/@cloudscape-design/global-styles/dist/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@aws/amazon-codeguru-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@aws/amazon-codeguru-extension\", \"1.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555\"), __webpack_require__.e(\"vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"@cloudscape-design/components\", \"3.0.264\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_index_js\"), __webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555\"), __webpack_require__.e(\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@cloudscape-design/components/index.js */ \"./node_modules/@cloudscape-design/components/index.js\"))))));\n\t\t\tregister(\"@cloudscape-design/global-styles\", \"1.0.9\", () => (__webpack_require__.e(\"node_modules_cloudscape-design_global-styles_dist_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/@cloudscape-design/global-styles/dist/index.js */ \"./node_modules/@cloudscape-design/global-styles/dist/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-lsp/jupyterlab-lsp\", [1,4,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statusbar\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@cloudscape-design/components/@cloudscape-design/components\": () => (loadStrictVersionCheckFallback(\"default\", \"@cloudscape-design/components\", [1,3,0,264], () => (__webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_index_js\").then(() => (() => (__webpack_require__(/*! @cloudscape-design/components */ \"./node_modules/@cloudscape-design/components/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@cloudscape-design/global-styles/@cloudscape-design/global-styles\": () => (loadStrictVersionCheckFallback(\"default\", \"@cloudscape-design/global-styles\", [1,1,0,9], () => (__webpack_require__.e(\"node_modules_cloudscape-design_global-styles_dist_index_js\").then(() => (() => (__webpack_require__(/*! @cloudscape-design/global-styles */ \"./node_modules/@cloudscape-design/global-styles/dist/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/react-dom\"\n\t],\n\t\"lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@cloudscape-design/components/@cloudscape-design/components\"\n\t],\n\t\"style_index_js\": [\n\t\t\"webpack/sharing/consume/default/@cloudscape-design/global-styles/@cloudscape-design/global-styles\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-lsp/jupyterlab-lsp\", [1,4,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statusbar\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@cloudscape-design/components/@cloudscape-design/components\": () => (loadStrictVersionCheckFallback(\"default\", \"@cloudscape-design/components\", [1,3,0,264], () => (__webpack_require__.e(\"vendors-node_modules_cloudscape-design_components_index_js\").then(() => (() => (__webpack_require__(/*! @cloudscape-design/components */ \"./node_modules/@cloudscape-design/components/index.js\"))))))),\n\t\"webpack/sharing/consume/default/@cloudscape-design/global-styles/@cloudscape-design/global-styles\": () => (loadStrictVersionCheckFallback(\"default\", \"@cloudscape-design/global-styles\", [1,1,0,9], () => (__webpack_require__.e(\"node_modules_cloudscape-design_global-styles_dist_index_js\").then(() => (() => (__webpack_require__(/*! @cloudscape-design/global-styles */ \"./node_modules/@cloudscape-design/global-styles/dist/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/react-dom\"\n\t],\n\t\"lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@cloudscape-design/components/@cloudscape-design/components\"\n\t],\n\t\"style_index_js\": [\n\t\t\"webpack/sharing/consume/default/@cloudscape-design/global-styles/@cloudscape-design/global-styles\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@aws/amazon-codeguru-extension\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(\"webpack_sharing_consume_default_react-dom-webpack_sharing_consume_default_react\" != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_aws_amazon_codeguru_extension\"] = self[\"webpackChunk_aws_amazon_codeguru_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@aws/amazon-codeguru-extension\");\n",
         ""
     ],
     "version": 3
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js.map` & `amazon_codeguru_jupyterlab_extension-1.1.1/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js.map`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/schema/plugin.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/src/index.ts` & `amazon_codeguru_jupyterlab_extension-1.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/About.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.1/src/components/About.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanButton.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.1/src/components/CodeScanButton.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanErrorPopup.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.1/src/components/CodeScanErrorPopup.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanStatus.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.1/src/components/CodeScanStatus.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/style/base.css` & `amazon_codeguru_jupyterlab_extension-1.1.1/style/base.css`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/style/icons/cg-icon.svg` & `amazon_codeguru_jupyterlab_extension-1.1.1/style/icons/cg-icon.svg`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/tests/conftest.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_diagnostics.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_plugin.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/tests/test_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest.mock import ANY
 
 from amazon_codeguru_jupyterlab_extension import plugin
 from tests.conftest import *
 
+
 def test_settings():
     result = plugin.pylsp_settings()
     expected = {
         "plugins": {}
     }
     assert result == expected
 
@@ -29,27 +30,34 @@
     plugin.cfg.diagnostics_by_document = {}
     result = plugin.pylsp_lint(config, workspace, document, False)
     expected = None
     assert result == expected
 
 
 def test_execute_run_scan(config, workspace, document):
-    plugin.get_diagnostics_from_other_sources = Mock(return_value=[{"message": "1"}])
+    plugin.get_diagnostics_from_other_sources = Mock(
+        return_value=[{"message": "1"}])
     plugin.get_diagnostics = Mock(return_value=[{"message": "2"}])
     plugin.Workspace.publish_diagnostics = Mock()
-    plugin.execute_run_scan(config, workspace, document, "region")
-    plugin.get_diagnostics_from_other_sources.assert_called_once_with(config, workspace, document)
-    plugin.get_diagnostics.assert_called_once_with(workspace, document, "region")
-    plugin.Workspace.publish_diagnostics.assert_called_once_with(doc_uri=document.uri, diagnostics=[{"message": "1"}, {"message": "2"}])
+    plugin.execute_run_scan(config, workspace, document, "region", "jl")
+    plugin.get_diagnostics_from_other_sources.assert_called_once_with(
+        config, workspace, document)
+    plugin.get_diagnostics.assert_called_once_with(
+        workspace, document, "region", "jl")
+    plugin.Workspace.publish_diagnostics.assert_called_once_with(
+        doc_uri=document.uri, diagnostics=[{"message": "1"}, {"message": "2"}])
 
 
 def test_execute_command_run_scan(config, workspace, document):
     plugin.execute_run_scan = Mock()
     workspace.get_document = Mock(return_value=document)
-    plugin.pylsp_execute_command(config, workspace, "cgs.runScan", [document.uri, "region"])
-    plugin.execute_run_scan.assert_called_once_with(config, workspace, document, "region")
+    plugin.pylsp_execute_command(config, workspace, "cgs.runScan", [
+                                 document.uri, "region", "jl"])
+    plugin.execute_run_scan.assert_called_once_with(
+        config, workspace, document, "region", "jl")
 
 
 def test_execute_command_other(config, workspace):
     plugin.execute_run_scan = Mock()
-    plugin.pylsp_execute_command(config, workspace, "some-cmd", ["some", "args"])
+    plugin.pylsp_execute_command(
+        config, workspace, "some-cmd", ["some", "args"])
     assert not plugin.execute_run_scan.called
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/converted.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/tests/fixtures/converted.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/finding.json` & `amazon_codeguru_jupyterlab_extension-1.1.1/tests/fixtures/finding.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/README.md` & `amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/jupyter_server_test_config.py` & `amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/yarn.lock` & `amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts` & `amazon_codeguru_jupyterlab_extension-1.1.1/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/.gitignore` & `amazon_codeguru_jupyterlab_extension-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/LICENSE` & `amazon_codeguru_jupyterlab_extension-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/README.md` & `amazon_codeguru_jupyterlab_extension-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/pyproject.toml` & `amazon_codeguru_jupyterlab_extension-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.1.0/PKG-INFO` & `amazon_codeguru_jupyterlab_extension-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_codeguru_jupyterlab_extension
-Version: 1.1.0
+Version: 1.1.1
 Summary: Security, code quality, and ML recommendations
 Project-URL: Homepage, https://github.com/aws/amazon-codeguru-jupyterlab-extension
 Project-URL: Bug Tracker, https://github.com/aws/amazon-codeguru-jupyterlab-extension/issues
 Project-URL: Repository, https://github.com/aws/amazon-codeguru-jupyterlab-extension.git
 License-File: LICENSE
 License-File: NOTICE
 Classifier: Framework :: Jupyter
```

