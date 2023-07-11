# Comparing `tmp/tvb_ext_bucket-0.3.0.tar.gz` & `tmp/tvb_ext_bucket-1.0.0.tar.gz`

## Comparing `tvb_ext_bucket-0.3.0.tar` & `tvb_ext_bucket-1.0.0.tar`

### file list

```diff
@@ -1,79 +1,84 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/.eslintrc.js
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/.prettierrc
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/babel.config.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/conftest.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/jest.config.js
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/setup.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tsconfig.json
--rw-r--r--   0        0        0   454119 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/yarn.lock
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/jupyter-config/nb-config/tvb_ext_bucket.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/jupyter-config/server-config/tvb_ext_bucket.json
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/BucketContext.tsx
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/BucketSearch.tsx
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/BucketWidget.tsx
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/CollabSpaceEntry.tsx
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/ContextMenu.tsx
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/ContextMenuItem.tsx
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/DragDownload.tsx
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/DropZone.tsx
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/FileTransferAnimations.tsx
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/JpFileBrowser.ts
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/JpSpinner.tsx
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/Tooltip.tsx
--rw-r--r--   0        0        0    14489 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/bucketFileBrowser.ts
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/exceptions.ts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/handler.ts
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/hooks.ts
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/index.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/utils.ts
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/__tests__/BucketWidget.spec.tsx
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/__tests__/ContextMenu.spec.tsx
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/__tests__/bucketFileBrowser.spec.ts
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/__tests__/testUtils.ts
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/src/__tests__/utils.spec.ts
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/Collaboratory_EBRAINS.svg
--rw-r--r--   0        0        0    50766 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/Collaboratory_bucket_simple.png
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/base.css
--rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/ebrains_logo.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/hdd-o-4.svg
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/style/index.js
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/_version.py
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/ebrains_drive_wrapper.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/exceptions.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/__init__.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/bucket.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/bucket_api.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/buckets.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/dataproxy_file.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/package.json
--rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/529.3f5fcb349df6ed19fa54.js
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/747.8201db85e4d2a978f4c3.js
--rw-r--r--   0        0        0    50766 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/acb28ef48e64b689e3e44624dd56425825ae6f016b1ff6d65e9004f9d15b3301.png
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/remoteEntry.b2ee1fefe23289008a39.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/logger/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/logger/builder.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/logger/logging.conf
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/__init__.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_bucket.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_buckets.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_dataproxy_file.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_drive_wrapper.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_handlers.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/LICENSE
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/README.md
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    45863 2020-02-02 00:00:00.000000 tvb_ext_bucket-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/.prettierrc
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/babel.config.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/conftest.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/jest.config.js
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/setup.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/sonar-project.properties
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tsconfig.json
+-rw-r--r--   0        0        0   454119 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/yarn.lock
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/jupyter-config/nb-config/tvb_ext_bucket.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/jupyter-config/server-config/tvb_ext_bucket.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/BucketContext.tsx
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/BucketSearch.tsx
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/BucketWidget.tsx
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/CollabSpaceEntry.tsx
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/ContextMenu.tsx
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/ContextMenuItem.tsx
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/DragDownload.tsx
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/DropZone.tsx
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/FileTransferAnimations.tsx
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/JpFileBrowser.ts
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/JpSpinner.tsx
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/Settings.tsx
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/Tooltip.tsx
+-rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/bucketFileBrowser.ts
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/exceptions.ts
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/handler.ts
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/index.ts
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/__tests__/BucketWidget.spec.tsx
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/__tests__/ContextMenu.spec.tsx
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/__tests__/bucketFileBrowser.spec.ts
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/__tests__/testUtils.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/__tests__/utils.spec.ts
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/hooks/useBucketSearch.ts
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/hooks/useOuterClickClosable.ts
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/hooks/useStoredState.ts
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/utils/bucketUtils.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/src/utils/domUtils.ts
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/Collaboratory_EBRAINS.svg
+-rw-r--r--   0        0        0    50766 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/Collaboratory_bucket_simple.png
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/base.css
+-rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/ebrains_logo.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/hdd-o-4.svg
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/style/index.js
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/_version.py
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/ebrains_drive_wrapper.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/exceptions.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/__init__.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/bucket.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/bucket_api.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/buckets.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/dataproxy_file.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/package.json
+-rw-r--r--   0        0        0    23160 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/522.88137ffbe3671c70bd7e.js
+-rw-r--r--   0        0        0    11663 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/747.e24cd10495543003a807.js
+-rw-r--r--   0        0        0    50766 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/acb28ef48e64b689e3e44624dd56425825ae6f016b1ff6d65e9004f9d15b3301.png
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/remoteEntry.c935a8c2bed6559fef34.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/logger/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/logger/builder.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/logger/logging.conf
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/__init__.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_bucket.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_buckets.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_dataproxy_file.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_drive_wrapper.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_handlers.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/README.md
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    45863 2020-02-02 00:00:00.000000 tvb_ext_bucket-1.0.0/PKG-INFO
```

### Comparing `tvb_ext_bucket-0.3.0/.eslintrc.js` & `tvb_ext_bucket-1.0.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/RELEASE.md` & `tvb_ext_bucket-1.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/jest.config.js` & `tvb_ext_bucket-1.0.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/package.json` & `tvb_ext_bucket-1.0.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -113,9 +113,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "1.0.0"
 }
```

### Comparing `tvb_ext_bucket-0.3.0/tsconfig.json` & `tvb_ext_bucket-1.0.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/yarn.lock` & `tvb_ext_bucket-1.0.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/BucketSearch.tsx` & `tvb_ext_bucket-1.0.0/src/BucketSearch.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,46 @@
-import React from 'react';
-import { IBucketSearch } from './hooks';
+import React, { forwardRef } from 'react';
+import { IBucketSearch } from './hooks/useBucketSearch';
 
-export const BucketSearch: React.FC<BucketSearch.IProps> = ({
-  data,
-  showList
-}) => {
-  return (
-    <div>
-      {data.loading ? (
-        <span className={'jp-Spinner'} />
-      ) : (
-        <>
-          <span className={'error'}>{(data.error as Error).toString()}</span>
-
-          <select
-            name={'bucket'}
-            id={'bucket'}
-            autoFocus={true}
-            value={data.chosenValue}
-            onChange={ev => data.setChosenValue(ev.target.value)}
-            style={{ display: 'none' }}
-          >
-            {data.searchMatchingValues.map(val => {
-              return (
-                <option value={val} key={val}>
-                  {val}
-                </option>
-              );
-            })}
-          </select>
-          <ul
-            className={'available-buckets'}
-            style={{ visibility: showList ? 'visible' : 'hidden' }}
-          >
-            {data.searchMatchingValues.map(val => {
-              return (
-                <li
-                  onClick={_ev => {
-                    data.setChosenValue(val);
-                  }}
-                  key={val}
-                >
-                  {val}
-                </li>
-              );
-            })}
-          </ul>
-        </>
-      )}
-    </div>
-  );
-};
+export const BucketSearch = forwardRef<HTMLDivElement, BucketSearch.IProps>(
+  ({ data, showList, setShowList }, ref) => {
+    const { error, loading, searchMatchingValues, setChosenValue } = data;
+    return (
+      <div ref={ref}>
+        {error && <p style={{ color: 'red' }}>{error}</p>}
+        {loading ? (
+          <span className={'jp-Spinner'} />
+        ) : (
+          <>
+            <span className={'error'}>{(error as Error).toString()}</span>
+            <ul
+              className={'available-buckets'}
+              style={{ visibility: showList ? 'visible' : 'hidden' }}
+            >
+              {searchMatchingValues.map(val => {
+                return (
+                  <li
+                    onClick={_ev => {
+                      setChosenValue(val);
+                      setShowList(false);
+                    }}
+                    key={val}
+                  >
+                    {val}
+                  </li>
+                );
+              })}
+            </ul>
+          </>
+        )}
+      </div>
+    );
+  }
+);
 
 export namespace BucketSearch {
   export interface IProps {
     data: IBucketSearch;
     showList: boolean;
+    setShowList: (show: boolean) => void;
   }
 }
```

### Comparing `tvb_ext_bucket-0.3.0/src/BucketWidget.tsx` & `tvb_ext_bucket-1.0.0/src/BucketWidget.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,51 @@
-import React, { ReactElement, useCallback, useEffect, useState } from 'react';
-import { ReactWidget } from '@jupyterlab/apputils';
+import React, {
+  ReactElement,
+  useCallback,
+  useEffect,
+  useRef,
+  useState
+} from 'react';
+import { ReactWidget, showErrorMessage } from '@jupyterlab/apputils';
 import { BucketFileBrowser } from './bucketFileBrowser';
 import { CollabSpaceEntry } from './CollabSpaceEntry';
 import { folderIcon } from '@jupyterlab/ui-components';
 import { JpSpinner } from './JpSpinner';
 import { DropZone } from './DropZone';
-import { BucketContextProvider, useBucketContext } from './BucketContext';
+import {
+  AutoCompleteOptions,
+  BucketContextProvider,
+  useBucketContext
+} from './BucketContext';
 import { BucketSearch } from './BucketSearch';
-import { useBucketSearch } from './hooks';
+import { useBucketSearch } from './hooks/useBucketSearch';
+import { Settings } from './Settings';
+import { guessBucket } from './utils/bucketUtils';
+import { useOuterClickClosable } from './hooks/useOuterClickClosable';
 
 export const BucketSpace = (): JSX.Element => {
   const [currentDir, setCurrentDir] =
     useState<BucketFileBrowser.BucketDirectory | null>(null);
   const [showSpinner, setShowSpinner] = useState<boolean>(false);
-  const [showList, setShowList] = useState<boolean>(false);
 
-  const bucketBrowser = useBucketContext().fileBrowser;
+  const {
+    fileBrowser: bucketBrowser,
+    lastBucket,
+    setLastBucket,
+    autocompleteOption
+  } = useBucketContext();
+
+  const data = useBucketSearch();
+  const { searchValue, setSearchValue, setChosenValue } = data;
+
+  const inputContainerRef = useRef<HTMLSpanElement>(null);
+  const { isComponentVisible, setIsComponentVisible, ref } =
+    useOuterClickClosable<HTMLDivElement>(false, {
+      refToIgnore: inputContainerRef
+    });
 
   /**
    * decorator for async functions to show a spinner instead of the dir structure while they resolve
    */
   const withSpinnerDecorator = useCallback((callback: () => Promise<any>) => {
     return () => {
       setShowSpinner(true);
@@ -29,64 +55,101 @@
     };
   }, []);
 
   const getBucket = useCallback(
     withSpinnerDecorator(async () => {
       const bucketHomeDir = await bucketBrowser.openBucket();
       bucketHomeDir && setCurrentDir(bucketHomeDir);
+      setLastBucket(bucketBrowser.bucket);
     }),
     [bucketBrowser]
   );
 
-  const data = useBucketSearch();
+  const navigateHome = useCallback(
+    withSpinnerDecorator(async () => {
+      if (!bucketBrowser.currentDirectory) {
+        return;
+      }
+      const home = await bucketBrowser.cd();
+      setCurrentDir(home);
+    }),
+    [bucketBrowser]
+  );
 
   useEffect(() => {
-    bucketBrowser.bucket = data.searchValue;
-  }, [data.searchValue]);
+    bucketBrowser.bucket = searchValue;
+  }, [searchValue, bucketBrowser]);
 
+  // if on mount we have a bucket name saved, open that bucket
   useEffect(() => {
-    bucketBrowser.bucket = data.chosenValue;
-  }, [data.chosenValue]);
+    if (autocompleteOption === AutoCompleteOptions.Guess) {
+      guessBucket()
+        .then(guessedBucket => setChosenValue(guessedBucket))
+        .catch(err => {
+          showErrorMessage('ERROR', err).then(() => {
+            console.warn('Did not estimate a bucket!');
+            setChosenValue('');
+          });
+        });
+    } else if (
+      autocompleteOption === AutoCompleteOptions.None ||
+      autocompleteOption === null
+    ) {
+      setChosenValue('');
+    } else {
+      setChosenValue(lastBucket ?? '');
+    }
+  }, []);
 
   return (
     <>
       <div>
         <div className={'bucket-logo'}>
           <span className={'collab-logo'} />
           <span className={'bucket-logo-text'}>Bucket</span>
+          <Settings />
         </div>
+        <span ref={inputContainerRef}>
+          <input
+            type={'text'}
+            value={searchValue}
+            aria-label={'bucket-name-input'}
+            placeholder={'bucket-name'}
+            onChange={ev => setSearchValue(ev.target.value)}
+            onFocus={_ev => setIsComponentVisible(true)} // on focus show available buckets list
+          />
+        </span>
 
-        <input
-          type={'text'}
-          value={data.searchValue}
-          aria-label={'bucket-name-input'}
-          placeholder={'bucket-name'}
-          onChange={ev => data.setSearchValue(ev.target.value)}
-          onFocus={_ev => setShowList(true)}
-          onBlur={_ev => setTimeout(() => setShowList(false), 500)}
-        />
         <button onClick={getBucket}>Connect!</button>
-        <BucketSearch data={data} showList={showList} />
+        <BucketSearch
+          data={data}
+          showList={isComponentVisible}
+          setShowList={setIsComponentVisible}
+          ref={ref}
+        />
       </div>
 
       <div className={'bucket-BreadCrumbs'}>
-        <folderIcon.react tag="span" className={'bucket-home'} />
+        <span onClick={navigateHome}>
+          <folderIcon.react tag="span" className={'bucket-home'} />
+        </span>
         {bucketBrowser.breadcrumbs.map((dir, index) => {
           return (
             <span
               key={index}
               className={'bucket-BreadCrumbs-Item'}
               aria-label={`breadcrumb-${index}`}
               onClick={withSpinnerDecorator(async () => {
                 const currentDir = await bucketBrowser.goTo(
                   bucketBrowser.breadcrumbs[index].name
                 );
                 setCurrentDir(currentDir);
               })}
             >
+              {index === 0 && '/'}
               {dir.name}/
             </span>
           );
         })}
       </div>
 
       <JpSpinner show={showSpinner} />
```

### Comparing `tvb_ext_bucket-0.3.0/src/CollabSpaceEntry.tsx` & `tvb_ext_bucket-1.0.0/src/CollabSpaceEntry.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/ContextMenu.tsx` & `tvb_ext_bucket-1.0.0/src/ContextMenu.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/ContextMenuItem.tsx` & `tvb_ext_bucket-1.0.0/src/ContextMenuItem.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/DragDownload.tsx` & `tvb_ext_bucket-1.0.0/src/DragDownload.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/DropZone.tsx` & `tvb_ext_bucket-1.0.0/src/DropZone.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/Tooltip.tsx` & `tvb_ext_bucket-1.0.0/src/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/bucketFileBrowser.ts` & `tvb_ext_bucket-1.0.0/src/bucketFileBrowser.ts`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import {
   BreadCrumbNotFoundError,
   FilePathMatchError,
   InvalidDirectoryError
 } from './exceptions';
 import { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';
 import { JpFileBrowser } from './JpFileBrowser';
-import { getExtension } from './utils';
+import { getExtension } from './utils/bucketUtils';
 
 export class BucketFileBrowser {
   private _bucket: string;
   private readonly _bucketEndpoint: string;
   private _breadcrumbs: Array<BucketFileBrowser.BucketDirectory> = [];
   private readonly _currentFiles: Map<string, BucketFileBrowser.IBrowserEntry>;
   private _homeDirectory?: BucketFileBrowser.BucketDirectory;
@@ -104,31 +104,34 @@
       await showErrorMessage('ERROR', `Could not open bucket. ${e}`);
     }
 
     return this.currentDirectory;
   }
 
   /**
-   * method to access a directory child to current directory
+   * method to access a directory child to current directory. If no dir name is provided, navigates home.
    */
-  async cd(directoryName: string): Promise<BucketFileBrowser.BucketDirectory> {
-    const dirToCd = this._currentDirectory?.directories.get(directoryName);
+  async cd(directoryName?: string): Promise<BucketFileBrowser.BucketDirectory> {
+    if ((!directoryName || directoryName === '') && this._homeDirectory) {
+      this._currentDirectory = this._homeDirectory;
+      this._currentFiles.clear();
+      this._breadcrumbs = [];
+      return this._homeDirectory;
+    }
+    const dirToCd = this._currentDirectory?.directories.get(
+      directoryName ?? ''
+    );
     if (!dirToCd) {
       throw new InvalidDirectoryError(
         `Can't cd to directory ${directoryName}! Directory doesn't seem to exist.`
       );
     }
     this._currentDirectory = dirToCd;
     this._currentFiles.clear();
     this._breadcrumbs.push(dirToCd);
-    const prefix = this.breadcrumbs.reduce(
-      (acc, curr) => acc + curr.name + '/',
-      ''
-    );
-    console.log('Going to files in: ', prefix);
 
     return dirToCd;
   }
 
   /**
    * opens a directory from breadcrumbs
    * @param directory
```

### Comparing `tvb_ext_bucket-0.3.0/src/exceptions.ts` & `tvb_ext_bucket-1.0.0/src/exceptions.ts`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/handler.ts` & `tvb_ext_bucket-1.0.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/hooks.ts` & `tvb_ext_bucket-1.0.0/src/hooks/useBucketSearch.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import React, { useEffect, useState } from 'react';
-import { requestAPI } from './handler';
+import { requestAPI } from '../handler';
 
 export const useBucketSearch = (): IBucketSearch => {
   const [loading, setLoading] = useState<boolean>(true);
   const [error, setError] = useState<string>('');
   const [availableBuckets, setAvailableBuckets] = useState<Array<string>>([]);
   const [searchValue, setSearchValue] = useState<string>('');
-  const [chosenValue, setChosenValue] = useState<string>(searchValue);
+  const [chosenValue, setChosenValue] = useState<string>('');
   const [searchMatchingValues, setSearchMatchingValues] = useState<
     Array<string>
   >([]);
+
   useEffect(() => {
     let isMounted = true;
     if (isMounted) {
       requestAPI<Array<string>>('buckets_list')
         .then(res => {
           setAvailableBuckets(res);
           setSearchMatchingValues(res);
@@ -27,20 +28,17 @@
     return () => {
       // cleanup in case component is unmounted when request is done
       isMounted = false;
     };
   }, []);
 
   useEffect(() => {
-    const filteredValues = [];
-    for (const value of availableBuckets) {
-      if (value.includes(searchValue)) {
-        filteredValues.push(value);
-      }
-    }
+    const filteredValues = availableBuckets.filter(bucketName =>
+      bucketName.includes(searchValue)
+    );
     setSearchMatchingValues(filteredValues);
   }, [searchValue]);
 
   useEffect(() => {
     setSearchValue(chosenValue);
   }, [chosenValue]);
```

### Comparing `tvb_ext_bucket-0.3.0/src/index.ts` & `tvb_ext_bucket-1.0.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/__tests__/BucketWidget.spec.tsx` & `tvb_ext_bucket-1.0.0/src/__tests__/BucketWidget.spec.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 });
 
 describe('Test BucketContext', () => {
     it('throws error when out of context', async () => {
         const WrongComponent = () => {
             const bucket = useBucketContext();
             return (
-                <div>{bucket.bucketName}</div>
+                <div>{bucket}</div>
             )
         }
         const err = await getError(() => render(<WrongComponent/>));
         expect(err).toBeInstanceOf(ContextError);
     })
 });
```

### Comparing `tvb_ext_bucket-0.3.0/src/__tests__/ContextMenu.spec.tsx` & `tvb_ext_bucket-1.0.0/src/__tests__/ContextMenu.spec.tsx`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/__tests__/bucketFileBrowser.spec.ts` & `tvb_ext_bucket-1.0.0/src/__tests__/bucketFileBrowser.spec.ts`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/src/__tests__/handler.spec.ts` & `tvb_ext_bucket-1.0.0/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/style/Collaboratory_EBRAINS.svg` & `tvb_ext_bucket-1.0.0/style/Collaboratory_EBRAINS.svg`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/style/Collaboratory_bucket_simple.png` & `tvb_ext_bucket-1.0.0/style/Collaboratory_bucket_simple.png`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/style/base.css` & `tvb_ext_bucket-1.0.0/style/base.css`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,24 @@
   height: 1em;
   width: 1em;
   border-radius: 50%;
   margin: 0 0.5em;
   animation: spin 0.5s infinite linear;
 }
 
+.bucket-home {
+  cursor: pointer;
+  padding: 0 3px;
+  display: inline-block;
+}
+
+.bucket-home:hover {
+  background-color: var(--jp-layout-color2);
+}
+
 .align-flex-horizontal {
   display: flex;
   flex-direction: row;
   align-items: flex-start;
   justify-content: center;
 }
 
@@ -292,7 +302,37 @@
   width: 100%;
 }
 
 .bucket-container ul.available-buckets > li:hover {
   background-color: var(--jp-layout-color2);
   cursor: pointer;
 }
+
+.bucket-Settings {
+  position: absolute;
+  z-index: 9999;
+  background-color: var(--jp-layout-color1);
+  box-shadow: var(--jp-elevation-z6);
+  top: 2em;
+  right: 1em;
+  left: 1em;
+  display: flex;
+  flex-direction: column;
+  padding: 0.5em;
+}
+
+.bucket-Settings h4 {
+  margin: 0;
+  font-weight: 600;
+}
+
+.bucket-Settings-toggle {
+  display: inline-block;
+  margin-left: auto;
+  margin-right: 1em;
+  cursor: pointer;
+}
+
+.bucket-Settings-container {
+  margin-right: 0;
+  margin-left: auto;
+}
```

### Comparing `tvb_ext_bucket-0.3.0/style/ebrains_logo.png` & `tvb_ext_bucket-1.0.0/style/ebrains_logo.png`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/style/hdd-o-4.svg` & `tvb_ext_bucket-1.0.0/style/hdd-o-4.svg`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/__init__.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/ebrains_drive_wrapper.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/ebrains_drive_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from tvb_ext_bucket.logger.builder import get_logger
 from tvb_ext_bucket.exceptions import CollabTokenError, CollabAccessError, DataproxyFileNotFound
 import os
 
 from tvb_ext_bucket.bucket_api.bucket_api import BucketApiClient
 from tvb_ext_bucket.bucket_api.bucket import Bucket
-from tvb_ext_bucket.bucket_api.buckets import Buckets, BucketDTO
+import pathlib
 
 LOGGER = get_logger(__name__)
 
 TOKEN_ENV_VAR = 'CLB_AUTH'
 
 
 def get_collab_token():
@@ -94,15 +94,16 @@
         :return:
         """
         bucket = self._get_bucket(bucket_name)
         # remove the prefix from the list of files
         files_list = [f.name for f in bucket.ls()]
         return files_list
 
-    def get_client(self):
+    @staticmethod
+    def get_client():
         # type: () -> BucketApiClient
         """
         Get an instance of the BucketApiClient
         Returns
         -------
 
         """
@@ -206,7 +207,38 @@
         resp.raise_for_status()
         dataproxy_file.delete()
         return {'name': new_name, 'path': dir_path + '/' + new_name}
 
     def list_buckets(self):
         buckets = self.client.buckets.list_buckets()
         return [b.name for b in buckets]
+
+    def guess_bucket(self):
+        # type: () -> str
+        """
+        Attempt to guess a bucket name by looking for repos named as the mounted drive
+        """
+        LOGGER.info('Trying to guess bucket...')
+        token = self.client.token
+        collab_name = pathlib.Path.cwd().parts[4]  # educated guess, safer than lab env vars
+        LOGGER.info(f'educated guess: {collab_name}')
+        LOGGER.info('getting drive client...')
+        drive_client = ebrains_drive.connect(token=token)
+        LOGGER.info(f'try to get repo by name {collab_name}...')
+        repos = drive_client.repos.get_repos_by_name(collab_name)
+        assert (len(repos) == 1)
+        LOGGER.info(f'found {len(repos)} repos')
+        LOGGER.info(f'attempting to find collab of repo {repos[0].id}')
+        response = requests.get(
+            "https://wiki.ebrains.eu/rest/v1/collabs",
+            params={
+                "driveId": repos[0].id,
+            },
+            headers={'Authorization': f'Bearer {token}'}
+        )
+        if not response.ok:
+            LOGGER.error(f'Could not complete request: {response.reason}')
+            raise ConnectionError(f'Failed request: {response.reason}')
+
+        bucket_name = response.json()['name']  # same as collab url name
+        LOGGER.info(f'Estimated bucket to be {bucket_name}')
+        return bucket_name
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/exceptions.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/handlers.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,31 +191,52 @@
         if not response['success']:
             self.set_status(400)
             self.finish(json.dumps(response))
         else:
             self.finish(json.dumps(response))
 
 
+class GuessBucketHandler(APIHandler):
+    def get(self):
+        response = {
+            'success': False,
+            'bucket': '',
+            'message': ''
+        }
+        try:
+            wrapper = BucketWrapper()
+            response['bucket'] = wrapper.guess_bucket()
+            response['success'] = True
+        except AssertionError:
+            response['message'] = 'Could not identify a repo. ' \
+                                  'This installation of tvb-ext-bucket might not be in an ebrains environment!'
+        except Exception as e:
+            response['message'] = str(e)
+        self.finish(json.dumps(response))
+
+
 def setup_handlers(web_app):
     host_pattern = ".*$"
 
     base_url = web_app.settings["base_url"]
     buckets_list_pattern = url_path_join(base_url, "tvb_ext_bucket", "buckets_list")
     bucket_pattern = url_path_join(base_url, "tvb_ext_bucket", "buckets")
     download_pattern = url_path_join(base_url, "tvb_ext_bucket", "download")
     download_ulr_pattern = url_path_join(base_url, "tvb_ext_bucket", "download_url")
     upload_pattern = url_path_join(base_url, "tvb_ext_bucket", "upload")
     local_upload_pattern = url_path_join(base_url, "tvb_ext_bucket", "local_upload")
     objects_handler = url_path_join(base_url, "tvb_ext_bucket", r"objects/(.*)/(.*)")
     rename_handler_pattern = url_path_join(base_url, "tvb_ext_bucket", "rename")
+    guess_bucket_pattern = url_path_join(base_url, "tvb_ext_bucket", "guess_bucket")
 
     handlers = [
         (buckets_list_pattern, BucketsHandler),
         (bucket_pattern, BucketHandler),
         (download_pattern, DownloadHandler),
         (download_ulr_pattern, DownloadUrlHandler),
         (upload_pattern, UploadHandler),
         (local_upload_pattern, LocalUploadHandler),
         (objects_handler, ObjectsHandler),
-        (rename_handler_pattern, RenameHandler)
+        (rename_handler_pattern, RenameHandler),
+        (guess_bucket_pattern, GuessBucketHandler)
     ]
     web_app.add_handlers(host_pattern, handlers)
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/bucket.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/bucket.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/bucket_api.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/bucket_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
         super().__init__(username, password, token, env)
 
         self.server = "https://data-proxy.ebrains.eu/api"
 
         self.buckets = Buckets(self)
 
+    @property
+    def token(self):
+        return self._token
+
     @on_401_raise_unauthorized(
         "Failed. Note: BucketApiClient.create_new needs to have clb.drive:write as a part of scope.")
     def create_new(self, bucket_name: str, title=None, description="Created by ebrains_drive"):
         # attempt to create new collab
         self.send_request("POST", "https://wiki.ebrains.eu/rest/v1/collabs", json={
             "name": bucket_name,
             "title": title or bucket_name,
@@ -42,15 +46,15 @@
 
     @on_401_raise_unauthorized(
         "Failed. Note: BucketApiClient.create_new needs to have clb.drive:write as a part of scope.")
     def delete_bucket(self, bucket_name: str):
         self.send_request("DELETE", f"/v1/buckets/{bucket_name}")
 
     def send_request(self, method: str, url: str, *args, **kwargs):
-        hdr, info, sig = self._token.split('.')
+        _, info, _ = self._token.split('.')
         info_json = base64.b64decode(info + '==').decode('utf-8')
 
         # https://www.rfc-editor.org/rfc/rfc7519#section-2
         exp_utc_seconds = json.loads(info_json).get('exp')
         now_tc_seconds = time.time()
 
         if now_tc_seconds > exp_utc_seconds:
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/buckets.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/buckets.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/bucket_api/dataproxy_file.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/bucket_api/dataproxy_file.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/package.json` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c935a8c2bed6559fef34.js'}}",*

 * * "'version'": "'1.0.0'"}*

```diff
@@ -54,15 +54,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b2ee1fefe23289008a39.js",
+            "load": "static/remoteEntry.c935a8c2bed6559fef34.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "tvb-ext-bucket"
                 },
@@ -118,9 +118,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "1.0.0"
 }
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/529.3f5fcb349df6ed19fa54.js` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/522.88137ffbe3671c70bd7e.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,75 +1,75 @@
 "use strict";
 (self.webpackChunktvb_ext_bucket = self.webpackChunktvb_ext_bucket || []).push([
-    [529], {
-        529: (e, t, a) => {
-            a.r(t), a.d(t, {
-                default: () => O
+    [522], {
+        522: (e, t, n) => {
+            n.r(t), n.d(t, {
+                default: () => W
             });
-            var n = a(866),
-                r = a(535),
-                o = a(510),
-                s = a(468),
-                l = a(271),
-                i = a.n(l),
-                c = a(591);
+            var a = n(638),
+                r = n(122),
+                o = n(303),
+                s = n(543),
+                l = n(271),
+                c = n.n(l),
+                i = n(745);
             const u = ({
                 label: e,
                 action: t,
-                icon: a,
-                onContextFinish: n
+                icon: n,
+                onContextFinish: a
             }) => {
                 const [r, o] = (0, l.useState)(!1), s = (0, l.useCallback)((async () => {
-                    o(!0), await t(), n && n(), o(!1)
+                    o(!0), await t(), a && a(), o(!1)
                 }), []);
-                return i().createElement("li", {
+                return c().createElement("li", {
                     onClick: s,
                     className: "bucket-ContextMenu-item"
-                }, a && i().createElement(a.react, null), i().createElement("p", {
+                }, n && c().createElement(n.react, null), c().createElement("p", {
                     style: {
                         paddingLeft: "0.5em"
                     }
-                }, e), i().createElement("span", {
+                }, e), c().createElement("span", {
                     className: "bucket-Spinner",
                     style: {
                         display: r ? "inline-block" : "none"
                     }
                 }))
             };
-            var d = a(886),
-                m = a(258);
+            var d = n(344),
+                m = n(139);
             async function h(e = "", t = {}) {
-                const a = m.ServerConnection.makeSettings(),
-                    n = d.URLExt.join(a.baseUrl, "tvb_ext_bucket", e);
+                const n = m.ServerConnection.makeSettings(),
+                    a = d.URLExt.join(n.baseUrl, "tvb_ext_bucket", e);
                 let r;
                 try {
-                    r = await m.ServerConnection.makeRequest(n, t, a)
+                    r = await m.ServerConnection.makeRequest(a, t, n)
                 } catch (e) {
                     throw new m.ServerConnection.NetworkError(e)
                 }
                 let o = await r.text();
                 if (o.length > 0) try {
                     o = JSON.parse(o)
                 } catch (e) {
                     console.log("Not a JSON response body.", r)
                 }
                 if (!r.ok) throw new m.ServerConnection.ResponseError(r, o.message || o);
                 return o
             }
             class b extends Error {}
             class p extends Error {}
-            class v extends Error {}
             class f extends Error {}
+            class v extends Error {}
             class g extends Error {}
             const w = {
                     current: null
                 },
                 k = e => {
                     let t = "";
-                    for (let a = e.length - 1; a > -1 && (t = e[a] + t, "." !== e[a]); a--);
+                    for (let n = e.length - 1; n > -1 && (t = e[n] + t, "." !== e[n]); n--);
                     return t.startsWith(".") ? t : ""
                 };
             class E {
                 constructor(e) {
                     this._breadcrumbs = [], this._bucket = e.bucket, this._bucketEndpoint = e.bucketEndPoint, this._currentFiles = new Map
                 }
                 _buildBrowser(e) {
@@ -107,47 +107,55 @@
                     } catch (e) {
                         await (0, o.showErrorMessage)("ERROR", `Could not open bucket. ${e}`)
                     }
                     return this.currentDirectory
                 }
                 async cd(e) {
                     var t;
-                    const a = null === (t = this._currentDirectory) || void 0 === t ? void 0 : t.directories.get(e);
-                    if (!a) throw new f(`Can't cd to directory ${e}! Directory doesn't seem to exist.`);
-                    this._currentDirectory = a, this._currentFiles.clear(), this._breadcrumbs.push(a);
-                    const n = this.breadcrumbs.reduce(((e, t) => e + t.name + "/"), "");
-                    return console.log("Going to files in: ", n), a
+                    if ((!e || "" === e) && this._homeDirectory) return this._currentDirectory = this._homeDirectory, this._currentFiles.clear(), this._breadcrumbs = [], this._homeDirectory;
+                    const n = null === (t = this._currentDirectory) || void 0 === t ? void 0 : t.directories.get(null != e ? e : "");
+                    if (!n) throw new v(`Can't cd to directory ${e}! Directory doesn't seem to exist.`);
+                    return this._currentDirectory = n, this._currentFiles.clear(), this._breadcrumbs.push(n), n
                 }
                 async goTo(e) {
                     const t = [...this._breadcrumbs];
-                    let a = t.pop();
-                    for (; void 0 !== a && a.name !== e;) a = t.pop();
-                    if (void 0 === a) throw new b(`Could not find breadcrumb ${e}`);
-                    return t.push(a), this._breadcrumbs = t, this._currentDirectory = a, a
+                    let n = t.pop();
+                    for (; void 0 !== n && n.name !== e;) n = t.pop();
+                    if (void 0 === n) throw new b(`Could not find breadcrumb ${e}`);
+                    return t.push(n), this._breadcrumbs = t, this._currentDirectory = n, n
                 }
+            }
+
+            function y(e, t) {
+                const n = (0, l.useMemo)((() => `tvb-ext-bucket:${t}`), []),
+                    [a, r] = (0, l.useState)(JSON.parse(localStorage.getItem(n)));
+                return (0, l.useEffect)((() => {
+                    const e = JSON.stringify(a);
+                    localStorage.setItem(n, e)
+                }), [a]), [a, r, n]
             }! function(e) {
                 class t {
-                    constructor(e, t, a, n) {
-                        this.directories = new Map, this.files = new Map, this.isFile = !1, this.name = e, this.bucket = a, this.absolutePath = n || "", this._buildContents(t)
+                    constructor(e, t, n, a) {
+                        this.directories = new Map, this.files = new Map, this.isFile = !1, this.name = e, this.bucket = n, this.absolutePath = a || "", this._buildContents(t)
                     }
                     _buildContents(e) {
-                        const n = new Map;
+                        const a = new Map;
                         for (const t of e)
                             if (t.includes("/")) {
                                 const e = t.slice(0, t.indexOf("/")),
-                                    a = t.slice(t.indexOf("/") + 1),
-                                    r = n.get(e);
-                                r ? r.push(a) : n.set(e, [a])
+                                    n = t.slice(t.indexOf("/") + 1),
+                                    r = a.get(e);
+                                r ? r.push(n) : a.set(e, [n])
                             } else {
-                                const e = new a(t, this.absolutePath ? `${this.absolutePath}/${t}` : t, this.bucket);
+                                const e = new n(t, this.absolutePath ? `${this.absolutePath}/${t}` : t, this.bucket);
                                 this.files.set(e.name, e)
-                            } n.forEach(((e, a) => {
-                            const n = this.absolutePath ? `${this.absolutePath}/${a}` : a,
-                                r = new t(a, e, this.bucket, n);
-                            this.directories.set(a, r)
+                            } a.forEach(((e, n) => {
+                            const a = this.absolutePath ? `${this.absolutePath}/${n}` : n,
+                                r = new t(n, e, this.bucket, a);
+                            this.directories.set(n, r)
                         }))
                     }
                     get filesCount() {
                         return this.files.size
                     }
                     get directoriesCount() {
                         return this.directories.size
@@ -156,16 +164,16 @@
                         const e = [];
                         for (const t of this.directories.values()) e.push(t);
                         for (const t of this.files.values()) e.push(t);
                         return e
                     }
                     async upload(e, t) {
                         if (!await this._confirmOverride(t)) return;
-                        const a = h(`upload?source_file=${e}&bucket=${this.bucket}&destination=${this.absolutePath}&filename=${t}`);
-                        console.log("result: ", a)
+                        const n = h(`upload?source_file=${e}&bucket=${this.bucket}&destination=${this.absolutePath}&filename=${t}`);
+                        console.log("result: ", n)
                     }
                     async getUploadUrl(e) {
                         if (!await this._confirmOverride(e)) return "#";
                         const t = await h(`local_upload?to_bucket=${this.bucket}&with_name=${e}&to_path=${encodeURIComponent(this.absolutePath)}`);
                         return t.success || await (0, o.showErrorMessage)("Error", "Could not get an upload url for this file!"), t.url
                     }
                     async _confirmOverride(e) {
@@ -177,34 +185,34 @@
                             }), o.Dialog.okButton({
                                 label: "Continue"
                             })]
                         })).button.accept
                     }
                 }
                 e.BucketDirectory = t;
-                class a {
-                    constructor(e, t, a) {
-                        this.isFile = !0, this._name = e, this.bucket = a, this._absolutePath = t, this._validate()
+                class n {
+                    constructor(e, t, n) {
+                        this.isFile = !0, this._name = e, this.bucket = n, this._absolutePath = t, this._validate()
                     }
                     get name() {
                         return this._name
                     }
                     get absolutePath() {
                         return this._absolutePath
                     }
                     async download() {
                         var e;
                         try {
                             const t = this.absolutePath;
-                            let a = null === (e = w.current) || void 0 === e ? void 0 : e.model.path;
-                            a || (a = ""), console.log("downloading to: ", a);
-                            const n = await h(`download?file=${encodeURIComponent(t)}&download_destination=${encodeURIComponent(a)}&bucket=${this.bucket}`);
+                            let n = null === (e = w.current) || void 0 === e ? void 0 : e.model.path;
+                            n || (n = ""), console.log("downloading to: ", n);
+                            const a = await h(`download?file=${encodeURIComponent(t)}&download_destination=${encodeURIComponent(n)}&bucket=${this.bucket}`);
                             await (0, o.showDialog)({
-                                title: n.success ? "Success!" : "Failed!",
-                                body: `File ${this.name} was ${n.success?"":"not"} downloaded! \n ${n.message?n.message:""}`,
+                                title: a.success ? "Success!" : "Failed!",
+                                body: `File ${this.name} was ${a.success?"":"not"} downloaded! \n ${a.message?a.message:""}`,
                                 buttons: [o.Dialog.okButton({
                                     label: "OK"
                                 })]
                             })
                         } catch (e) {
                             await (0, o.showErrorMessage)("Something went wrong!", e)
                         }
@@ -241,290 +249,296 @@
                         if (!t.success) throw new Error(`Could not rename file ${this.name} to ${e}!`);
                         this._name = t.newData.name, this._absolutePath = t.newData.path
                     }
                     _validate() {
                         if (!this.absolutePath.endsWith(this.name)) throw new p(`Provided absolute path (${this.absolutePath}) does not lead to the provided file name (${this.name})!`)
                     }
                 }
-                e.BucketFile = a
+                e.BucketFile = n
             }(E || (E = {}));
-            const y = (0, l.createContext)(void 0),
-                C = ({
+            const C = (0, l.createContext)(void 0),
+                D = ({
                     children: e
                 }) => {
-                    const [t, a] = (0, l.useState)(""), n = {
-                        fileBrowser: new E({
+                    const [t, n] = y(0, "last-accessed-bucket"), [a, r] = y(x.None, "autocomplete-option"), o = {
+                        fileBrowser: (0, l.useMemo)((() => new E({
                             bucketEndPoint: "buckets",
-                            bucket: t
-                        }),
-                        bucketName: t,
-                        setBucketName: a
+                            bucket: ""
+                        })), []),
+                        lastBucket: t,
+                        setLastBucket: n,
+                        autocompleteOption: a,
+                        setAutocompleteOption: r
                     };
-                    return i().createElement(y.Provider, {
-                        value: n
+                    return c().createElement(C.Provider, {
+                        value: o
                     }, e)
                 },
-                D = () => {
-                    const e = (0, l.useContext)(y);
+                _ = () => {
+                    const e = (0, l.useContext)(C);
                     if (void 0 === e) throw new g("useBucketContext must be used within a BucketContextProvider");
                     return e
-                },
-                _ = ({
+                };
+            var x;
+            ! function(e) {
+                e.None = "no-preference", e.LastAccessed = "save-last", e.Guess = "guess"
+            }(x || (x = {}));
+            const S = ({
                     name: e,
                     onContextFinish: t,
-                    renameAction: a,
-                    children: n
+                    renameAction: n,
+                    children: a
                 }) => {
-                    const [r, s] = (0, l.useState)(!1), d = D().fileBrowser;
+                    const [r, s] = (0, l.useState)(!1), d = _().fileBrowser;
                     (0, l.useEffect)((() => {
                         const e = () => s(!1);
                         return document.addEventListener("click", e), () => document.removeEventListener("click", e)
                     }), []);
                     const m = (0, l.useCallback)((e => {
                             e.preventDefault(), s((e => !e))
                         }), [s]),
                         h = (0, l.useCallback)((async () => {
-                            var t, a;
-                            const n = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
-                            n ? await n.download() : await (0, o.showErrorMessage)("Download failed!", `Can't find file ${e} in directory ${null===(a=d.currentDirectory)||void 0===a?void 0:a.name}`)
+                            var t, n;
+                            const a = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
+                            a ? await a.download() : await (0, o.showErrorMessage)("Download failed!", `Can't find file ${e} in directory ${null===(n=d.currentDirectory)||void 0===n?void 0:n.name}`)
                         }), [e]),
                         b = (0, l.useCallback)((async () => {
-                            var t, a;
-                            const n = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
-                            if (n) {
-                                const t = await n.getDownloadUrl(),
-                                    a = document.createElement("a");
-                                a.href = t, a.download = e, document.body.appendChild(a), a.click(), document.body.removeChild(a)
-                            } else await (0, o.showErrorMessage)("Download failed!", `Can't find file ${e} in directory ${null===(a=d.currentDirectory)||void 0===a?void 0:a.name}. Please refresh and try again!`)
+                            var t, n;
+                            const a = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
+                            if (a) {
+                                const t = await a.getDownloadUrl(),
+                                    n = document.createElement("a");
+                                n.href = t, n.download = e, document.body.appendChild(n), n.click(), document.body.removeChild(n)
+                            } else await (0, o.showErrorMessage)("Download failed!", `Can't find file ${e} in directory ${null===(n=d.currentDirectory)||void 0===n?void 0:n.name}. Please refresh and try again!`)
                         }), [e]),
                         p = (0, l.useCallback)((async () => {
-                            var t, a;
-                            const n = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
-                            if (n) {
-                                const t = await n.delete();
+                            var t, n;
+                            const a = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
+                            if (a) {
+                                const t = await a.delete();
                                 if (!t) return;
                                 await (0, o.showDialog)({
                                     title: t.success ? "Success!" : "Failed!",
                                     body: `File ${e} was ${t.success?"":"not"} deleted! \n ${t.message?t.message:""}`,
                                     buttons: [o.Dialog.okButton({
                                         label: "OK"
                                     })]
                                 })
-                            } else await (0, o.showErrorMessage)("Deletion failed!", `Can't find file ${e} in directory ${null===(a=d.currentDirectory)||void 0===a?void 0:a.name}. Please refresh and try again!`)
+                            } else await (0, o.showErrorMessage)("Deletion failed!", `Can't find file ${e} in directory ${null===(n=d.currentDirectory)||void 0===n?void 0:n.name}. Please refresh and try again!`)
                         }), [e]),
-                        v = (0, l.useCallback)((async () => {
+                        f = (0, l.useCallback)((async () => {
                             var t;
-                            let a = "";
+                            let n = "";
                             try {
-                                const n = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
-                                if (!n) return void await (0, o.showErrorMessage)("ERROR", `Could not get details on file ${e}. Please refresh and try again!`);
-                                a = await n.getDownloadUrl(), await (0, o.showDialog)({
+                                const a = null === (t = d.currentDirectory) || void 0 === t ? void 0 : t.files.get(e);
+                                if (!a) return void await (0, o.showErrorMessage)("ERROR", `Could not get details on file ${e}. Please refresh and try again!`);
+                                n = await a.getDownloadUrl(), await (0, o.showDialog)({
                                     title: "Your share URL:",
-                                    body: i().createElement(i().Fragment, null, i().createElement("a", {
-                                        href: a,
+                                    body: c().createElement(c().Fragment, null, c().createElement("a", {
+                                        href: n,
                                         className: "bucket-ShareLink"
-                                    }, a), i().createElement("p", null, "Copy and paste this url in a browser to download the file!"), i().createElement("p", {
+                                    }, n), c().createElement("p", null, "Copy and paste this url in a browser to download the file!"), c().createElement("p", {
                                         style: {
                                             color: "red"
                                         }
                                     }, "* If this bucket is private this link will expire very soon.")),
                                     buttons: [o.Dialog.okButton({
                                         label: "Close"
                                     })]
                                 })
                             } catch (e) {
                                 await (0, o.showErrorMessage)("ERROR", e)
                             }
                         }), [e]);
-                    return i().createElement("div", {
+                    return c().createElement("div", {
                         onContextMenu: m,
                         className: "bucket-ContextMenu-container"
-                    }, n, i().createElement("div", {
+                    }, a, c().createElement("div", {
                         className: "bucket-ContextMenu",
                         "aria-label": "context-menu",
                         onClick: e => e.stopPropagation(),
                         style: {
                             display: r ? "block" : "none"
                         }
-                    }, i().createElement("ul", null, i().createElement(u, {
+                    }, c().createElement("ul", null, c().createElement(u, {
                         label: "Download",
                         action: h,
-                        icon: c.downloadIcon
-                    }), i().createElement(u, {
+                        icon: i.downloadIcon
+                    }), c().createElement(u, {
                         label: "Local Download",
                         action: b,
-                        icon: c.downloadIcon
-                    }), i().createElement(u, {
+                        icon: i.downloadIcon
+                    }), c().createElement(u, {
                         label: "Delete",
                         action: p,
-                        icon: c.closeIcon,
+                        icon: i.closeIcon,
                         onContextFinish: t
-                    }), i().createElement(u, {
+                    }), c().createElement(u, {
                         label: "Rename",
                         action: () => {
-                            a(), s(!1)
+                            n(), s(!1)
                         },
-                        icon: c.editIcon
-                    }), i().createElement(u, {
+                        icon: i.editIcon
+                    }), c().createElement(u, {
                         label: "Share download url",
-                        action: v,
-                        icon: c.linkIcon
+                        action: f,
+                        icon: i.linkIcon
                     }))))
                 },
-                x = () => i().createElement("span", {
+                $ = () => c().createElement("span", {
                     className: "bucket-DownloadAnimation"
-                }, i().createElement("i", {
+                }, c().createElement("i", {
                     className: "fa fa-arrow-down"
                 })),
-                $ = () => i().createElement("span", {
+                N = () => c().createElement("span", {
                     className: "bucket-UploadAnimation"
-                }, i().createElement(c.fileUploadIcon.react, null)),
-                S = ({
+                }, c().createElement(i.fileUploadIcon.react, null)),
+                L = ({
                     children: e,
                     file: t
                 }) => {
-                    const [a, n] = (0, l.useState)(!1), r = (0, l.useCallback)((e => e.clientX > 20 && e.clientX < 280), []), o = (0, l.useCallback)((async e => {
-                        e.preventDefault(), e.stopPropagation(), r(e) && (n(!0), await t.download(), n(!1))
+                    const [n, a] = (0, l.useState)(!1), r = (0, l.useCallback)((e => e.clientX > 20 && e.clientX < 280), []), o = (0, l.useCallback)((async e => {
+                        e.preventDefault(), e.stopPropagation(), r(e) && (a(!0), await t.download(), a(!1))
                     }), []);
-                    return i().createElement("div", {
-                        draggable: !a,
+                    return c().createElement("div", {
+                        draggable: !n,
                         onDragEnd: o,
                         className: "align-flex-horizontal"
-                    }, e, a && i().createElement(x, null))
+                    }, e, n && c().createElement($, null))
                 };
 
-            function N({
+            function R({
                 tag: e,
                 metadata: t,
-                onClick: a,
-                onContextFinish: n
+                onClick: n,
+                onContextFinish: a
             }) {
-                const [r, s] = (0, l.useState)(!1), u = D().fileBrowser, d = (0, l.useRef)(null), [m, h, b] = (({
+                const [r, s] = (0, l.useState)(!1), u = _().fileBrowser, d = (0, l.useRef)(null), [m, h, b] = (({
                     hasLoader: e,
                     displayInfo: t
                 }) => {
-                    const [a, n] = (0, l.useState)(!1), [r, o] = (0, l.useState)(t || ""), s = {
-                        display: a ? "flex" : "none"
+                    const [n, a] = (0, l.useState)(!1), [r, o] = (0, l.useState)(t || ""), s = {
+                        display: n ? "flex" : "none"
                     };
-                    return [() => i().createElement("div", {
+                    return [() => c().createElement("div", {
                         style: s,
                         className: "bucket-Tooltip"
-                    }, e && i().createElement("span", {
+                    }, e && c().createElement("span", {
                         className: "bucket-Spinner"
-                    }), i().createElement("p", null, r)), o, n]
+                    }), c().createElement("p", null, r)), o, a]
                 })({
                     hasLoader: !0
                 });
                 (0, l.useEffect)((() => {
                     var e;
                     const t = async e => {
-                        var a;
-                        e.stopPropagation(), "Enter" === e.key && (e.preventDefault(), b(!0), h("Renaming file..."), await p(), b(!1), null === (a = d.current) || void 0 === a || a.removeEventListener("keypress", t), s(!1))
+                        var n;
+                        e.stopPropagation(), "Enter" === e.key && (e.preventDefault(), b(!0), h("Renaming file..."), await p(), b(!1), null === (n = d.current) || void 0 === n || n.removeEventListener("keypress", t), s(!1))
                     };
                     return r && (null === (e = d.current) || void 0 === e || e.addEventListener("keypress", t)), () => {
                         var e;
                         return null === (e = d.current) || void 0 === e ? void 0 : e.removeEventListener("keypress", t)
                     }
                 }), [r]);
                 const p = async () => {
                     var e;
-                    const a = null === (e = u.currentDirectory) || void 0 === e ? void 0 : e.files.get(t.name);
-                    if (a) try {
+                    const n = null === (e = u.currentDirectory) || void 0 === e ? void 0 : e.files.get(t.name);
+                    if (n) try {
                         const e = d.current ? d.current.value : t.name;
-                        await a.rename(e), await n()
+                        await n.rename(e), await a()
                     } catch (e) {
                         await (0, o.showErrorMessage)("Failed to rename", e)
                     } else {
                         const e = `File ${t.name} could not be found!`;
                         (0, o.showErrorMessage)("ERROR", e).then((() => console.error(e)))
                     }
                 };
-                return i().createElement(P.Wrapper, {
+                return c().createElement(I.Wrapper, {
                     tag: e
-                }, t.isFile ? i().createElement(c.fileIcon.react, {
+                }, t.isFile ? c().createElement(i.fileIcon.react, {
                     tag: "span",
                     right: "7px",
                     className: "jp-DirListing-itemIcon"
-                }) : i().createElement(c.folderIcon.react, {
+                }) : c().createElement(i.folderIcon.react, {
                     tag: "span",
                     right: "7px",
                     className: "jp-DirListing-itemIcon"
-                }), t.isFile ? i().createElement(_, {
+                }), t.isFile ? c().createElement(S, {
                     name: t.name,
-                    onContextFinish: n,
+                    onContextFinish: a,
                     renameAction: () => s(!0)
-                }, i().createElement(m, null), i().createElement(S, {
+                }, c().createElement(m, null), c().createElement(L, {
                     file: t
-                }, r ? i().createElement("input", {
+                }, r ? c().createElement("input", {
                     "aria-label": "rename-input",
                     defaultValue: t.name,
                     ref: d
-                }) : i().createElement("p", {
-                    onClick: a
-                }, t.name))) : i().createElement("p", {
-                    onClick: a,
+                }) : c().createElement("p", {
+                    onClick: n
+                }, t.name))) : c().createElement("p", {
+                    onClick: n,
                     style: {
                         cursor: "pointer"
                     }
                 }, t.name))
             }
-            var P;
+            var I;
             ! function(e) {
                 e.Wrapper = ({
                     tag: e,
                     children: t
-                }) => i().createElement(i().Fragment, null, "li" === e ? i().createElement("li", {
+                }) => c().createElement(c().Fragment, null, "li" === e ? c().createElement("li", {
                     className: "bucket-BrowserListItem"
-                }, t) : i().createElement("div", null, t))
-            }(P || (P = {}));
-            const R = e => !1 === e.show ? i().createElement(i().Fragment, null) : i().createElement("div", {
+                }, t) : c().createElement("div", null, t))
+            }(I || (I = {}));
+            const P = e => !1 === e.show ? c().createElement(c().Fragment, null) : c().createElement("div", {
                 className: "jp-SpinnerContent"
             });
-            var L = a(694),
-                F = a(526);
-            const B = ({
+            var F = n(694),
+                B = n(526);
+            const M = ({
                     show: e,
                     finishAction: t
                 }) => {
-                    const [a, n] = (0, l.useState)("default"), [r, s] = (0, l.useState)(!1), c = (0, l.useRef)(r);
+                    const [n, a] = (0, l.useState)("default"), [r, s] = (0, l.useState)(!1), i = (0, l.useRef)(r);
                     (0, l.useEffect)((() => {
-                        c.current = r
+                        i.current = r
                     }), [r]);
                     const u = (0, l.useRef)(null),
-                        d = D().fileBrowser,
+                        d = _().fileBrowser,
                         m = (0, l.useMemo)((() => ({
                             title: "Not allowed!",
                             error: "Please wait for the previous upload to finish!"
                         })), []),
                         h = (0, l.useCallback)((e => {
                             var t;
                             if (2 === e.button) return;
-                            const a = e.target,
-                                n = null === (t = w.current) || void 0 === t ? void 0 : t.selectedItems();
-                            if (null == n) return;
+                            const n = e.target,
+                                a = null === (t = w.current) || void 0 === t ? void 0 : t.selectedItems();
+                            if (null == a) return;
                             const r = [];
                             let o = !1,
-                                s = null == n ? void 0 : n.next();
-                            for (; s;) r.push(s), s.name === (null == a ? void 0 : a.innerText) && (o = !0), s = null == n ? void 0 : n.next();
+                                s = null == a ? void 0 : a.next();
+                            for (; s;) r.push(s), s.name === (null == n ? void 0 : n.innerText) && (o = !0), s = null == a ? void 0 : a.next();
                             if (!o) return void console.warn("Did not start a drag operation!");
                             const l = r[0],
-                                i = {
+                                c = {
                                     source: l,
                                     action: async () => {
                                         var e;
-                                        const [t, a] = [l.path, l.name];
-                                        await (null === (e = d.currentDirectory) || void 0 === e ? void 0 : e.upload(t, a))
+                                        const [t, n] = [l.path, l.name];
+                                        await (null === (e = d.currentDirectory) || void 0 === e ? void 0 : e.upload(t, n))
                                     }
                                 },
-                                c = new L.Drag({
-                                    mimeData: new F.MimeData,
-                                    source: i,
+                                i = new F.Drag({
+                                    mimeData: new B.MimeData,
+                                    source: c,
                                     proposedAction: "copy"
                                 });
-                            c.mimeData.setData("text/plain", JSON.stringify(l)), c.start(e.clientX, e.clientY).then((() => console.log("drag ended")))
+                            i.mimeData.setData("text/plain", JSON.stringify(l)), i.start(e.clientX, e.clientY).then((() => console.log("drag ended")))
                         }), []),
                         b = (0, l.useMemo)((() => {
                             const e = {
                                 handleEvent: t => {
                                     switch (console.log("handling: ", t.type), t.type) {
                                         case "lm-dragenter":
                                             e._dragEnter(t);
@@ -536,237 +550,346 @@
                                             e._drop(t).then((() => console.log("drop handled")));
                                             break;
                                         case "lm-dragleave":
                                             e._dragLeave(t)
                                     }
                                 },
                                 _dragEnter: e => {
-                                    e.preventDefault(), e.stopPropagation(), n("hover"), L.Drag.overrideCursor("pointer")
+                                    e.preventDefault(), e.stopPropagation(), a("hover"), F.Drag.overrideCursor("pointer")
                                 },
                                 _dragOver: e => {
-                                    e.preventDefault(), e.stopPropagation(), e.dropAction = e.proposedAction, L.Drag.overrideCursor("pointer"), n("hover")
+                                    e.preventDefault(), e.stopPropagation(), e.dropAction = e.proposedAction, F.Drag.overrideCursor("pointer"), a("hover")
                                 },
                                 _dragLeave: e => {
-                                    e.preventDefault(), e.stopPropagation(), L.Drag.overrideCursor("auto"), n("default")
+                                    e.preventDefault(), e.stopPropagation(), F.Drag.overrideCursor("auto"), a("default")
                                 },
                                 _drop: async e => {
-                                    e.preventDefault(), e.stopPropagation(), c.current ? await (0, o.showErrorMessage)(m.title, m.error) : (s(!0), e.source && e.source.action ? (await e.source.action(), await t()) : console.warn("Did not upload file to bucket since drag initiator does not provide an action!"), L.Drag.overrideCursor("auto"), n("default"), s(!1))
+                                    e.preventDefault(), e.stopPropagation(), i.current ? await (0, o.showErrorMessage)(m.title, m.error) : (s(!0), e.source && e.source.action ? (await e.source.action(), await t()) : console.warn("Did not upload file to bucket since drag initiator does not provide an action!"), F.Drag.overrideCursor("auto"), a("default"), s(!1))
                                 }
                             };
                             return e
                         }), []);
                     (0, l.useEffect)((() => {
-                        var e, t, a, n, r;
-                        null === (e = u.current) || void 0 === e || e.addEventListener("lm-dragenter", b), null === (t = u.current) || void 0 === t || t.addEventListener("lm-dragleave", b), null === (a = u.current) || void 0 === a || a.addEventListener("lm-dragover", b), null === (n = u.current) || void 0 === n || n.addEventListener("lm-drop", b);
+                        var e, t, n, a, r;
+                        null === (e = u.current) || void 0 === e || e.addEventListener("lm-dragenter", b), null === (t = u.current) || void 0 === t || t.addEventListener("lm-dragleave", b), null === (n = u.current) || void 0 === n || n.addEventListener("lm-dragover", b), null === (a = u.current) || void 0 === a || a.addEventListener("lm-drop", b);
                         const o = null === (r = w.current) || void 0 === r ? void 0 : r.node;
                         return null == o || o.addEventListener("mousedown", h), () => {
-                            var e, t, a, n;
-                            null == o || o.removeEventListener("mousedown", h), null === (e = u.current) || void 0 === e || e.removeEventListener("lm-dragenter", b), null === (t = u.current) || void 0 === t || t.removeEventListener("lm-dragleave", b), null === (a = u.current) || void 0 === a || a.removeEventListener("lm-dragover", b), null === (n = u.current) || void 0 === n || n.removeEventListener("lm-drop", b)
+                            var e, t, n, a;
+                            null == o || o.removeEventListener("mousedown", h), null === (e = u.current) || void 0 === e || e.removeEventListener("lm-dragenter", b), null === (t = u.current) || void 0 === t || t.removeEventListener("lm-dragleave", b), null === (n = u.current) || void 0 === n || n.removeEventListener("lm-dragover", b), null === (a = u.current) || void 0 === a || a.removeEventListener("lm-drop", b)
                         }
                     }), []);
                     const p = (0, l.useCallback)((e => {
-                            e.preventDefault(), n("hover")
+                            e.preventDefault(), a("hover")
                         }), []),
-                        v = (0, l.useCallback)((e => {
-                            e.preventDefault(), n("default")
+                        f = (0, l.useCallback)((e => {
+                            e.preventDefault(), a("default")
                         }), []),
-                        f = (0, l.useCallback)((async e => {
-                            var a, r;
-                            if (e.preventDefault(), e.stopPropagation(), c.current) await (0, o.showErrorMessage)(m.title, m.error);
+                        v = (0, l.useCallback)((async e => {
+                            var n, r;
+                            if (e.preventDefault(), e.stopPropagation(), i.current) await (0, o.showErrorMessage)(m.title, m.error);
                             else {
                                 if (s(!0), e.dataTransfer.files && e.dataTransfer.files[0])
                                     if (e.dataTransfer.files.length > 1) await (0, o.showErrorMessage)("Unsupported", "Currently you can only upload a file at a time!");
                                     else try {
-                                        const n = e.dataTransfer.files[0],
-                                            s = n.name,
-                                            l = await (null === (a = d.currentDirectory) || void 0 === a ? void 0 : a.getUploadUrl(s));
+                                        const a = e.dataTransfer.files[0],
+                                            s = a.name,
+                                            l = await (null === (n = d.currentDirectory) || void 0 === n ? void 0 : n.getUploadUrl(s));
                                         if (!l) return;
                                         (await fetch(l, {
                                             method: "PUT",
-                                            body: n
+                                            body: a
                                         })).ok && (await (0, o.showDialog)({
                                             title: "Upload Success!",
                                             body: `${s} was uploaded to ${null===(r=d.currentDirectory)||void 0===r?void 0:r.absolutePath}/${s}`,
                                             buttons: [o.Dialog.okButton({
                                                 label: "OK"
                                             })]
                                         }), await t())
                                     } catch (e) {
                                         await (0, o.showErrorMessage)("Upload Failed", e)
                                     }
-                                s(!1), n("default")
+                                s(!1), a("default")
                             }
                         }), []);
-                    return i().createElement("div", {
-                        className: `bucket-DropZone ${a}`,
+                    return c().createElement("div", {
+                        className: `bucket-DropZone ${n}`,
                         ref: u,
                         onDragOver: p,
-                        onDragLeave: v,
-                        onDrop: f,
+                        onDragLeave: f,
+                        onDrop: v,
                         style: {
                             display: e ? "block" : "none"
                         }
-                    }, r ? i().createElement(i().Fragment, null, i().createElement("p", {
+                    }, r ? c().createElement(c().Fragment, null, c().createElement("p", {
                         className: "bucket-text-info"
-                    }, "Uploading files..."), i().createElement($, null)) : i().createElement("p", {
+                    }, "Uploading files..."), c().createElement(N, null)) : c().createElement("p", {
                         className: "bucket-text-info"
                     }, "Drop your files here for upload."))
                 },
-                M = ({
+                O = (0, l.forwardRef)((({
                     data: e,
-                    showList: t
-                }) => i().createElement("div", null, e.loading ? i().createElement("span", {
-                    className: "jp-Spinner"
-                }) : i().createElement(i().Fragment, null, i().createElement("span", {
-                    className: "error"
-                }, e.error.toString()), i().createElement("select", {
-                    name: "bucket",
-                    id: "bucket",
-                    autoFocus: !0,
-                    value: e.chosenValue,
-                    onChange: t => e.setChosenValue(t.target.value),
-                    style: {
-                        display: "none"
-                    }
-                }, e.searchMatchingValues.map((e => i().createElement("option", {
-                    value: e,
-                    key: e
-                }, e)))), i().createElement("ul", {
-                    className: "available-buckets",
-                    style: {
-                        visibility: t ? "visible" : "hidden"
-                    }
-                }, e.searchMatchingValues.map((t => i().createElement("li", {
-                    onClick: a => {
-                        e.setChosenValue(t)
-                    },
-                    key: t
-                }, t)))))),
-                I = () => {
-                    const [e, t] = (0, l.useState)(null), [a, n] = (0, l.useState)(!1), [r, o] = (0, l.useState)(!1), s = D().fileBrowser, u = (0, l.useCallback)((e => () => {
-                        n(!0), e().then((() => {
-                            n(!1)
-                        }))
-                    }), []), d = (0, l.useCallback)(u((async () => {
-                        const e = await s.openBucket();
-                        e && t(e)
-                    })), [s]), m = (() => {
-                        const [e, t] = (0, l.useState)(!0), [a, n] = (0, l.useState)(""), [r, o] = (0, l.useState)([]), [s, i] = (0, l.useState)(""), [c, u] = (0, l.useState)(s), [d, m] = (0, l.useState)([]);
+                    showList: t,
+                    setShowList: n
+                }, a) => {
+                    const {
+                        error: r,
+                        loading: o,
+                        searchMatchingValues: s,
+                        setChosenValue: l
+                    } = e;
+                    return c().createElement("div", {
+                        ref: a
+                    }, r && c().createElement("p", {
+                        style: {
+                            color: "red"
+                        }
+                    }, r), o ? c().createElement("span", {
+                        className: "jp-Spinner"
+                    }) : c().createElement(c().Fragment, null, c().createElement("span", {
+                        className: "error"
+                    }, r.toString()), c().createElement("ul", {
+                        className: "available-buckets",
+                        style: {
+                            visibility: t ? "visible" : "hidden"
+                        }
+                    }, s.map((e => c().createElement("li", {
+                        onClick: t => {
+                            l(e), n(!1)
+                        },
+                        key: e
+                    }, e))))))
+                }));
+
+            function U(e, t, n) {
+                const [a, r] = (0, l.useState)(e), o = (0, l.useRef)(null), s = e => {
+                    var a, s, l;
+                    const c = e.target;
+                    ! function(e) {
+                        if (!e || !("nodeType" in e)) throw new TypeError("Node expected")
+                    }(c), (null === (s = null === (a = null == t ? void 0 : t.refToIgnore) || void 0 === a ? void 0 : a.current) || void 0 === s ? void 0 : s.contains(c)) || o.current && !(null === (l = null == o ? void 0 : o.current) || void 0 === l ? void 0 : l.contains(c)) && r(void 0 !== n && n)
+                };
+                return (0, l.useEffect)((() => (document.addEventListener("click", s, !0), () => {
+                    document.removeEventListener("click", s, !0)
+                })), []), {
+                    ref: o,
+                    isComponentVisible: a,
+                    setIsComponentVisible: r
+                }
+            }
+            const A = () => {
+                    const {
+                        autocompleteOption: e,
+                        setAutocompleteOption: t
+                    } = _(), {
+                        ref: n,
+                        isComponentVisible: a,
+                        setIsComponentVisible: r
+                    } = U(!1);
+                    return c().createElement("span", {
+                        className: "bucket-Settings-container",
+                        ref: n
+                    }, c().createElement("span", {
+                        onClick: e => {
+                            r((e => !e))
+                        },
+                        className: "bucket-Settings-toggle"
+                    }, c().createElement(i.settingsIcon.react, null)), c().createElement("div", {
+                        className: "bucket-Settings",
+                        style: {
+                            display: a ? "block" : "none"
+                        }
+                    }, c().createElement("h4", null, "Settings"), c().createElement("hr", null), c().createElement("div", {
+                        className: "bucket-Preferences-container",
+                        onChange: e => {
+                            t(e.target.value)
+                        }
+                    }, c().createElement("p", {
+                        title: "After setting an option refresh the page for the setting to have effect!"
+                    }, "Auto-complete:"), c().createElement("div", null, c().createElement("input", {
+                        type: "radio",
+                        name: "bucket-preferences",
+                        id: "no-preference",
+                        value: x.None,
+                        defaultChecked: e === x.None || null === e
+                    }), c().createElement("label", {
+                        htmlFor: "no-preference",
+                        title: "On opening bucket extension, bucket name will not be completed automatically"
+                    }, "No auto-complete")), c().createElement("div", null, c().createElement("input", {
+                        type: "radio",
+                        name: "bucket-preferences",
+                        id: "save-last",
+                        value: x.LastAccessed,
+                        defaultChecked: e === x.LastAccessed
+                    }), c().createElement("label", {
+                        htmlFor: "save-last",
+                        title: "On opening the bucket extension, bucket name will be autocompleted with the name of the last accessed bucket."
+                    }, "Last accessed bucket")), c().createElement("div", null, c().createElement("input", {
+                        type: "radio",
+                        name: "bucket-preferences",
+                        id: "guess",
+                        value: x.Guess,
+                        defaultChecked: e === x.Guess
+                    }), c().createElement("label", {
+                        htmlFor: "guess",
+                        title: "On opening bucket extension, will try to autocomplete bucket name by guessing the bucket from collab."
+                    }, "Estimated bucket")))))
+                },
+                V = () => {
+                    const [e, t] = (0, l.useState)(null), [n, a] = (0, l.useState)(!1), {
+                        fileBrowser: r,
+                        lastBucket: s,
+                        setLastBucket: u,
+                        autocompleteOption: d
+                    } = _(), m = (() => {
+                        const [e, t] = (0, l.useState)(!0), [n, a] = (0, l.useState)(""), [r, o] = (0, l.useState)([]), [s, c] = (0, l.useState)(""), [i, u] = (0, l.useState)(""), [d, m] = (0, l.useState)([]);
                         return (0, l.useEffect)((() => {
                             let e = !0;
                             return e && h("buckets_list").then((e => {
                                 o(e), m(e), t(!1)
                             })).catch((e => {
-                                n(e)
+                                a(e)
                             })), () => {
                                 e = !1
                             }
                         }), []), (0, l.useEffect)((() => {
-                            const e = [];
-                            for (const t of r) t.includes(s) && e.push(t);
+                            const e = r.filter((e => e.includes(s)));
                             m(e)
                         }), [s]), (0, l.useEffect)((() => {
-                            i(c)
-                        }), [c]), {
+                            c(i)
+                        }), [i]), {
                             loading: e,
                             searchValue: s,
-                            setSearchValue: i,
+                            setSearchValue: c,
                             searchMatchingValues: d,
-                            error: a,
-                            chosenValue: c,
+                            error: n,
+                            chosenValue: i,
                             setChosenValue: u
                         }
-                    })();
+                    })(), {
+                        searchValue: b,
+                        setSearchValue: p,
+                        setChosenValue: f
+                    } = m, v = (0, l.useRef)(null), {
+                        isComponentVisible: g,
+                        setIsComponentVisible: w,
+                        ref: k
+                    } = U(!1, {
+                        refToIgnore: v
+                    }), E = (0, l.useCallback)((e => () => {
+                        a(!0), e().then((() => {
+                            a(!1)
+                        }))
+                    }), []), y = (0, l.useCallback)(E((async () => {
+                        const e = await r.openBucket();
+                        e && t(e), u(r.bucket)
+                    })), [r]), C = (0, l.useCallback)(E((async () => {
+                        if (!r.currentDirectory) return;
+                        const e = await r.cd();
+                        t(e)
+                    })), [r]);
                     return (0, l.useEffect)((() => {
-                        s.bucket = m.searchValue
-                    }), [m.searchValue]), (0, l.useEffect)((() => {
-                        s.bucket = m.chosenValue
-                    }), [m.chosenValue]), i().createElement(i().Fragment, null, i().createElement("div", null, i().createElement("div", {
+                        r.bucket = b
+                    }), [b, r]), (0, l.useEffect)((() => {
+                        d === x.Guess ? async function() {
+                            const e = await h("guess_bucket");
+                            if (!e.success) throw new Error(e.message);
+                            return e.bucket
+                        }().then((e => f(e))).catch((e => {
+                            (0, o.showErrorMessage)("ERROR", e).then((() => {
+                                console.warn("Did not estimate a bucket!"), f("")
+                            }))
+                        })): d === x.None || null === d ? f("") : f(null != s ? s : "")
+                    }), []), c().createElement(c().Fragment, null, c().createElement("div", null, c().createElement("div", {
                         className: "bucket-logo"
-                    }, i().createElement("span", {
+                    }, c().createElement("span", {
                         className: "collab-logo"
-                    }), i().createElement("span", {
+                    }), c().createElement("span", {
                         className: "bucket-logo-text"
-                    }, "Bucket")), i().createElement("input", {
+                    }, "Bucket"), c().createElement(A, null)), c().createElement("span", {
+                        ref: v
+                    }, c().createElement("input", {
                         type: "text",
-                        value: m.searchValue,
+                        value: b,
                         "aria-label": "bucket-name-input",
                         placeholder: "bucket-name",
-                        onChange: e => m.setSearchValue(e.target.value),
-                        onFocus: e => o(!0),
-                        onBlur: e => setTimeout((() => o(!1)), 500)
-                    }), i().createElement("button", {
-                        onClick: d
-                    }, "Connect!"), i().createElement(M, {
+                        onChange: e => p(e.target.value),
+                        onFocus: e => w(!0)
+                    })), c().createElement("button", {
+                        onClick: y
+                    }, "Connect!"), c().createElement(O, {
                         data: m,
-                        showList: r
-                    })), i().createElement("div", {
+                        showList: g,
+                        setShowList: w,
+                        ref: k
+                    })), c().createElement("div", {
                         className: "bucket-BreadCrumbs"
-                    }, i().createElement(c.folderIcon.react, {
+                    }, c().createElement("span", {
+                        onClick: C
+                    }, c().createElement(i.folderIcon.react, {
                         tag: "span",
                         className: "bucket-home"
-                    }), s.breadcrumbs.map(((e, a) => i().createElement("span", {
-                        key: a,
+                    })), r.breadcrumbs.map(((e, n) => c().createElement("span", {
+                        key: n,
                         className: "bucket-BreadCrumbs-Item",
-                        "aria-label": `breadcrumb-${a}`,
-                        onClick: u((async () => {
-                            const e = await s.goTo(s.breadcrumbs[a].name);
+                        "aria-label": `breadcrumb-${n}`,
+                        onClick: E((async () => {
+                            const e = await r.goTo(r.breadcrumbs[n].name);
                             t(e)
                         }))
-                    }, e.name, "/")))), i().createElement(R, {
-                        show: a
-                    }), i().createElement("ul", {
+                    }, 0 === n && "/", e.name, "/")))), c().createElement(P, {
+                        show: n
+                    }), c().createElement("ul", {
                         style: {
-                            display: a ? "none" : "block"
+                            display: n ? "none" : "block"
                         },
                         className: "scrollableY"
                     }, null == e ? void 0 : e.ls().map((e => {
-                        let a = () => {};
-                        return e.isFile || (a = u((async () => {
-                            const a = await s.cd(e.name);
-                            t(a)
-                        }))), i().createElement(N, {
+                        let n = () => {};
+                        return e.isFile || (n = E((async () => {
+                            const n = await r.cd(e.name);
+                            t(n)
+                        }))), c().createElement(R, {
                             tag: "li",
                             metadata: e,
                             key: e.name,
-                            onClick: a,
-                            onContextFinish: d
+                            onClick: n,
+                            onContextFinish: y
                         })
-                    }))), i().createElement(B, {
-                        show: !a && null !== e,
-                        finishAction: d
+                    }))), c().createElement(M, {
+                        show: !n && null !== e,
+                        finishAction: y
                     }))
                 };
-            class U extends o.ReactWidget {
+            class T extends o.ReactWidget {
                 constructor() {
                     super(), this.addClass("tvb-bucketWidget")
                 }
                 render() {
-                    return i().createElement("div", {
+                    return c().createElement("div", {
                         className: "bucket-container"
-                    }, i().createElement(C, null, i().createElement(I, null)))
+                    }, c().createElement(D, null, c().createElement(V, null)))
                 }
             }
-            const O = {
+            const W = {
                 id: "tvb-ext-bucket:plugin",
                 autoStart: !0,
-                requires: [o.ICommandPalette, n.ILayoutRestorer, s.IConsoleTracker, n.ILabShell, r.IFileBrowserFactory],
-                activate: (e, t, a, n, r, s) => {
+                requires: [o.ICommandPalette, a.ILayoutRestorer, s.IConsoleTracker, a.ILabShell, r.IFileBrowserFactory],
+                activate: (e, t, n, a, r, s) => {
                     console.log("JupyterLab extension tvb-ext-bucket is activated!");
                     const l = s.defaultBrowser;
                     w.current = l;
-                    const i = "tvb-ext-bucket",
-                        c = new U;
-                    c.id = i, c.title.iconClass = "bucket-CollabLogo jp-SideBar-tabIcon", c.title.caption = "Bucket", r.add(c, "right", {
+                    const c = "tvb-ext-bucket",
+                        i = new T;
+                    i.id = c, i.title.iconClass = "bucket-CollabLogo jp-SideBar-tabIcon", i.title.caption = "Bucket", r.add(i, "right", {
                         rank: 200
                     });
                     const u = new o.WidgetTracker({
                         namespace: "bucket"
                     });
-                    a.add(c, i), a.restore(u, {
+                    n.add(i, c), n.restore(u, {
                         command: "tvbextbucket:open",
                         name: () => "bucket"
                     })
                 }
             }
         }
     }
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/747.8201db85e4d2a978f4c3.js` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/747.e24cd10495543003a807.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
                 c = t(453),
                 s = t.n(c),
                 d = r()((function(n) {
                     return n[1]
                 })),
                 u = a()(l.Z),
                 p = a()(s());
-            d.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n:root {\n  --bucket-download-color: #060;\n  --bucket-text-info-color: #d3d3d3;\n}\n\n/* --------- SPIN ANIMATION ---------- */\n@keyframes spin {\n  from {\n    -moz-transform: rotate(0deg);\n  }\n\n  to {\n    -moz-transform: rotate(360deg);\n  }\n}\n@keyframes spin {\n  from {\n    -webkit-transform: rotate(0deg);\n  }\n\n  to {\n    -webkit-transform: rotate(360deg);\n  }\n}\n@keyframes spin {\n  from {\n    transform: rotate(0deg);\n  }\n\n  to {\n    transform: rotate(360deg);\n  }\n}\n\n/* --------- END SPIN ANIMATION ---------- */\n\n.bucket-container,\n.tvb-bucketWidget {\n  background-color: var(--jp-layout-color1);\n  list-style-type: none;\n}\n\n.bucket-BreadCrumbs {\n  display: flex;\n  flex-flow: row wrap;\n  align-items: center;\n  justify-content: flex-start;\n}\n\n.bucket-BreadCrumbs-Item {\n  cursor: pointer;\n  color: var(--md-blue-500);\n}\n\n.bucket-BreadCrumbs-Item:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.bucket-container ul {\n  list-style-type: none;\n  padding: 0;\n  margin: 0;\n}\n\n.bucket-container ul > li {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: flex-start;\n  padding-left: 1em;\n}\n\n.bucket-BrowserListItem:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.bucket-ContextMenu-container {\n  position: relative;\n}\n\n.bucket-ContextMenu {\n  position: absolute;\n  top: 10px;\n  left: 5px;\n  z-index: 10000;\n  padding: 4px 0;\n  font-size: var(--jp-ui-font-size1);\n  background: var(--jp-layout-color0);\n  color: var(--jp-ui-font-color1);\n  border: var(--jp-border-width) solid var(--jp-ui-font-size1);\n  box-shadow: var(--jp-elevation-z6);\n  white-space: nowrap;\n  overflow-x: hidden;\n  overflow-y: auto;\n  outline: none;\n  opacity: 1;\n  width: 200px;\n}\n\n.bucket-ContextMenu-item {\n  min-height: var(--jp-private-menu-item-height);\n  max-height: var(--jp-private-menu-item-height);\n  line-height: var(--jp-private-menu-item-height);\n}\n\n.bucket-ContextMenu-item div {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\n\n.bucket-ContextMenu li:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.collab-logo {\n  display: inline-block;\n  background-image: url(" + u + ");\n  background-repeat: no-repeat;\n  background-size: contain;\n  height: 40px;\n  width: 30px;\n  margin-left: 1em;\n}\n\n.bucket-logo {\n  display: flex;\n  align-items: center;\n  justify-content: flex-start;\n}\n\n.bucket-logo-text {\n  margin-left: 0.2em;\n  font-size: 1.2em;\n  display: inline-block;\n}\n\n.bucket-CollabLogo {\n  background-image: url(" + p + ");\n  filter: opacity(70%);\n}\n\n.bucket-Spinner {\n  display: inline-block;\n  border: 3px solid #7f7f7f;\n  border-left: 3px solid #4ec261;\n  height: 1em;\n  width: 1em;\n  border-radius: 50%;\n  margin: 0 0.5em;\n  animation: spin 0.5s infinite linear;\n}\n\n.align-flex-horizontal {\n  display: flex;\n  flex-direction: row;\n  align-items: flex-start;\n  justify-content: center;\n}\n\n@keyframes rain {\n  0% {\n    top: -1em;\n    opacity: 0;\n  }\n\n  50% {\n    opacity: 1;\n  }\n\n  100% {\n    top: 1em;\n    opacity: 0;\n  }\n}\n\n/* download animation style */\n.bucket-DownloadAnimation {\n  display: inline-block;\n  z-index: 2;\n  position: relative;\n  height: 0.8em;\n  width: 1em;\n  margin-left: 0.5em;\n  margin-top: 0.2em;\n  overflow: hidden;\n  border-top: solid 1px var(--bucket-download-color);\n}\n\n.bucket-DownloadAnimation i {\n  color: var(--bucket-download-color);\n  position: absolute;\n  z-index: 1;\n  animation: linear 0.5s rain infinite;\n}\n\n/* end download animation style */\n\n/* upload animation style */\n.bucket-UploadAnimation {\n  display: inline-block;\n  z-index: 2;\n  position: relative;\n  height: 0.8em;\n  width: 1em;\n  margin-left: 0.5em;\n  margin-top: 0.2em;\n  overflow: hidden;\n  border-top: solid 1px var(--bucket-download-color);\n}\n\n.bucket-UploadAnimation > :first-child {\n  color: var(--bucket-download-color);\n  position: absolute;\n  z-index: 1;\n  animation: reverse 0.5s rain infinite;\n}\n\n/* end upload animation style */\n\n.bucket-DropZone {\n  margin: 0 auto;\n  padding: 0.5em;\n  width: 90%;\n  height: 4em;\n  border: dashed 2px var(--bucket-text-info-color);\n  border-radius: 7px;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\n\n.default {\n  border-color: var(--bucket-text-info-color);\n}\n\n.hover {\n  border-color: black;\n}\n\n.bucket-text-info {\n  color: var(--bucket-text-info-color);\n  font-style: italic;\n}\n\n.bucket-Tooltip {\n  position: absolute;\n  top: 5vh;\n  z-index: 99;\n  width: 100%;\n  height: 4em;\n  background-color: var(--jp-layout-color1);\n  border-radius: 7px;\n  box-shadow: var(--jp-elevation-z6);\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n  justify-content: center;\n  padding: 0.5em;\n}\n\n.bucket-ShareLink {\n  color: var(--md-blue-500);\n}\n\n.bucket-ShareLink:hover {\n  text-decoration: underline;\n}\n\n.scrollableY {\n  max-height: 70vh;\n  overflow-y: auto;\n  overflow-x: hidden;\n}\n\n.bucket-container ul.available-buckets {\n  max-height: 40vh;\n  position: absolute;\n  top: 4.5em;\n  z-index: 9999;\n  background-color: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z6);\n  overflow-x: hidden;\n  overflow-y: auto;\n  padding-top: 0.5em;\n  padding-bottom: 0.5em;\n  width: 100%;\n}\n\n.bucket-container ul.available-buckets > li:hover {\n  background-color: var(--jp-layout-color2);\n  cursor: pointer;\n}\n", ""]);
+            d.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n:root {\n  --bucket-download-color: #060;\n  --bucket-text-info-color: #d3d3d3;\n}\n\n/* --------- SPIN ANIMATION ---------- */\n@keyframes spin {\n  from {\n    -moz-transform: rotate(0deg);\n  }\n\n  to {\n    -moz-transform: rotate(360deg);\n  }\n}\n@keyframes spin {\n  from {\n    -webkit-transform: rotate(0deg);\n  }\n\n  to {\n    -webkit-transform: rotate(360deg);\n  }\n}\n@keyframes spin {\n  from {\n    transform: rotate(0deg);\n  }\n\n  to {\n    transform: rotate(360deg);\n  }\n}\n\n/* --------- END SPIN ANIMATION ---------- */\n\n.bucket-container,\n.tvb-bucketWidget {\n  background-color: var(--jp-layout-color1);\n  list-style-type: none;\n}\n\n.bucket-BreadCrumbs {\n  display: flex;\n  flex-flow: row wrap;\n  align-items: center;\n  justify-content: flex-start;\n}\n\n.bucket-BreadCrumbs-Item {\n  cursor: pointer;\n  color: var(--md-blue-500);\n}\n\n.bucket-BreadCrumbs-Item:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.bucket-container ul {\n  list-style-type: none;\n  padding: 0;\n  margin: 0;\n}\n\n.bucket-container ul > li {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: flex-start;\n  padding-left: 1em;\n}\n\n.bucket-BrowserListItem:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.bucket-ContextMenu-container {\n  position: relative;\n}\n\n.bucket-ContextMenu {\n  position: absolute;\n  top: 10px;\n  left: 5px;\n  z-index: 10000;\n  padding: 4px 0;\n  font-size: var(--jp-ui-font-size1);\n  background: var(--jp-layout-color0);\n  color: var(--jp-ui-font-color1);\n  border: var(--jp-border-width) solid var(--jp-ui-font-size1);\n  box-shadow: var(--jp-elevation-z6);\n  white-space: nowrap;\n  overflow-x: hidden;\n  overflow-y: auto;\n  outline: none;\n  opacity: 1;\n  width: 200px;\n}\n\n.bucket-ContextMenu-item {\n  min-height: var(--jp-private-menu-item-height);\n  max-height: var(--jp-private-menu-item-height);\n  line-height: var(--jp-private-menu-item-height);\n}\n\n.bucket-ContextMenu-item div {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\n\n.bucket-ContextMenu li:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.collab-logo {\n  display: inline-block;\n  background-image: url(" + u + ");\n  background-repeat: no-repeat;\n  background-size: contain;\n  height: 40px;\n  width: 30px;\n  margin-left: 1em;\n}\n\n.bucket-logo {\n  display: flex;\n  align-items: center;\n  justify-content: flex-start;\n}\n\n.bucket-logo-text {\n  margin-left: 0.2em;\n  font-size: 1.2em;\n  display: inline-block;\n}\n\n.bucket-CollabLogo {\n  background-image: url(" + p + ");\n  filter: opacity(70%);\n}\n\n.bucket-Spinner {\n  display: inline-block;\n  border: 3px solid #7f7f7f;\n  border-left: 3px solid #4ec261;\n  height: 1em;\n  width: 1em;\n  border-radius: 50%;\n  margin: 0 0.5em;\n  animation: spin 0.5s infinite linear;\n}\n\n.bucket-home {\n  cursor: pointer;\n  padding: 0 3px;\n  display: inline-block;\n}\n\n.bucket-home:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.align-flex-horizontal {\n  display: flex;\n  flex-direction: row;\n  align-items: flex-start;\n  justify-content: center;\n}\n\n@keyframes rain {\n  0% {\n    top: -1em;\n    opacity: 0;\n  }\n\n  50% {\n    opacity: 1;\n  }\n\n  100% {\n    top: 1em;\n    opacity: 0;\n  }\n}\n\n/* download animation style */\n.bucket-DownloadAnimation {\n  display: inline-block;\n  z-index: 2;\n  position: relative;\n  height: 0.8em;\n  width: 1em;\n  margin-left: 0.5em;\n  margin-top: 0.2em;\n  overflow: hidden;\n  border-top: solid 1px var(--bucket-download-color);\n}\n\n.bucket-DownloadAnimation i {\n  color: var(--bucket-download-color);\n  position: absolute;\n  z-index: 1;\n  animation: linear 0.5s rain infinite;\n}\n\n/* end download animation style */\n\n/* upload animation style */\n.bucket-UploadAnimation {\n  display: inline-block;\n  z-index: 2;\n  position: relative;\n  height: 0.8em;\n  width: 1em;\n  margin-left: 0.5em;\n  margin-top: 0.2em;\n  overflow: hidden;\n  border-top: solid 1px var(--bucket-download-color);\n}\n\n.bucket-UploadAnimation > :first-child {\n  color: var(--bucket-download-color);\n  position: absolute;\n  z-index: 1;\n  animation: reverse 0.5s rain infinite;\n}\n\n/* end upload animation style */\n\n.bucket-DropZone {\n  margin: 0 auto;\n  padding: 0.5em;\n  width: 90%;\n  height: 4em;\n  border: dashed 2px var(--bucket-text-info-color);\n  border-radius: 7px;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\n\n.default {\n  border-color: var(--bucket-text-info-color);\n}\n\n.hover {\n  border-color: black;\n}\n\n.bucket-text-info {\n  color: var(--bucket-text-info-color);\n  font-style: italic;\n}\n\n.bucket-Tooltip {\n  position: absolute;\n  top: 5vh;\n  z-index: 99;\n  width: 100%;\n  height: 4em;\n  background-color: var(--jp-layout-color1);\n  border-radius: 7px;\n  box-shadow: var(--jp-elevation-z6);\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n  justify-content: center;\n  padding: 0.5em;\n}\n\n.bucket-ShareLink {\n  color: var(--md-blue-500);\n}\n\n.bucket-ShareLink:hover {\n  text-decoration: underline;\n}\n\n.scrollableY {\n  max-height: 70vh;\n  overflow-y: auto;\n  overflow-x: hidden;\n}\n\n.bucket-container ul.available-buckets {\n  max-height: 40vh;\n  position: absolute;\n  top: 4.5em;\n  z-index: 9999;\n  background-color: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z6);\n  overflow-x: hidden;\n  overflow-y: auto;\n  padding-top: 0.5em;\n  padding-bottom: 0.5em;\n  width: 100%;\n}\n\n.bucket-container ul.available-buckets > li:hover {\n  background-color: var(--jp-layout-color2);\n  cursor: pointer;\n}\n\n.bucket-Settings {\n  position: absolute;\n  z-index: 9999;\n  background-color: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z6);\n  top: 2em;\n  right: 1em;\n  left: 1em;\n  display: flex;\n  flex-direction: column;\n  padding: 0.5em;\n}\n\n.bucket-Settings h4 {\n  margin: 0;\n  font-weight: 600;\n}\n\n.bucket-Settings-toggle {\n  display: inline-block;\n  margin-left: auto;\n  margin-right: 1em;\n  cursor: pointer;\n}\n\n.bucket-Settings-container {\n  margin-right: 0;\n  margin-left: auto;\n}\n", ""]);
             const f = d
         },
         645: n => {
             "use strict";
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/acb28ef48e64b689e3e44624dd56425825ae6f016b1ff6d65e9004f9d15b3301.png` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/acb28ef48e64b689e3e44624dd56425825ae6f016b1ff6d65e9004f9d15b3301.png`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/remoteEntry.b2ee1fefe23289008a39.js` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/remoteEntry.c935a8c2bed6559fef34.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, d, s, c, p, h, v = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, c, p, h, v = {
             368: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(529).then((() => () => t(529))),
-                        "./extension": () => t.e(529).then((() => () => t(529))),
+                        "./index": () => t.e(522).then((() => () => t(522))),
+                        "./extension": () => t.e(522).then((() => () => t(522))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,49 +43,49 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        529: "3f5fcb349df6ed19fa54",
-        747: "8201db85e4d2a978f4c3"
+        522: "88137ffbe3671c70bd7e",
+        747: "e24cd10495543003a807"
     } [e] + ".js?v=" + {
-        529: "3f5fcb349df6ed19fa54",
-        747: "8201db85e4d2a978f4c3"
+        522: "88137ffbe3671c70bd7e",
+        747: "e24cd10495543003a807"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "tvb-ext-bucket:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -102,19 +102,19 @@
                 var a = g.S[t],
                     i = "tvb-ext-bucket",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => g.e(529).then((() => () => g(529))),
+                        get: () => g.e(522).then((() => () => g(522))),
                         from: i,
                         eager: !1
                     })
-                })("tvb-ext-bucket", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("tvb-ext-bucket", "1.0.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -163,33 +163,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (s == d)
+                    if (d == s)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (o ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < s != o) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
@@ -200,31 +200,31 @@
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
-    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, p = {
-        258: () => s("default", "@jupyterlab/services", [1, 6, 6, 1]),
-        271: () => s("default", "react", [1, 17, 0, 1]),
-        468: () => s("default", "@jupyterlab/console", [1, 3, 6, 1]),
-        510: () => s("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        535: () => s("default", "@jupyterlab/filebrowser", [1, 3, 6, 1]),
-        591: () => s("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        694: () => s("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        866: () => s("default", "@jupyterlab/application", [1, 3, 6, 1]),
-        886: () => s("default", "@jupyterlab/coreutils", [1, 5, 6, 1])
+        122: () => d("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        139: () => d("default", "@jupyterlab/services", [1, 6, 6, 5]),
+        271: () => d("default", "react", [1, 17, 0, 1]),
+        303: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        344: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
+        526: () => d("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        543: () => d("default", "@jupyterlab/console", [1, 3, 6, 5]),
+        638: () => d("default", "@jupyterlab/application", [1, 3, 6, 5]),
+        694: () => d("default", "@lumino/dragdrop", [1, 1, 13, 0]),
+        745: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 5])
     }, h = {
-        529: [258, 271, 468, 510, 526, 535, 591, 694, 866, 886]
+        522: [122, 139, 271, 303, 344, 526, 543, 638, 694, 745]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
             if (g.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
```

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/labextension/static/third-party-licenses.json` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/logger/builder.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/logger/logging.conf` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_bucket.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_buckets.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_dataproxy_file.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_dataproxy_file.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/tvb_ext_bucket/tests/test_drive_wrapper.py` & `tvb_ext_bucket-1.0.0/tvb_ext_bucket/tests/test_drive_wrapper.py`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/.gitignore` & `tvb_ext_bucket-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/LICENSE` & `tvb_ext_bucket-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/README.md` & `tvb_ext_bucket-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/pyproject.toml` & `tvb_ext_bucket-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvb_ext_bucket-0.3.0/PKG-INFO` & `tvb_ext_bucket-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb_ext_bucket
-Version: 0.3.0
+Version: 1.0.0
 Summary: Extension for collabs bucket interaction
 Project-URL: Homepage, https://github.com/the-virtual-brain/tvb-ext-bucket
 Project-URL: Bug Tracker, https://github.com/the-virtual-brain/tvb-ext-bucket/issues
 Project-URL: Repository, https://github.com/the-virtual-brain/tvb-ext-bucket.git
 Author-email: TVB Widgets Team <tvb.admin@thevirtualbrain.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

