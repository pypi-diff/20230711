# Comparing `tmp/matlab-proxy-0.7.0.tar.gz` & `tmp/matlab-proxy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-proxy-0.7.0.tar", last modified: Wed Jun 21 05:23:54 2023, max compression
+gzip compressed data, was "matlab-proxy-0.7.2.tar", last modified: Tue Jul 11 10:01:55 2023, max compression
```

## Comparing `matlab-proxy-0.7.0.tar` & `matlab-proxy-0.7.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.336860 matlab-proxy-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-21 05:23:54.336860 matlab-proxy-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.316859 matlab-proxy-0.7.0/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1289896 2023-06-21 05:23:31.000000 matlab-proxy-0.7.0/gui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.316859 matlab-proxy-0.7.0/gui/public/
--rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.316859 matlab-proxy-0.7.0/gui/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.316859 matlab-proxy-0.7.0/gui/src/actionCreators/
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/actionCreators/actionCreators.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/actionCreators/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.316859 matlab-proxy-0.7.0/gui/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.312859 matlab-proxy-0.7.0/gui/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.316859 matlab-proxy-0.7.0/gui/src/components/App/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.312859 matlab-proxy-0.7.0/gui/src/components/App/3p/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.320859 matlab-proxy-0.7.0/gui/src/components/App/3p/css/
--rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/css/site7.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.320859 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-eps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-eps.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-eps.woff
--rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
--rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
--rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.312859 matlab-proxy-0.7.0/gui/src/components/App/3p/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.320859 matlab-proxy-0.7.0/gui/src/components/App/3p/images/bug_reports/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/images/bug_reports/workaround.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.312859 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.324859 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/App.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/MATLAB-env-blur.png
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/App/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.324859 matlab-proxy-0.7.0/gui/src/components/Confirmation/
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Confirmation/Confirmation.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Confirmation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.324859 matlab-proxy-0.7.0/gui/src/components/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/Controls.css
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/Controls.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/feedback.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/help.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/sign-out.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/start.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Controls/terminate.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.324859 matlab-proxy-0.7.0/gui/src/components/Error/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Error/Error.css
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Error/Error.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Error/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.324859 matlab-proxy-0.7.0/gui/src/components/Help/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Help/Help.css
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Help/Help.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Help/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.324859 matlab-proxy-0.7.0/gui/src/components/Information/
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Information/Information.css
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Information/Information.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Information/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/ExistingLicense.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/ExistingLicense.js
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/LicensingGatherer.css
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/MHLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/NLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/components/MatlabJsd/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/MatlabJsd/MatlabJsd.css
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/MatlabJsd/MatlabJsd.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/MatlabJsd/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/components/Overlay/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Overlay/Overlay.css
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Overlay/Overlay.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/Overlay/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/OverlayTrigger.css
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/gripper.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/trigger-error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/trigger-ok.svg
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/jest.config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/reducers/
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/reducers/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/reducers/reducers.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/selectors/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/selectors/selectors.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/setupTests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.312859 matlab-proxy-0.7.0/gui/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.328859 matlab-proxy-0.7.0/gui/src/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/gui/src/test/utils/react-test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.332859 matlab-proxy-0.7.0/matlab_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    50370 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/app_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/default_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/devel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.332859 matlab-proxy-0.7.0/matlab_proxy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/icons/matlab.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.332859 matlab-proxy-0.7.0/matlab_proxy/matlab/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/matlab/startup.m
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.332859 matlab-proxy-0.7.0/matlab_proxy/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/list_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.336860 matlab-proxy-0.7.0/matlab_proxy/util/mwi/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/custom_http_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.336860 matlab-proxy-0.7.0/matlab_proxy/util/mwi/embedded_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/embedded_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/embedded_connector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/embedded_connector/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/mwi/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/matlab_proxy/util/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:54.332859 matlab-proxy-0.7.0/matlab_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 05:23:05.000000 matlab-proxy-0.7.0/matlab_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 05:23:54.336860 matlab-proxy-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-21 05:22:20.000000 matlab-proxy-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1289896 2023-07-11 10:01:38.000000 matlab-proxy-0.7.2/gui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/actionCreators/
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/actionCreators/actionCreators.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/actionCreators/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/components/App/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/App/3p/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/components/App/3p/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/css/site7.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/bug_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/bug_reports/workaround.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/App.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/MATLAB-env-blur.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Confirmation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Confirmation/Confirmation.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Confirmation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/Controls.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/Controls.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/feedback.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/sign-out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/terminate.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Error/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Error/Error.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Error/Error.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Error/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Help/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Help/Help.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Help/Help.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Help/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Information/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Information/Information.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Information/Information.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Information/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/ExistingLicense.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/ExistingLicense.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/LicensingGatherer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/MHLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/NLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/MatlabJsd.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/MatlabJsd.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/Overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.css
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Overlay/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/gripper.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-ok.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/jest.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/reducers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/reducers/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/reducers/reducers.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/selectors/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/selectors/selectors.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/setupTests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/test/utils/react-test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50370 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/app_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/default_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/devel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/icons/matlab.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/matlab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/matlab/startup.m
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/list_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/matlab_proxy/util/mwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/custom_http_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/setup.py
```

### Comparing `matlab-proxy-0.7.0/LICENSE.md` & `matlab-proxy-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/PKG-INFO` & `matlab-proxy-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.7.0
+Version: 0.7.2
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
```

### Comparing `matlab-proxy-0.7.0/README.md` & `matlab-proxy-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/README.md` & `matlab-proxy-0.7.2/gui/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/package-lock.json` & `matlab-proxy-0.7.2/gui/package-lock.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/package.json` & `matlab-proxy-0.7.2/gui/package.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/public/favicon.ico` & `matlab-proxy-0.7.2/gui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/public/index.html` & `matlab-proxy-0.7.2/gui/public/index.html`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/actionCreators/actionCreators.spec.js` & `matlab-proxy-0.7.2/gui/src/actionCreators/actionCreators.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/actionCreators/index.js` & `matlab-proxy-0.7.2/gui/src/actionCreators/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/actions/index.js` & `matlab-proxy-0.7.2/gui/src/actions/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/css/bootstrap.min.css` & `matlab-proxy-0.7.2/gui/src/components/App/3p/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/css/site7.min.css` & `matlab-proxy-0.7.2/gui/src/components/App/3p/css/site7.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-eps.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-eps.ttf` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-eps.woff` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-pictograms.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks-pictograms.woff` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks.ttf` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/fonts/mathworks.woff` & `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/images/bug_reports/workaround.gif` & `matlab-proxy-0.7.2/gui/src/components/App/3p/images/bug_reports/workaround.gif`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg` & `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/3p/images/responsive/global/ico-sprite.png` & `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-sprite.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/App.css` & `matlab-proxy-0.7.2/gui/src/components/App/App.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/App.spec.js` & `matlab-proxy-0.7.2/gui/src/components/App/App.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/MATLAB-env-blur.png` & `matlab-proxy-0.7.2/gui/src/components/App/MATLAB-env-blur.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/App/index.js` & `matlab-proxy-0.7.2/gui/src/components/App/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Confirmation/Confirmation.spec.js` & `matlab-proxy-0.7.2/gui/src/components/Confirmation/Confirmation.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Confirmation/index.js` & `matlab-proxy-0.7.2/gui/src/components/Confirmation/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/Controls.css` & `matlab-proxy-0.7.2/gui/src/components/Controls/Controls.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/Controls.spec.js` & `matlab-proxy-0.7.2/gui/src/components/Controls/Controls.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/feedback.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/feedback.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/help.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/help.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/index.js` & `matlab-proxy-0.7.2/gui/src/components/Controls/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/restart.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/restart.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/sign-out.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/sign-out.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/start.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/start.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/stop.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/stop.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Controls/terminate.svg` & `matlab-proxy-0.7.2/gui/src/components/Controls/terminate.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Error/Error.spec.js` & `matlab-proxy-0.7.2/gui/src/components/Error/Error.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Error/index.js` & `matlab-proxy-0.7.2/gui/src/components/Error/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Help/Help.spec.js` & `matlab-proxy-0.7.2/gui/src/components/Help/Help.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Help/index.js` & `matlab-proxy-0.7.2/gui/src/components/Help/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Information/Information.css` & `matlab-proxy-0.7.2/gui/src/components/Information/Information.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Information/Information.spec.js` & `matlab-proxy-0.7.2/gui/src/components/Information/Information.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Information/index.js` & `matlab-proxy-0.7.2/gui/src/components/Information/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/ExistingLicense.js` & `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/ExistingLicense.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js` & `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/MHLM.js` & `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/MHLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/NLM.js` & `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/NLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/LicensingGatherer/index.js` & `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/MatlabJsd/MatlabJsd.spec.js` & `matlab-proxy-0.7.2/gui/src/components/MatlabJsd/MatlabJsd.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Overlay/Overlay.css` & `matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Overlay/Overlay.spec.js` & `matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/Overlay/index.js` & `matlab-proxy-0.7.2/gui/src/components/Overlay/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/OverlayTrigger.css` & `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js` & `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js` & `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/index.js` & `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/trigger-error.svg` & `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-error.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/components/OverlayTrigger/trigger-ok.svg` & `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-ok.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/index.js` & `matlab-proxy-0.7.2/gui/src/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/logo.svg` & `matlab-proxy-0.7.2/gui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/reducers/index.js` & `matlab-proxy-0.7.2/gui/src/reducers/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/reducers/reducers.spec.js` & `matlab-proxy-0.7.2/gui/src/reducers/reducers.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/selectors/index.js` & `matlab-proxy-0.7.2/gui/src/selectors/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/selectors/selectors.spec.js` & `matlab-proxy-0.7.2/gui/src/selectors/selectors.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/serviceWorker.js` & `matlab-proxy-0.7.2/gui/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/gui/src/test/utils/react-test.js` & `matlab-proxy-0.7.2/gui/src/test/utils/react-test.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/__init__.py` & `matlab-proxy-0.7.2/matlab_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/app.py` & `matlab-proxy-0.7.2/matlab_proxy/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import asyncio
 import json
 import mimetypes
 import pkgutil
 import sys
 
@@ -15,15 +15,15 @@
 import matlab_proxy
 from matlab_proxy import settings, util
 from matlab_proxy.app_state import AppState
 from matlab_proxy.default_configuration import config
 from matlab_proxy.util import list_servers, mwi
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
-from matlab_proxy.util.mwi.exceptions import AppError, LicensingError, InvalidTokenError
+from matlab_proxy.util.mwi.exceptions import AppError, InvalidTokenError, LicensingError
 
 mimetypes.add_type("font/woff", ".woff")
 mimetypes.add_type("font/woff2", ".woff2")
 mimetypes.add_type("font/eot", ".eot")
 mimetypes.add_type("font/ttf", ".ttf")
 mimetypes.add_type("application/json", ".map")
 mimetypes.add_type("image/png", ".ico")
@@ -300,16 +300,16 @@
     await res.prepare(req)
     await res.write_eof()
 
     logger.debug("Shutting down the server...")
     # End termination with 0 exit code to indicate intentional termination
     await req.app.shutdown()
     await req.app.cleanup()
-    """When testing with pytest, its not possible to catch sys.exit(0) using the construct 
-    'with pytest.raises()', there by causing the test : test_termination_integration_delete() 
+    """When testing with pytest, its not possible to catch sys.exit(0) using the construct
+    'with pytest.raises()', there by causing the test : test_termination_integration_delete()
     to fail. Inorder to avoid this, adding the below if condition to check to skip sys.exit(0) when testing
     """
     logger.debug("Exiting with return code 0")
     if not mwi_env.is_testing_mode_enabled():
         sys.exit(0)
 
 
@@ -404,28 +404,33 @@
     Raises:
         ValueError: When unable to handle WebSocket Request.
         web.HTTPNotFound: When a non-existing file is requested.
 
     Returns:
         WebSocketResponse or HTTPResponse: based on the Request type.
     """
+    # Special keys for web socket requests
+    CONNECTION = "connection"
+    UPGRADE = "upgrade"
+
     reqH = req.headers.copy()
 
     state = req.app["state"]
     matlab_port = state.matlab_port
     matlab_protocol = req.app["settings"]["matlab_protocol"]
     mwapikey = req.app["settings"]["mwapikey"]
     matlab_base_url = f"{matlab_protocol}://127.0.0.1:{matlab_port}"
 
     # WebSocket
+    # According to according to RFC6455 (https://www.rfc-editor.org/rfc/rfc6455.html)
+    # the values of 'connection' and 'upgrade'  keys of request header
+    # should be ASCII case-insensitive matches.
     if (
-        reqH.get("connection")
-        and reqH.get("connection").lower() == "upgrade"
-        and reqH.get("upgrade")
-        and reqH.get("upgrade").lower() == "websocket"
+        reqH.get(CONNECTION, "").lower() == UPGRADE
+        and reqH.get(UPGRADE, "").lower() == "websocket"
         and req.method == "GET"
     ):
         ws_server = web.WebSocketResponse()
         await ws_server.prepare(req)
 
         async with aiohttp.ClientSession(
             cookies=req.cookies, connector=aiohttp.TCPConnector(verify_ssl=False)
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/app_state.py` & `matlab-proxy-0.7.2/matlab_proxy/app_state.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/default_configuration.py` & `matlab-proxy-0.7.2/matlab_proxy/default_configuration.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/devel.py` & `matlab-proxy-0.7.2/matlab_proxy/devel.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/icons/matlab.svg` & `matlab-proxy-0.7.2/matlab_proxy/icons/matlab.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/matlab/startup.m` & `matlab-proxy-0.7.2/matlab_proxy/matlab/startup.m`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/settings.py` & `matlab-proxy-0.7.2/matlab_proxy/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,36 +7,76 @@
 import sys
 import tempfile
 import uuid
 import xml.etree.ElementTree as ET
 from pathlib import Path
 
 import matlab_proxy
+from matlab_proxy.constants import VERSION_INFO_FILE_NAME
 from matlab_proxy.util import mwi, system
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
 
 logger = mwi.logger.get()
 
 
-def get_matlab_path():
+def get_matlab_root_path():
+    """Returns the path from the MWI_CUSTOM_MATLAB_ROOT environment variable if valid, else returns
+    MATLAB root based on the matlab executable if found on the system path.
+
+    Returns:
+        pathlib.Path: pathlib.Path object to MATLAB root.
+    """
+    custom_matlab_root_path = os.environ.get(mwi_env.get_env_name_custom_matlab_root())
+
+    if custom_matlab_root_path and mwi.validators.validate_custom_matlab_root_path(
+        Path(custom_matlab_root_path)
+    ):
+        return custom_matlab_root_path
+
     which_matlab = shutil.which("matlab")
-    if which_matlab is None:
+
+    return Path(which_matlab).resolve().parent.parent if which_matlab else None
+
+
+def get_matlab_executable_path(matlab_root_path: Path):
+    """Returns path to the MATLAB executable based on the OS
+
+    Args:
+        matlab_root_path (Path): Path to MATLAB Root
+
+    Returns:
+        [Path | None]: Path to MATLAB executable if a valid MATLAB root path is supplied else return None
+    """
+    if not matlab_root_path:
         return None
-    return Path(which_matlab).resolve().parent.parent
 
+    return (
+        matlab_root_path / "bin" / "matlab"
+        if system.is_posix()
+        else matlab_root_path / "bin" / "matlab.exe"
+    )
 
-def get_matlab_version(matlab_path):
-    """Get the MATLAB Release version in this image"""
 
-    if matlab_path is None:
+def get_matlab_version(matlab_root_path):
+    """Returns MATLAB version from VersionInfo.xml file present at matlab_root_path
+
+    Args:
+        matlab_root_path (pathlib.Path): pathlib.Path to MATLAB root.
+
+    Returns:
+        (str | None): Returns MATLAB version from VersionInfo.xml file.
+    """
+    if matlab_root_path is None:
         return None
 
-    tree = ET.parse(matlab_path / "VersionInfo.xml")
+    version_info_file_path = Path(matlab_root_path) / VERSION_INFO_FILE_NAME
+    tree = ET.parse(version_info_file_path)
     root = tree.getroot()
+
     return root.find("release").text
 
 
 def get_ws_env_settings():
     ws_env = (os.getenv("WS_ENV") or "").lower()
     ws_env_suffix = f"-{ws_env}" if "integ" in ws_env else ""
 
@@ -133,15 +173,16 @@
 
         return settings
 
     else:
         matlab_startup_file = str(
             Path(__file__).resolve().parent / "matlab" / "startup.m"
         )
-        matlab_path = get_matlab_path()
+        matlab_path = get_matlab_root_path()
+        matlab_executable_path = get_matlab_executable_path(Path(matlab_path))
         ws_env, ws_env_suffix = get_ws_env_settings()
 
         ssl_key_file, ssl_cert_file = mwi.validators.validate_ssl_key_and_cert_file(
             os.getenv(mwi_env.get_env_name_ssl_key_file(), None),
             os.getenv(mwi_env.get_env_name_ssl_cert_file(), None),
         )
 
@@ -168,15 +209,15 @@
         # This will allow for other user's to launch the integration from the same system
         # and not have their config's overwritten.
         mwi_config_folder = get_mwi_config_folder()
         return {
             "matlab_path": matlab_path,
             "matlab_version": get_matlab_version(matlab_path),
             "matlab_cmd": [
-                "matlab",
+                matlab_executable_path,
                 "-nosplash",
                 flag_to_hide_desktop,
                 "-softwareopengl",
                 *matlab_lic_mode,
                 "-r",
                 f"try; run('{matlab_startup_file}'); catch ME; disp(ME.message); end;",
             ],
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/__init__.py` & `matlab-proxy-0.7.2/matlab_proxy/util/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 import argparse
 import os
 import socket
-import sys
+
+from pathlib import Path
 
 import matlab_proxy
 from matlab_proxy.util import mwi, system
 from matlab_proxy.util.event_loop import *
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 
 logger = mwi.logger.get()
@@ -237,7 +238,20 @@
         fqdn = socket.getfqdn(hostname)
 
         url = f"{access_protocol}://{fqdn}:{port}{base_url}"
     else:
         url = f"{access_protocol}://{host_interface}:{port}{base_url}"
 
     return url
+
+
+def is_valid_path(path: Path):
+    """Returns true if path supplied is a valid path to a file or directory
+
+    Args:
+        path (pathlib.Path): pathlib.Path object of a file or directory
+
+    Returns:
+        bool: True if a valid path is supplied else False
+    """
+    path = Path(path)
+    return path.is_dir() or path.is_file()
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/event_loop.py` & `matlab-proxy-0.7.2/matlab_proxy/util/event_loop.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/list_servers.py` & `matlab-proxy-0.7.2/matlab_proxy/util/list_servers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mw.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mw.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     "release": matlab_release,
                     "coreProduct": "ML",
                     "context": "jupyter",
                     "excludeExpired": "true",
                 }
             ),
         ) as res:
-            if res.reason != "OK":
+            if not res.ok:
                 raise OnlineLicensingError(
                     f"Communication with {mhlm_api_endpoint} failed ({res.status}). For more details, see {__get_licensing_url()}."
                 )
 
             root = ET.fromstring(await res.text())
             entitlement_el = root.find("entitlements")
 
@@ -110,15 +110,15 @@
                 {
                     "tokenString": identity_token,
                     "tokenPolicyName": "R2",
                     "sourceId": source_id,
                 }
             ),
         ) as res:
-            if res.reason != "OK":
+            if not res.ok:
                 raise OnlineLicensingError(
                     f"Communication with {mwa_api_endpoint} failed ({res.status}). For more details, see {__get_licensing_url()}."
                 )
 
             data = await res.json()
 
             return {
@@ -157,15 +157,15 @@
                 {
                     "tokenString": identity_token,
                     "type": "MWAS",
                     "sourceId": source_id,
                 }
             ),
         ) as res:
-            if res.reason != "OK":
+            if not res.ok:
                 raise OnlineLicensingError(
                     f"Communication with {mwa_api_endpoint} failed ({res.status}). For more details, see {__get_licensing_url()}."
                 )
 
             data = await res.json()
 
             return {
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/custom_http_headers.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/custom_http_headers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/embedded_connector/helpers.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/helpers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/embedded_connector/request.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         data = json.dumps(data)
 
     try:
         async with aiohttp.ClientSession() as session:
             async with session.request(
                 method=method, url=url, data=data, headers=None, ssl=False
             ) as resp:
-                if resp.reason != "OK":
+                if not resp.ok:
                     # Converting to dict and formatting for printing
                     data = json.loads(data)
 
                     raise EmbeddedConnectorError(
                         f"""Failed to communicate with Embedded Connector.\nHTTP Request details:\n{json.dumps(data, indent=2)}"""
                     )
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/environment_variables.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/environment_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 """This file lists and exposes the environment variables which are used by the integration."""
 
 import os
 
 
 def get_env_name_network_license_manager():
     """Specifies the path to valid license file or address of a network license server"""
@@ -141,7 +141,12 @@
     """Returns the key used for MATLAB log dir env variable"""
     return "MATLAB_LOG_DIR"
 
 
 def get_env_name_mwi_use_existing_license():
     """Returns the environment variable name used to instruct matlab-proxy to use an existing license. Usually used by already activated MATLAB installations."""
     return "MWI_USE_EXISTING_LICENSE"
+
+
+def get_env_name_custom_matlab_root():
+    """User specified path to MATLAB root"""
+    return "MWI_CUSTOM_MATLAB_ROOT"
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/exceptions.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/exceptions.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/logger.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/logger.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/token_auth.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/token_auth.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/mwi/validators.py` & `matlab-proxy-0.7.2/matlab_proxy/util/mwi/validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 """This file contains validators for various runtime artefacts.
 A validator is defined as a function which verifies the input and 
 returns it unchanged if validation passes. 
 Returning inputs allows validators to be used inline with the input.
 
 Example: 
 Original code: if( input ):
@@ -10,23 +10,31 @@
 
 Exceptions are thrown to signal failure.
 """
 import errno
 import os
 import socket
 import sys
+from pathlib import Path
+
+from typing import List
 
 import pkg_resources
 
 import matlab_proxy
+from matlab_proxy.constants import VERSION_INFO_FILE_NAME
 
 from . import environment_variables as mwi_env
 from matlab_proxy.util import system
 from . import logger as mwi_logger
 
+from matlab_proxy import util
+
+from .exceptions import MatlabError
+
 logger = mwi_logger.get()
 
 
 def validate_mlm_license_file(nlm_connections_str):
     """Validates and returns input if it passes validation.
     Throws exception when validation fails.
     The connection string should be in the form of port@hostname
@@ -272,7 +280,55 @@
     Args:
         use_existing_license (str): value from the environment variable MWI_USE_EXISTING_LICENSE
 
     Returns:
         bool: if use_existing_license is set to true
     """
     return True if use_existing_license.casefold() == "true" else False
+
+
+def validate_paths(paths: List[Path]):
+    """Validates if  paths of directories or files exists on the file system.
+
+    Args:
+        paths ([pathlib.Path]): List of pathlib.Path's to directories or files
+
+    Raises:
+        OSError: When an invalid path is supplied
+
+    Returns:
+        [pathlib.Path] | None: [pathlib.Path] if valid paths are supplied else None
+    """
+    for path in paths:
+        if not util.is_valid_path(path):
+            raise OSError(f"Supplied invalid path:{path}")
+
+    return paths
+
+
+def validate_custom_matlab_root_path(matlab_root: Path):
+    """Validate if path supplied is MATLAB_ROOT by checking for the existence of VersionInfo.xml file
+    at matlab_root
+
+    Args:
+        path (pathlib.Path): path to MATLAB root
+
+    Returns:
+        pathlib.Path | None: pathlib.Path if a valid path to MATLAB root is supplied else None
+    """
+    try:
+        matlab_root = matlab_root
+        validate_paths([matlab_root])
+        logger.debug(f"Supplied valid MATLAB root path:{matlab_root}")
+    except OSError as exc:
+        logger.error(". ".join(exc.args))
+        sys.exit(1)
+
+    version_info_file_path = matlab_root / VERSION_INFO_FILE_NAME
+
+    if not version_info_file_path.is_file():
+        logger.error(
+            f" {VERSION_INFO_FILE_NAME} file doesn't exist at the provided path :{matlab_root}"
+        )
+        sys.exit(1)
+
+    return matlab_root
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/system.py` & `matlab-proxy-0.7.2/matlab_proxy/util/system.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy/util/windows.py` & `matlab-proxy-0.7.2/matlab_proxy/util/windows.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/matlab_proxy.egg-info/PKG-INFO` & `matlab-proxy-0.7.2/matlab_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.7.0
+Version: 0.7.2
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
```

### Comparing `matlab-proxy-0.7.0/matlab_proxy.egg-info/SOURCES.txt` & `matlab-proxy-0.7.2/matlab_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.0/setup.py` & `matlab-proxy-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 INSTALL_REQUIRES = ["aiohttp>=3.7.4", "psutil", "aiohttp_session[secure]"]
 
 HERE = Path(__file__).parent.resolve()
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="matlab-proxy",
-    version="0.7.0",
+    version="0.7.2",
     url=config["doc_url"],
     author="The MathWorks, Inc.",
     author_email="cloud@mathworks.com",
     license="MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE",
     description="Python® package enables you to launch MATLAB® and access it from a web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

