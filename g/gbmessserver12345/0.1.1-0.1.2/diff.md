# Comparing `tmp/gbmessserver12345-0.1.1.tar.gz` & `tmp/gbmessserver12345-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbmessserver12345-0.1.1.tar", max compression
+gzip compressed data, was "gbmessserver12345-0.1.2.tar", last modified: Tue Jul 11 18:57:26 2023, max compression
```

## Comparing `gbmessserver12345-0.1.1.tar` & `gbmessserver12345-0.1.2.tar`

### file list

```diff
@@ -1,98 +1,69 @@
--rw-r--r--   0        0        0     2259 2023-07-11 10:12:25.263251 gbmessserver12345-0.1.1/README.rst
--rw-r--r--   0        0        0     2215 2023-07-11 14:19:36.029200 gbmessserver12345-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-11 13:05:06.924997 gbmessserver12345-0.1.1/src/gbmessserver12345/__init__.py
--rw-r--r--   0        0        0       90 2023-07-11 09:12:58.151577 gbmessserver12345-0.1.1/src/gbmessserver12345/common/__init__.py
--rw-r--r--   0        0        0      304 2023-07-11 09:12:58.607578 gbmessserver12345-0.1.1/src/gbmessserver12345/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       97 2023-07-10 15:58:18.271767 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__init__.py
--rw-r--r--   0        0        0     3524 2023-07-10 15:58:18.295768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/JIM.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-07-10 18:30:11.112372 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1768 2023-07-11 13:40:39.480768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/descriptors.cpython-39.pyc
--rw-r--r--   0        0        0     4852 2023-07-11 13:40:39.488768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/endpoints.cpython-39.pyc
--rw-r--r--   0        0        0     4112 2023-07-10 18:30:11.116372 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     3687 2023-07-10 18:30:11.404364 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/metaclasses.cpython-39.pyc
--rw-r--r--   0        0        0     6131 2023-07-11 13:40:39.716769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/protocol.cpython-39.pyc
--rw-r--r--   0        0        0     8997 2023-07-11 13:40:39.736769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/security.cpython-39.pyc
--rw-r--r--   0        0        0     1936 2023-07-10 15:58:18.323768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/__pycache__/serializers.cpython-39.pyc
--rw-r--r--   0        0        0     1167 2023-07-11 13:34:14.770541 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/descriptors.py
--rw-r--r--   0        0        0     3881 2023-07-11 13:34:14.798542 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/endpoints.py
--rw-r--r--   0        0        0     2297 2023-07-10 15:58:18.323768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/errors.py
--rw-r--r--   0        0        0     4340 2023-07-10 15:58:18.323768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/metaclasses.py
--rw-r--r--   0        0        0       57 2023-07-10 15:58:18.323768 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/__init__.py
--rw-r--r--   0        0        0      287 2023-07-10 18:30:11.156371 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10691 2023-07-11 13:37:41.747943 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/__pycache__/message.cpython-39.pyc
--rw-r--r--   0        0        0     1331 2023-07-10 15:58:18.347769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/__pycache__/observer.cpython-39.pyc
--rw-r--r--   0        0        0      935 2023-07-10 18:30:11.312366 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     5790 2023-07-11 13:34:14.710541 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/message.py
--rw-r--r--   0        0        0      501 2023-07-10 15:58:18.347769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/user.py
--rw-r--r--   0        0        0     7561 2023-07-11 13:34:14.890542 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/protocol.py
--rw-r--r--   0        0        0     8805 2023-07-11 13:34:14.798542 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/security.py
--rw-r--r--   0        0        0      103 2023-07-10 15:58:18.351769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/__init__.py
--rw-r--r--   0        0        0      339 2023-07-10 18:30:11.368365 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6297 2023-07-11 13:40:39.780769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/__pycache__/message.cpython-39.pyc
--rw-r--r--   0        0        0     1384 2023-07-11 13:40:39.792769 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     6171 2023-07-11 13:34:14.546539 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/message.py
--rw-r--r--   0        0        0     1197 2023-07-11 13:34:14.578540 gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/user.py
--rw-r--r--   0        0        0       32 2023-07-10 15:58:42.036181 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__init__.py
--rw-r--r--   0        0        0      252 2023-07-10 18:30:11.116372 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1375 2023-07-11 09:20:20.007174 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/debug_decorators.cpython-39.pyc
--rw-r--r--   0        0        0     1613 2023-07-10 15:58:42.072182 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/descriptors.cpython-39.pyc
--rw-r--r--   0        0        0     1403 2023-07-10 15:58:42.072182 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     2242 2023-07-10 15:58:42.080182 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/metaclasses.cpython-39.pyc
--rw-r--r--   0        0        0     1953 2023-07-10 18:30:11.116372 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/observer.cpython-39.pyc
--rw-r--r--   0        0        0     1109 2023-07-10 18:30:11.404364 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/__pycache__/security.cpython-39.pyc
--rw-r--r--   0        0        0      871 2023-07-10 15:58:42.092182 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/debug_decorators.py
--rw-r--r--   0        0        0     1075 2023-07-10 15:58:42.092182 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/observer.py
--rw-r--r--   0        0        0      729 2023-07-10 15:58:42.092182 gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/security.py
--rw-r--r--   0        0        0       69 2023-07-10 14:31:52.338629 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__init__.py
--rw-r--r--   0        0        0      283 2023-07-11 06:11:00.386636 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4437 2023-07-11 13:40:39.900770 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__pycache__/app.cpython-39.pyc
--rw-r--r--   0        0        0     1692 2023-07-11 13:40:39.916770 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0        0        0     1824 2023-07-11 13:40:39.920770 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0      900 2023-07-11 06:11:00.726635 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     1759 2023-07-11 06:11:00.782634 gbmessserver12345-0.1.1/src/gbmessserver12345/server/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     5978 2023-07-11 13:33:19.166058 gbmessserver12345-0.1.1/src/gbmessserver12345/server/app.py
--rw-r--r--   0        0        0     1129 2023-07-11 13:33:24.718108 gbmessserver12345-0.1.1/src/gbmessserver12345/server/cli.py
--rw-r--r--   0        0        0     1569 2023-07-11 13:33:38.062228 gbmessserver12345-0.1.1/src/gbmessserver12345/server/config.py
--rw-r--r--   0        0        0      134 2023-07-10 14:31:52.342630 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__init__.py
--rw-r--r--   0        0        0      360 2023-07-10 18:30:11.116372 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3053 2023-07-11 13:40:40.096770 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/app.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2023-07-11 13:40:40.104771 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/auth.cpython-39.pyc
--rw-r--r--   0        0        0     9262 2023-07-11 13:40:40.108770 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/client_session.cpython-39.pyc
--rw-r--r--   0        0        0     1065 2023-07-10 18:30:11.156371 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     2132 2023-07-11 13:40:40.132771 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     2742 2023-07-11 13:40:40.140771 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/serializers.cpython-39.pyc
--rw-r--r--   0        0        0     3297 2023-07-11 13:40:40.236771 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/__pycache__/session_manager.cpython-39.pyc
--rw-r--r--   0        0        0     4318 2023-07-11 13:34:14.478539 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/app.py
--rw-r--r--   0        0        0      952 2023-07-11 13:34:14.666540 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/auth.py
--rw-r--r--   0        0        0    12655 2023-07-11 13:34:14.490539 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/client_session.py
--rw-r--r--   0        0        0      296 2023-07-10 14:31:52.358631 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/errors.py
--rw-r--r--   0        0        0     1309 2023-07-11 13:34:14.642540 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/model.py
--rw-r--r--   0        0        0     2236 2023-07-11 13:34:14.478539 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/serializers.py
--rw-r--r--   0        0        0     2549 2023-07-11 13:34:00.410421 gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/session_manager.py
--rw-r--r--   0        0        0       55 2023-07-10 14:31:52.358631 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__init__.py
--rw-r--r--   0        0        0      279 2023-07-10 18:30:11.160371 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1552 2023-07-11 13:40:40.256771 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-07-10 18:30:11.352365 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4262 2023-07-09 13:53:16.961524 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/message_view.cpython-39.pyc
--rw-r--r--   0        0        0     6566 2023-07-11 08:01:30.118399 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     4236 2023-07-07 14:34:56.420673 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/user_session_view.cpython-39.pyc
--rw-r--r--   0        0        0     7361 2023-07-08 07:49:32.640137 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/user_view.cpython-39.pyc
--rw-r--r--   0        0        0    13548 2023-07-11 13:40:41.584776 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/__pycache__/view.cpython-39.pyc
--rw-r--r--   0        0        0      721 2023-07-11 13:33:30.918164 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/config.py
--rw-r--r--   0        0        0      650 2023-07-10 14:31:52.366631 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/errors.py
--rw-r--r--   0        0        0     5596 2023-07-11 08:01:07.550337 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/model.py
--rw-r--r--   0        0        0    14564 2023-07-11 13:33:33.546188 gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/view.py
--rw-r--r--   0        0        0      368 2023-07-10 14:31:52.366631 gbmessserver12345-0.1.1/src/gbmessserver12345/server/errors.py
--rw-r--r--   0        0        0      115 2023-07-10 14:31:52.366631 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/__init__.py
--rw-r--r--   0        0        0      340 2023-07-10 18:30:11.416363 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2589 2023-07-11 13:40:41.616776 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/__pycache__/app.cpython-39.pyc
--rw-r--r--   0        0        0     3240 2023-07-11 13:40:41.664777 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/__pycache__/controller.cpython-39.pyc
--rw-r--r--   0        0        0     6457 2023-07-11 13:40:41.676777 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0    10293 2023-07-11 13:40:41.684777 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/__pycache__/view.cpython-39.pyc
--rw-r--r--   0        0        0     2387 2023-07-11 13:33:35.730207 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/app.py
--rw-r--r--   0        0        0     2041 2023-07-11 13:33:54.190369 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/controller.py
--rw-r--r--   0        0        0     5159 2023-07-11 13:33:51.490345 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/model.py
--rw-r--r--   0        0        0    13988 2023-07-11 13:33:45.926297 gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/view.py
--rw-r--r--   0        0        0     1791 2023-07-10 14:31:52.382632 gbmessserver12345-0.1.1/src/gbmessserver12345/server/logger.py
--rw-r--r--   0        0        0     1710 2023-07-11 13:33:16.014029 gbmessserver12345-0.1.1/src/gbmessserver12345/server.py
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 gbmessserver12345-0.1.1/PKG-INFO
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.255255 gbmessserver12345-0.1.2/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2548 2023-07-11 18:57:26.255255 gbmessserver12345-0.1.2/PKG-INFO
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2259 2023-07-11 10:12:25.000000 gbmessserver12345-0.1.2/README.rst
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      970 2023-07-11 18:56:03.000000 gbmessserver12345-0.1.2/pyproject.toml
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      298 2023-07-11 18:57:26.255255 gbmessserver12345-0.1.2/setup.cfg
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.247255 gbmessserver12345-0.1.2/src/
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.247255 gbmessserver12345-0.1.2/src/gbmessserver12345/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       69 2023-07-11 13:05:06.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/__init__.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.247255 gbmessserver12345-0.1.2/src/gbmessserver12345/common/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       90 2023-07-11 09:12:58.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/__init__.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.251255 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       97 2023-07-10 15:58:18.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1185 2023-07-11 18:32:42.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/descriptors.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     3917 2023-07-11 18:33:17.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/endpoints.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2297 2023-07-10 15:58:18.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/errors.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     4340 2023-07-10 15:58:18.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/metaclasses.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.251255 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/model/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       57 2023-07-10 15:58:18.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/model/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     5808 2023-07-11 18:31:59.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/model/message.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      501 2023-07-10 15:58:18.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/model/user.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     7615 2023-07-11 18:33:44.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/protocol.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     8841 2023-07-11 18:34:01.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/security.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.251255 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/serializers/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      103 2023-07-10 15:58:18.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/serializers/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     6189 2023-07-11 18:32:23.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/serializers/message.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1233 2023-07-11 18:32:33.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/serializers/user.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.251255 gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       32 2023-07-10 15:58:42.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      871 2023-07-10 15:58:42.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/debug_decorators.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1075 2023-07-10 15:58:42.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/observer.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      729 2023-07-10 15:58:42.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/security.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.251255 gbmessserver12345-0.1.2/src/gbmessserver12345/server/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       69 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     6086 2023-07-11 18:40:58.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/app.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1201 2023-07-11 18:41:13.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/cli.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1605 2023-07-11 18:41:29.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/config.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.251255 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      134 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     4390 2023-07-11 18:35:13.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/app.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1024 2023-07-11 18:35:30.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/auth.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)    12817 2023-07-11 18:36:41.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/client_session.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      296 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/errors.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1327 2023-07-11 18:37:00.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/model.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2308 2023-07-11 18:37:22.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/serializers.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2621 2023-07-11 18:37:39.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/session_manager.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.255255 gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       55 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      739 2023-07-11 18:37:51.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/config.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      650 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/errors.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     5579 2023-07-11 18:38:15.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/model.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)    14672 2023-07-11 18:38:45.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/view.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      368 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/errors.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.255255 gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)      115 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/__init__.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2476 2023-07-11 18:39:22.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/app.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2095 2023-07-11 18:39:41.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/controller.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     5303 2023-07-11 18:40:16.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/model.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)    14060 2023-07-11 18:40:38.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/view.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1791 2023-07-10 14:31:52.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server/logger.py
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     1764 2023-07-11 16:07:16.000000 gbmessserver12345-0.1.2/src/gbmessserver12345/server.py
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.247255 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2548 2023-07-11 18:57:26.000000 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/PKG-INFO
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     2362 2023-07-11 18:57:26.000000 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)        1 2023-07-11 18:57:26.000000 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)        1 2023-07-11 18:57:25.000000 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/not-zip-safe
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       55 2023-07-11 18:57:26.000000 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/requires.txt
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)       18 2023-07-11 18:57:26.000000 gbmessserver12345-0.1.2/src/gbmessserver12345.egg-info/top_level.txt
+drwxrwxr-x   0 ivanst    (1000) ivanst    (1000)        0 2023-07-11 18:57:26.255255 gbmessserver12345-0.1.2/test/
+-rw-rw-r--   0 ivanst    (1000) ivanst    (1000)     4586 2023-07-11 18:30:14.000000 gbmessserver12345-0.1.2/test/test_common.py
```

### Comparing `gbmessserver12345-0.1.1/README.rst` & `gbmessserver12345-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/descriptors.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/descriptors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Дескрипторы """
 import socket
 
-from common.transport.errors import EndpointParamError
+from gbmessserver12345.common.transport.errors import EndpointParamError
 
 
 class EndpointPort:
     min_value = 1024
     max_value = 65535
 
     def __set__(self, instance, value):
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/endpoints.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Классы-абстракции для обеспечения передачи данных"""
 import socket
 
-from common.transport.errors import (
+from gbmessserver12345.common.transport.errors import (
     EndpointCommunicationError,
     EndpointTimeout,
 )
-from common.transport.metaclasses import (
+from gbmessserver12345.common.transport.metaclasses import (
     EndpointVerifier,
     ClientEndpointVerifier,
     ServerEndpointVerifier,
 )
 
 MESSAGE_MAX_SIZE = 4096
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/errors.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/errors.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/metaclasses.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/metaclasses.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/model/message.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/model/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Сообщения протокола.
 
 Под сообщением здесь понимаем любой запрос (action/auth) и ответ (response)
 """
 
 from typing import List, Optional
 
-from common.transport.errors import JIMValidationError
+from gbmessserver12345.common.transport.errors import JIMValidationError
 
 
 class JIMMessage:
     def __init__(self, msg_type):
         self._type = msg_type
 
     @property
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/protocol.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Протокол передачи сообщений (JIM)"""
 import json
 
-from common.transport.errors import *
-from common.transport.model.message import (
+from gbmessserver12345.common.transport.errors import *
+from gbmessserver12345.common.transport.model.message import (
     JIMAction,
     JIMActionAddContact,
     JIMActionDeleteContact,
     JIMActionExit,
     JIMActionGetContacts,
     JIMActionMessage,
     JIMActionPresence,
     JIMAuth,
     JIMMessage,
     JIMResponse,
 )
-from common.transport.serializers.message import (
+from gbmessserver12345.common.transport.serializers.message import (
     JIMActionAddDelContactSerializer,
     JIMActionGetContactsSerializer,
     JIMActionMessageSerializer,
     JIMAuthSerializer,
     JIMActionPresenceSerializer,
     JIMActionExitSerializer,
     JIMMessageSerializer,
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/security.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import hmac
 import os
 
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Random import get_random_bytes
 from Cryptodome.Cipher import AES, PKCS1_OAEP
 
-from common.utils.security import PasswordHash
-from common.transport.errors import (
+from gbmessserver12345.common.utils.security import PasswordHash
+from gbmessserver12345.common.transport.errors import (
     TransportSecurityAuthError,
     TransportSecurityNoSessionKeyError,
     TransportSecurityValidationError,
 )
 
 
 class TranportEncryption:
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/message.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/serializers/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from common.transport.model.message import *
+from gbmessserver12345.common.transport.model.message import *
 
 
 class JIMMessageSerializer:
     auth_action = "auth_action"
     data1 = "secret1"
     data2 = "secret2"
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/transport/serializers/user.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/transport/serializers/user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from common.transport.errors import JIMValidationError
-from common.transport.model.user import JIMUser
+from gbmessserver12345.common.transport.errors import JIMValidationError
+from gbmessserver12345.common.transport.model.user import JIMUser
 
 
 class JIMUserSerializer:
     @staticmethod
     def from_dict(us: dict) -> JIMUser:
         username = us.get(JIMUserSerializer.Const.username)
         is_active = us.get(JIMUserSerializer.Const.is_active) or False
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/debug_decorators.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/debug_decorators.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/observer.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/observer.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/common/utils/security.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/common/utils/security.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/app.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ Основное серверное приложение """
 import threading
 import time
 from copy import copy
 
-from server.config import ServerConfig
-from server.core.app import ServerCore
-from server.db.config import ServerStorage
-from server.errors import ServerNoDBError
-from server.gui.app import ServerGUI
-from server.logger import ServerLogger
+from gbmessserver12345.server.config import ServerConfig
+from gbmessserver12345.server.core.app import ServerCore
+from gbmessserver12345.server.db.config import ServerStorage
+from gbmessserver12345.server.errors import ServerNoDBError
+from gbmessserver12345.server.gui.app import ServerGUI
+from gbmessserver12345.server.logger import ServerLogger
 
 
 class ServerApp:
     """Server Application:
     Message dispatcher: client interaction thread (controller -> DB model, client sockets)
     GUI: Qt thread (reading view on DB & changing view on config model)
     Main thread: starts GUI and dispatcher in separate threads, config controller (restarts threads if config changed)
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/config.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Конфигурация сервера"""
 import os
 
 from sqlalchemy import URL
 
-from common.transport.descriptors import EndpointHost, EndpointPort
-from common.utils.observer import ObserverNotifier
+from gbmessserver12345.common.transport.descriptors import EndpointHost, EndpointPort
+from gbmessserver12345.common.utils.observer import ObserverNotifier
 
 SERVER_HOST_DEFAULT = "127.0.0.1"
 SERVER_PORT_DEFAULT = 7777
 
 SERVER_CONNECTION_LIMIT = 5
 SERVER_TIMEOUT = 0.5
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/app.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 Состояние моделей меняется соответствующими сетевыми сообщениями.
 """
 
 import select
 import threading
 
-from server.config import ServerConfig
-from server.core.session_manager import ClientSessionManager
-from server.db.config import ServerStorage
-from common.transport.endpoints import ServerEndpoint
+from gbmessserver12345.server.config import ServerConfig
+from gbmessserver12345.server.core.session_manager import ClientSessionManager
+from gbmessserver12345.server.db.config import ServerStorage
+from gbmessserver12345.common.transport.endpoints import ServerEndpoint
 
 
 class ServerCore:
     def __init__(self, logger, config: ServerConfig, db: ServerStorage):
         self.config = config
         self.logger = logger
         self.db = db
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/client_session.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/client_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """ Модуль для работы с подключенными клиентами """
 from abc import abstractmethod
 from functools import wraps
 from typing import List, Optional
-from server.core.auth import UserManager
 
-from server.core.errors import ServerCoreNotAuthorizedError
-from server.core.serializers import UserSessionSerializer
-from server.db.config import ServerStorage
-from server.db.view import (
+from gbmessserver12345.server.core.auth import UserManager
+from gbmessserver12345.server.core.errors import ServerCoreNotAuthorizedError
+from gbmessserver12345.server.core.serializers import UserSessionSerializer
+from gbmessserver12345.server.db.config import ServerStorage
+from gbmessserver12345.server.db.view import (
     MessageInfo,
     MessageView,
     UserSessionView,
     UserView,
-    UserAuthView,
 )
-from common.transport.errors import (
+from gbmessserver12345.common.transport.errors import (
     JIMSerializerError,
     TransportSecurityAuthError,
     TransportSecurityError,
 )
-from common.transport.model.message import *
-from common.transport.protocol import JIMSerializer
-from common.transport.serializers.user import JIMUserSerializer
-from common.transport.security import ServerSecurity
+from gbmessserver12345.common.transport.model.message import *
+from gbmessserver12345.common.transport.protocol import JIMSerializer
+from gbmessserver12345.common.transport.serializers.user import JIMUserSerializer
+from gbmessserver12345.common.transport.security import ServerSecurity
 
 
 class ClientSessionObserver:
     """Наблюдатель за сессией"""
 
     @abstractmethod
     def register_out_message(self, m_out: MessageInfo):
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/model.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Объектная модель сервера.
 
 Модель БД не подходит, т.к. распределена по нескольким таблицам
 """
 import datetime
 from typing import Optional
 
-from common.transport.model.message import JIMActionMessage
+from gbmessserver12345.common.transport.model.message import JIMActionMessage
 
 
 class UserInfo:
     def __init__(self, id, user: str, is_active: bool, status: Optional[str]) -> None:
         self.id = id
         self.user = user
         self.is_active = is_active
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/serializers.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Сериализаторы (БД/транспорт/сервер)"""
 import datetime
 
-from server.core.model import UserInfo, UserSessionInfo, MessageInfo
-from server.db.model import User, UserSession, Message
-from common.transport.model.message import JIMActionMessage
-from common.transport.model.user import JIMUser
+from gbmessserver12345.server.core.model import UserInfo, UserSessionInfo, MessageInfo
+from gbmessserver12345.server.db.model import User, UserSession, Message
+from gbmessserver12345.common.transport.model.message import JIMActionMessage
+from gbmessserver12345.common.transport.model.user import JIMUser
 
 
 class UserSerializer:
     """Пользователь"""
 
     @staticmethod
     def from_db(user: User) -> UserInfo:
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/core/session_manager.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/core/session_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Классы для хранения и управления клиентскими сессиями"""
 # Keeps & manages client sessions and interactions between them (Model/Mapper)
 from logging import Logger
 from typing import Dict, List, Optional
 
-from server.core.client_session import (
+from gbmessserver12345.server.core.client_session import (
     ClientSession,
     ClientSessionObserver,
 )
-from server.db.config import ServerStorage
-from server.db.view import UserSessionView, MessageInfo
-from common.transport.endpoints import Endpoint
+from gbmessserver12345.server.db.config import ServerStorage
+from gbmessserver12345.server.db.view import UserSessionView, MessageInfo
+from gbmessserver12345.common.transport.endpoints import Endpoint
 
 
 class ClientSessionManager(ClientSessionObserver):
     client_sessions: Dict[Endpoint, ClientSession]
 
     def __init__(self, logger: Logger, db: ServerStorage) -> None:
         self.client_sessions = dict()
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/config.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Конфигурация и общие функции для работы с БД"""
 import threading
 
 from sqlalchemy import create_engine
 
-from server.db.model import *
+from gbmessserver12345.server.db.model import *
 
 
 class ServerStorage:
     def __init__(self, db_url) -> None:
         self.db_engine = create_engine(db_url, echo=False, pool_recycle=7200)
         self.lock = threading.Lock()
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/errors.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/errors.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/model.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import datetime
 from typing import Annotated, List
 
 from sqlalchemy import (
     ForeignKey,
     Integer,
     String,
-    UnicodeText,
     Text,
     func,
 )
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 
 intpk = Annotated[
     int, mapped_column("id", Integer, primary_key=True, autoincrement=True)
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/db/view.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/db/view.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 """Методы для работы с данными пользователей"""
 import datetime
 from typing import List, Optional, Union
 
 from sqlalchemy import func, select
 from sqlalchemy.orm import Session
 
-from server.core.model import (
+from gbmessserver12345.server.core.model import (
     MessageInfo,
     UserInfo,
     UserSessionInfo,
     UserStatistic,
 )
-from server.core.serializers import (
+from gbmessserver12345.server.core.serializers import (
     MessageSerializer,
     UserSerializer,
     UserSessionSerializer,
 )
-from server.db.config import ServerDBBaseView, ServerStorage
-from server.db.errors import *
-from server.db.errors import (
+from gbmessserver12345.server.db.config import ServerDBBaseView, ServerStorage
+from gbmessserver12345.server.db.errors import *
+from gbmessserver12345.server.db.errors import (
     ServerDBError,
     ServerDBUserAlreadyExists,
     ServerDBUserNotExists,
 )
-from server.db.model import (
+from gbmessserver12345.server.db.model import (
     Message,
     User,
     UserContact,
     UserPrivate,
     UserSession,
     UserStatus,
     extpk,
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/app.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """ Графический интерфейс сервера, запускается в отдельном треде"""
 import sys
 import threading
 
 from PyQt5.QtCore import QTimer
 from PyQt5.QtWidgets import QApplication
 
-from server.config import ServerConfig
-
-from server.db.config import ServerStorage
-from server.gui.controller import ServerGUIController
-from server.gui.model import (
+from gbmessserver12345.server.config import ServerConfig
+from gbmessserver12345.server.db.config import ServerStorage
+from gbmessserver12345.server.gui.controller import ServerGUIController
+from gbmessserver12345.server.gui.model import (
     ActiveUsersModel,
     SettingsModel,
     SingleSelectionModel,
     UserModel,
     UserStatisticsModel,
 )
-from server.gui.view import (
+from gbmessserver12345.server.gui.view import (
     MainWindow,
     SettingsWindow,
     StatisticsWindow,
     UserWindow,
 )
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/controller.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Обработка событий (сигналов) между окнами/приложением"""
 import threading
 
 from PyQt5.QtWidgets import QWidget, qApp
 
-from server.config import ServerConfig
-from server.gui.model import SettingsModel
-from common.utils.observer import ObserverNotifier
+from gbmessserver12345.server.config import ServerConfig
+from gbmessserver12345.server.gui.model import SettingsModel
+from gbmessserver12345.common.utils.observer import ObserverNotifier
 
 
 class ServerGUIController(ObserverNotifier):
     """Класс-бработчик событий (сигналов) между окнами/приложением"""
 
     def __init__(
         self,
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/model.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ Модели с данными для GUI. Т.к. в проекте исползуется SQLAlchemy, то это скорее интеграционная прослойка"""
 from copy import copy
 from typing import List, Optional
 
 from PyQt5.QtGui import QStandardItem, QStandardItemModel
 
-from server.config import ServerConfig
-from server.core.auth import UserManager
-from server.core.model import UserInfo
-from server.db.config import ServerStorage
-from server.db.view import MessageView, UserSessionView, UserView
-from common.transport.descriptors import EndpointPort
-from common.utils.observer import ObserverNotifier
-from common.utils.security import PasswordHash
+from gbmessserver12345.server.config import ServerConfig
+from gbmessserver12345.server.core.auth import UserManager
+from gbmessserver12345.server.core.model import UserInfo
+from gbmessserver12345.server.db.config import ServerStorage
+from gbmessserver12345.server.db.view import MessageView, UserSessionView, UserView
+from gbmessserver12345.common.transport.descriptors import EndpointPort
+from gbmessserver12345.common.utils.observer import ObserverNotifier
+from gbmessserver12345.common.utils.security import PasswordHash
 
 
 class ActiveUsersModel(QStandardItemModel):
     """Модель для таблицы активных пользователей"""
 
     def __init__(self, db: ServerStorage):
         super().__init__()
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/gui/view.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/gui/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     QMessageBox,
     QPushButton,
     QTableView,
     QVBoxLayout,
     QWidget,
 )
 
-from server.gui.controller import ServerGUIController
-from server.gui.model import (
+from gbmessserver12345.server.gui.controller import ServerGUIController
+from gbmessserver12345.server.gui.model import (
     ActiveUsersModel,
     SettingsModel,
     SingleSelectionModel,
     UserModel,
     UserStatisticsModel,
 )
-from common.transport.descriptors import EndpointPort
-from common.utils.observer import Observer
+from gbmessserver12345.common.transport.descriptors import EndpointPort
+from gbmessserver12345.common.utils.observer import Observer
 
 
 class MainWindow(QMainWindow, Observer):
     def __init__(self, model: ActiveUsersModel, controller: ServerGUIController):
         super().__init__()
         self.model = model
         self.controller = controller
```

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server/logger.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server/logger.py`

 * *Files identical despite different names*

### Comparing `gbmessserver12345-0.1.1/src/gbmessserver12345/server.py` & `gbmessserver12345-0.1.2/src/gbmessserver12345/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Модуль для запуска сервера"""
 import argparse
 import os
 
 
-from server.app import ServerApp
-from server.cli import ServerCLI
-from server.config import ServerConfig
+from gbmessserver12345.server.app import ServerApp
+from gbmessserver12345.server.cli import ServerCLI
+from gbmessserver12345.server.config import ServerConfig
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Server commands")
     parser.add_argument("-d", "--db_url", type=str, help="DB connect string")
     subparsers = parser.add_subparsers(
         title="subcommands",
         description="valid subcommands",
```

