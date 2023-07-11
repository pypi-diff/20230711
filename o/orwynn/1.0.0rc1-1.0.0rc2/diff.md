# Comparing `tmp/orwynn-1.0.0rc1.tar.gz` & `tmp/orwynn-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orwynn-1.0.0rc1.tar", max compression
+gzip compressed data, was "orwynn-1.0.0rc2.tar", max compression
```

## Comparing `orwynn-1.0.0rc1.tar` & `orwynn-1.0.0rc2.tar`

### file list

```diff
@@ -1,263 +1,276 @@
--rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0rc1/README.md
--rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0rc1/orwynn/__init__.py
--rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0rc1/orwynn/apiversion/__init__.py
--rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/apiversion/errors.py
--rw-r--r--   0        0        0     4546 2023-06-09 12:16:54.007732 orwynn-1.0.0rc1/orwynn/apiversion/test_main.py
--rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0rc1/orwynn/app/__init__.py
--rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0rc1/orwynn/app/apirouter.py
--rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0rc1/orwynn/app/apiwebsocketroute.py
--rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0rc1/orwynn/app/app.py
--rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0rc1/orwynn/app/config.py
--rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0rc1/orwynn/app/core.py
--rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0rc1/orwynn/app/mode.py
--rw-r--r--   0        0        0     2206 2023-06-08 13:47:49.295428 orwynn-1.0.0rc1/orwynn/app/test_main.py
--rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0rc1/orwynn/app/types.py
--rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0rc1/orwynn/app/utils.py
--rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0rc1/orwynn/apprc/__init__.py
--rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0rc1/orwynn/apprc/apprc.py
--rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0rc1/orwynn/apprc/constants.py
--rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/apprc/errors.py
--rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0rc1/orwynn/apprc/parse.py
--rw-r--r--   0        0        0     2604 2023-06-09 06:20:20.107768 orwynn-1.0.0rc1/orwynn/apprc/test_main.py
--rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0rc1/orwynn/base/__init__.py
--rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0rc1/orwynn/base/config/__init__.py
--rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0rc1/orwynn/base/config/config.py
--rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0rc1/orwynn/base/config/test_config.py
--rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0rc1/orwynn/base/controller/__init__.py
--rw-r--r--   0        0        0     2211 2023-07-06 09:35:56.327943 orwynn-1.0.0rc1/orwynn/base/controller/controller.py
--rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0rc1/orwynn/base/controller/errors.py
--rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0rc1/orwynn/base/database/__init__.py
--rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0rc1/orwynn/base/database/database.py
--rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0rc1/orwynn/base/database/errors.py
--rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0rc1/orwynn/base/error/__init__.py
--rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0rc1/orwynn/base/error/code.py
--rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0rc1/orwynn/base/error/errors.py
--rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0rc1/orwynn/base/error/test_main.py
--rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0rc1/orwynn/base/error/test_utils.py
--rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0rc1/orwynn/base/error/utils.py
--rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0rc1/orwynn/base/error/valueschema.py
--rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0rc1/orwynn/base/errorhandler/__init__.py
--rw-r--r--   0        0        0     2364 2023-07-06 10:24:26.021973 orwynn-1.0.0rc1/orwynn/base/errorhandler/errorhandler.py
--rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0rc1/orwynn/base/middleware/__init__.py
--rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0rc1/orwynn/base/middleware/globalsetup.py
--rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0rc1/orwynn/base/middleware/middleware.py
--rw-r--r--   0        0        0     1186 2023-06-09 06:20:20.112767 orwynn-1.0.0rc1/orwynn/base/middleware/test_main.py
--rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0rc1/orwynn/base/model/__init__.py
--rw-r--r--   0        0        0     1423 2023-07-06 09:10:08.307376 orwynn-1.0.0rc1/orwynn/base/model/model.py
--rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0rc1/orwynn/base/model/test_model.py
--rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0rc1/orwynn/base/module/__init__.py
--rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0rc1/orwynn/base/module/errors.py
--rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0rc1/orwynn/base/module/module.py
--rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0rc1/orwynn/base/module/test_module.py
--rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0rc1/orwynn/base/service/__init__.py
--rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0rc1/orwynn/base/service/framework.py
--rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0rc1/orwynn/base/service/service.py
--rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0rc1/orwynn/base/worker/__init__.py
--rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0rc1/orwynn/base/worker/worker.py
--rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0rc1/orwynn/boot/__init__.py
--rw-r--r--   0        0        0    10361 2023-07-06 10:25:59.036484 orwynn-1.0.0rc1/orwynn/boot/boot.py
--rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0rc1/orwynn/boot/config.py
--rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0rc1/orwynn/boot/errors.py
--rw-r--r--   0        0        0     4754 2023-06-09 06:27:59.920644 orwynn-1.0.0rc1/orwynn/boot/test_main.py
--rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0rc1/orwynn/bootscript/__init__.py
--rw-r--r--   0        0        0      220 2023-06-08 13:59:21.194248 orwynn-1.0.0rc1/orwynn/bootscript/bootscript.py
--rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0rc1/orwynn/bootscript/callable.py
--rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0rc1/orwynn/bootscript/calltime.py
--rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0rc1/orwynn/bootscript/errors.py
--rw-r--r--   0        0        0      860 2023-06-09 06:20:20.107768 orwynn-1.0.0rc1/orwynn/bootscript/test_main.py
--rw-r--r--   0        0        0     2300 2023-06-09 06:20:20.107768 orwynn-1.0.0rc1/orwynn/bootscript/worker.py
--rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0rc1/orwynn/context/__init__.py
--rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/context/errors.py
--rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0rc1/orwynn/context/manager.py
--rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0rc1/orwynn/context/storage.py
--rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0rc1/orwynn/di/__init__.py
--rw-r--r--   0        0        0       69 2023-07-06 09:39:22.689224 orwynn-1.0.0rc1/orwynn/di/acceptor.py
--rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0rc1/orwynn/di/availability.py
--rw-r--r--   0        0        0     1719 2023-06-09 06:20:20.108768 orwynn-1.0.0rc1/orwynn/di/collecting/acceptordependencies.py
--rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0rc1/orwynn/di/collecting/errors.py
--rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0rc1/orwynn/di/collecting/helpers.py
--rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0rc1/orwynn/di/collecting/modulecollector.py
--rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/collect.py
--rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/map.py
--rw-r--r--   0        0        0     1765 2023-06-09 06:20:20.109768 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/test_main.py
--rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0rc1/orwynn/di/collecting/test_modules.py
--rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0rc1/orwynn/di/constants.py
--rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0rc1/orwynn/di/container.py
--rw-r--r--   0        0        0     4694 2023-06-09 06:20:20.104768 orwynn-1.0.0rc1/orwynn/di/di.py
--rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0rc1/orwynn/di/errors.py
--rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0rc1/orwynn/di/init/acceptors.py
--rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0rc1/orwynn/di/init/providers.py
--rw-r--r--   0        0        0     2871 2023-06-09 06:20:20.106768 orwynn-1.0.0rc1/orwynn/di/init/test_acceptors.py
--rw-r--r--   0        0        0      615 2023-06-09 06:23:04.561666 orwynn-1.0.0rc1/orwynn/di/init/test_providers.py
--rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0rc1/orwynn/di/isacceptor.py
--rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0rc1/orwynn/di/isprovider.py
--rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0rc1/orwynn/di/object.py
--rw-r--r--   0        0        0       45 2023-07-06 09:39:13.705327 orwynn-1.0.0rc1/orwynn/di/provider.py
--rw-r--r--   0        0        0      506 2023-06-09 06:20:20.105768 orwynn-1.0.0rc1/orwynn/di/testing.py
--rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0rc1/orwynn/helpers/constants.py
--rw-r--r--   0        0        0      455 2023-07-04 11:25:22.457577 orwynn-1.0.0rc1/orwynn/helpers/errors.py
--rw-r--r--   0        0        0     1140 2023-06-09 06:03:10.090856 orwynn-1.0.0rc1/orwynn/helpers/web.py
--rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0rc1/orwynn/http/__init__.py
--rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0rc1/orwynn/http/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0rc1/orwynn/http/context/__init__.py
--rw-r--r--   0        0        0      959 2023-07-05 09:50:46.449134 orwynn-1.0.0rc1/orwynn/http/context/id.py
--rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0rc1/orwynn/http/context/middleware/builtin.py
--rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0rc1/orwynn/http/context/middleware/contextbuiltin.py
--rw-r--r--   0        0        0      984 2023-06-09 06:27:59.920644 orwynn-1.0.0rc1/orwynn/http/context/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0rc1/orwynn/http/controller/__init__.py
--rw-r--r--   0        0        0     5446 2023-06-09 06:03:10.090856 orwynn-1.0.0rc1/orwynn/http/controller/controller.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/__init__.py
--rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/container.py
--rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/endpoint.py
--rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/response.py
--rw-r--r--   0        0        0     2231 2023-06-08 13:56:18.457476 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/test_main.py
--rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/http/controller/errors.py
--rw-r--r--   0        0        0     7262 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/http/controller/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0rc1/orwynn/http/cors/__init__.py
--rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0rc1/orwynn/http/cors/cors.py
--rw-r--r--   0        0        0     3491 2023-06-09 12:32:20.369783 orwynn-1.0.0rc1/orwynn/http/cors/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0rc1/orwynn/http/errorhandler/__init__.py
--rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0rc1/orwynn/http/errorhandler/default.py
--rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0rc1/orwynn/http/errorhandler/middleware.py
--rw-r--r--   0        0        0     6129 2023-06-09 07:32:02.382043 orwynn-1.0.0rc1/orwynn/http/errorhandler/test_main.py
--rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0rc1/orwynn/http/errors.py
--rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0rc1/orwynn/http/log/logger.py
--rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0rc1/orwynn/http/log/middleware.py
--rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0rc1/orwynn/http/middleware/__init__.py
--rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0rc1/orwynn/http/middleware/builtinmiddleware.py
--rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0rc1/orwynn/http/middleware/middleware.py
--rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0rc1/orwynn/http/middleware/nextcall.py
--rw-r--r--   0        0        0     2150 2023-06-09 06:00:41.008691 orwynn-1.0.0rc1/orwynn/http/middleware/test_main.py
--rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0rc1/orwynn/http/requests.py
--rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0rc1/orwynn/http/responses.py
--rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0rc1/orwynn/http/schema/validationvalue.py
--rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0rc1/orwynn/http/schema/value.py
--rw-r--r--   0        0        0      873 2023-06-09 05:50:36.425514 orwynn-1.0.0rc1/orwynn/http/test_responses.py
--rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0rc1/orwynn/http/testing.py
--rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/indication/__init__.py
--rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0rc1/orwynn/indication/default.py
--rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/indication/errors.py
--rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0rc1/orwynn/indication/indicatable.py
--rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0rc1/orwynn/indication/indication.py
--rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0rc1/orwynn/indication/indicator.py
--rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0rc1/orwynn/indication/test_main.py
--rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0rc1/orwynn/indication/type.py
--rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0rc1/orwynn/log/__init__.py
--rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0rc1/orwynn/log/config.py
--rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0rc1/orwynn/log/configure.py
--rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0rc1/orwynn/log/constants.py
--rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/log/errors.py
--rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0rc1/orwynn/log/handler.py
--rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0rc1/orwynn/log/helpers.py
--rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0rc1/orwynn/log/log.py
--rw-r--r--   0        0        0     1767 2023-06-09 07:50:09.129655 orwynn-1.0.0rc1/orwynn/log/test_main.py
--rw-r--r--   0        0        0     3679 2023-06-09 06:00:41.008691 orwynn-1.0.0rc1/orwynn/log/test_middleware.py
--rw-r--r--   0        0        0     1443 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/log/test_websocketmiddleware.py
--rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0rc1/orwynn/log/types.py
--rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0rc1/orwynn/mapping/__init__.py
--rw-r--r--   0        0        0      667 2023-07-05 09:49:27.438110 orwynn-1.0.0rc1/orwynn/mapping/errors.py
--rw-r--r--   0        0        0     1808 2023-07-05 09:47:23.970713 orwynn-1.0.0rc1/orwynn/mapping/mapping.py
--rw-r--r--   0        0        0      504 2023-07-05 09:49:15.096266 orwynn-1.0.0rc1/orwynn/mapping/test_main.py
--rw-r--r--   0        0        0      216 2023-07-04 11:01:21.049070 orwynn-1.0.0rc1/orwynn/mongo/__init__.py
--rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0rc1/orwynn/mongo/clientsession.py
--rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0rc1/orwynn/mongo/config.py
--rw-r--r--   0        0        0     7634 2023-07-06 08:54:40.455677 orwynn-1.0.0rc1/orwynn/mongo/document/__init__.py
--rw-r--r--   0        0        0      578 2023-07-06 07:33:03.897136 orwynn-1.0.0rc1/orwynn/mongo/document/errors.py
--rw-r--r--   0        0        0     1134 2023-07-05 09:33:28.956933 orwynn-1.0.0rc1/orwynn/mongo/document/helpers.py
--rw-r--r--   0        0        0     1367 2023-07-05 09:33:28.955933 orwynn-1.0.0rc1/orwynn/mongo/document/test_converttoobjectid.py
--rw-r--r--   0        0        0      219 2023-07-06 06:48:26.581243 orwynn-1.0.0rc1/orwynn/mongo/document/test_create.py
--rw-r--r--   0        0        0      742 2023-07-06 07:53:44.416182 orwynn-1.0.0rc1/orwynn/mongo/document/test_get.py
--rw-r--r--   0        0        0      703 2023-07-06 08:55:42.984735 orwynn-1.0.0rc1/orwynn/mongo/document/test_inc.py
--rw-r--r--   0        0        0      275 2023-07-06 07:46:04.044931 orwynn-1.0.0rc1/orwynn/mongo/document/test_refresh.py
--rw-r--r--   0        0        0      230 2023-07-06 06:48:10.593442 orwynn-1.0.0rc1/orwynn/mongo/document/test_remove.py
--rw-r--r--   0        0        0      829 2023-07-06 08:55:42.984735 orwynn-1.0.0rc1/orwynn/mongo/document/test_set.py
--rw-r--r--   0        0        0     1312 2023-07-06 07:42:00.340990 orwynn-1.0.0rc1/orwynn/mongo/document/test_updateoperators.py
--rw-r--r--   0        0        0      708 2023-07-06 08:51:37.969595 orwynn-1.0.0rc1/orwynn/mongo/document/testing.py
--rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0rc1/orwynn/mongo/entity.py
--rw-r--r--   0        0        0      882 2023-07-05 09:49:15.103266 orwynn-1.0.0rc1/orwynn/mongo/errors.py
--rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0rc1/orwynn/mongo/mongo.py
--rw-r--r--   0        0        0     1354 2023-07-04 11:01:22.010065 orwynn-1.0.0rc1/orwynn/mongo/test_main.py
--rw-r--r--   0        0        0      395 2023-07-06 07:28:27.154203 orwynn-1.0.0rc1/orwynn/mongo/testing.py
--rw-r--r--   0        0        0     2839 2023-06-09 06:03:10.133848 orwynn-1.0.0rc1/orwynn/proxy/boot.py
--rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0rc1/orwynn/proxy/indicationonly.py
--rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0rc1/orwynn/router/__init__.py
--rw-r--r--   0        0        0     3966 2023-06-09 06:23:57.815708 orwynn-1.0.0rc1/orwynn/router/errorhandlermanager.py
--rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/router/errors.py
--rw-r--r--   0        0        0    14259 2023-06-09 06:03:10.133848 orwynn-1.0.0rc1/orwynn/router/register/controller.py
--rw-r--r--   0        0        0     9656 2023-06-09 11:05:03.703488 orwynn-1.0.0rc1/orwynn/router/register/middleware.py
--rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0rc1/orwynn/router/router.py
--rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0rc1/orwynn/router/test_globalroute.py
--rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0rc1/orwynn/singleton/__init__.py
--rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0rc1/orwynn/singleton/singleton.py
--rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0rc1/orwynn/sql/__init__.py
--rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0rc1/orwynn/sql/config.py
--rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0rc1/orwynn/sql/databasekind.py
--rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0rc1/orwynn/sql/poolclass.py
--rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0rc1/orwynn/sql/sql.py
--rw-r--r--   0        0        0     2636 2023-07-05 09:50:46.449134 orwynn-1.0.0rc1/orwynn/sql/table.py
--rw-r--r--   0        0        0     5855 2023-06-09 06:20:20.114767 orwynn-1.0.0rc1/orwynn/sql/test_main.py
--rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0rc1/orwynn/testing/__init__.py
--rw-r--r--   0        0        0    11299 2023-06-09 07:32:18.165326 orwynn-1.0.0rc1/orwynn/testing/client.py
--rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0rc1/orwynn/testing/embeddedclient.py
--rw-r--r--   0        0        0     2046 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/testing/test_main.py
--rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0rc1/orwynn/testingtools/__init__.py
--rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0rc1/orwynn/utils/basesubclassable.py
--rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0rc1/orwynn/utils/crypto/__init__.py
--rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0rc1/orwynn/utils/dt/__init__.py
--rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0rc1/orwynn/utils/fmt/__init__.py
--rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0rc1/orwynn/utils/fmt/test_main.py
--rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0rc1/orwynn/utils/klass/__init__.py
--rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0rc1/orwynn/utils/klass/errors.py
--rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0rc1/orwynn/utils/klass/test_klass.py
--rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0rc1/orwynn/utils/mp/__init__.py
--rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0rc1/orwynn/utils/mp/dictpp.py
--rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0rc1/orwynn/utils/mp/location.py
--rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0rc1/orwynn/utils/mp/test_main.py
--rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0rc1/orwynn/utils/protocol.py
--rw-r--r--   0        0        0      131 2023-07-05 09:50:46.441135 orwynn-1.0.0rc1/orwynn/utils/rnd/__init__.py
--rw-r--r--   0        0        0       90 2023-07-05 09:50:46.449134 orwynn-1.0.0rc1/orwynn/utils/rnd/test_main.py
--rw-r--r--   0        0        0      376 2023-07-05 09:14:52.810766 orwynn-1.0.0rc1/orwynn/utils/types.py
--rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0rc1/orwynn/utils/uio.py
--rw-r--r--   0        0        0      682 2023-06-09 06:02:47.709865 orwynn-1.0.0rc1/orwynn/utils/url/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0rc1/orwynn/utils/url/helpers.py
--rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0rc1/orwynn/utils/url/test_utils.py
--rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0rc1/orwynn/utils/url/url.py
--rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0rc1/orwynn/utils/url/utils.py
--rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0rc1/orwynn/utils/url/vars.py
--rw-r--r--   0        0        0     9150 2023-06-09 06:02:55.428511 orwynn-1.0.0rc1/orwynn/utils/validation/__init__.py
--rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0rc1/orwynn/utils/validation/errors.py
--rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0rc1/orwynn/utils/validation/validator.py
--rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0rc1/orwynn/utils/yml/__init__.py
--rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/utils/yml/errors.py
--rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0rc1/orwynn/websocket/__init__.py
--rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0rc1/orwynn/websocket/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0rc1/orwynn/websocket/context/__init__.py
--rw-r--r--   0        0        0     1028 2023-07-05 09:50:46.450135 orwynn-1.0.0rc1/orwynn/websocket/context/id.py
--rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0rc1/orwynn/websocket/context/middleware/builtin.py
--rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0rc1/orwynn/websocket/context/middleware/contextbuiltin.py
--rw-r--r--   0        0        0     1241 2023-06-09 06:27:59.917644 orwynn-1.0.0rc1/orwynn/websocket/context/test_main.py
--rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0rc1/orwynn/websocket/controller/controller.py
--rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0rc1/orwynn/websocket/controller/eventhandlermethod.py
--rw-r--r--   0        0        0     3806 2023-06-09 07:21:01.679769 orwynn-1.0.0rc1/orwynn/websocket/controller/test_controller.py
--rw-r--r--   0        0        0     2888 2023-06-09 06:20:10.147480 orwynn-1.0.0rc1/orwynn/websocket/controller/test_globalroute.py
--rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0rc1/orwynn/websocket/errorhandler/default.py
--rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0rc1/orwynn/websocket/errorhandler/middleware.py
--rw-r--r--   0        0        0     1699 2023-06-09 06:03:10.090856 orwynn-1.0.0rc1/orwynn/websocket/errorhandler/test_default.py
--rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0rc1/orwynn/websocket/log/logger.py
--rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/websocket/log/middleware.py
--rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/websocket/middleware/builtin.py
--rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/websocket/middleware/connectionbuiltin.py
--rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0rc1/orwynn/websocket/middleware/middleware.py
--rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0rc1/orwynn/websocket/middleware/nextcall.py
--rw-r--r--   0        0        0     1053 2023-06-09 06:27:59.918644 orwynn-1.0.0rc1/orwynn/websocket/middleware/test_main.py
--rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0rc1/orwynn/websocket/routing/dispatchfn.py
--rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0rc1/orwynn/websocket/routing/genericfn.py
--rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0rc1/orwynn/websocket/routing/handlers.py
--rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0rc1/orwynn/websocket/routing/helpers.py
--rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0rc1/orwynn/websocket/routing/nextcall.py
--rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0rc1/orwynn/websocket/routing/stack.py
--rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0rc1/orwynn/websocket/websocket.py
--rw-r--r--   0        0        0      928 2023-07-06 10:45:11.657758 orwynn-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 orwynn-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0rc2/README.md
+-rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0rc2/orwynn/__init__.py
+-rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0rc2/orwynn/apiversion/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/apiversion/errors.py
+-rw-r--r--   0        0        0     4873 2023-07-10 13:45:40.443311 orwynn-1.0.0rc2/orwynn/apiversion/test_main.py
+-rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0rc2/orwynn/app/__init__.py
+-rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0rc2/orwynn/app/apirouter.py
+-rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0rc2/orwynn/app/apiwebsocketroute.py
+-rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0rc2/orwynn/app/app.py
+-rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0rc2/orwynn/app/config.py
+-rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0rc2/orwynn/app/core.py
+-rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0rc2/orwynn/app/mode.py
+-rw-r--r--   0        0        0     2367 2023-07-10 13:45:40.440312 orwynn-1.0.0rc2/orwynn/app/test_main.py
+-rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0rc2/orwynn/app/types.py
+-rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0rc2/orwynn/app/utils.py
+-rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0rc2/orwynn/apprc/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0rc2/orwynn/apprc/apprc.py
+-rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0rc2/orwynn/apprc/constants.py
+-rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/apprc/errors.py
+-rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0rc2/orwynn/apprc/parse.py
+-rw-r--r--   0        0        0     2724 2023-07-10 12:01:27.295418 orwynn-1.0.0rc2/orwynn/apprc/test_main.py
+-rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0rc2/orwynn/base/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0rc2/orwynn/base/config/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0rc2/orwynn/base/config/config.py
+-rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0rc2/orwynn/base/config/test_config.py
+-rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0rc2/orwynn/base/controller/__init__.py
+-rw-r--r--   0        0        0     2211 2023-07-06 09:35:56.327943 orwynn-1.0.0rc2/orwynn/base/controller/controller.py
+-rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0rc2/orwynn/base/controller/errors.py
+-rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0rc2/orwynn/base/database/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0rc2/orwynn/base/database/database.py
+-rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0rc2/orwynn/base/database/errors.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0rc2/orwynn/base/error/__init__.py
+-rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0rc2/orwynn/base/error/code.py
+-rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0rc2/orwynn/base/error/errors.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0rc2/orwynn/base/error/test_main.py
+-rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0rc2/orwynn/base/error/test_utils.py
+-rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0rc2/orwynn/base/error/utils.py
+-rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0rc2/orwynn/base/error/valueschema.py
+-rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0rc2/orwynn/base/errorhandler/__init__.py
+-rw-r--r--   0        0        0     2354 2023-07-10 16:06:16.709892 orwynn-1.0.0rc2/orwynn/base/errorhandler/errorhandler.py
+-rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0rc2/orwynn/base/middleware/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0rc2/orwynn/base/middleware/globalsetup.py
+-rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0rc2/orwynn/base/middleware/middleware.py
+-rw-r--r--   0        0        0     1281 2023-07-10 13:45:40.445311 orwynn-1.0.0rc2/orwynn/base/middleware/test_main.py
+-rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0rc2/orwynn/base/model/__init__.py
+-rw-r--r--   0        0        0     1423 2023-07-06 09:10:08.307376 orwynn-1.0.0rc2/orwynn/base/model/model.py
+-rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0rc2/orwynn/base/model/test_model.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0rc2/orwynn/base/module/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0rc2/orwynn/base/module/errors.py
+-rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0rc2/orwynn/base/module/module.py
+-rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0rc2/orwynn/base/module/test_module.py
+-rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0rc2/orwynn/base/service/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0rc2/orwynn/base/service/framework.py
+-rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0rc2/orwynn/base/service/service.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0rc2/orwynn/base/worker/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0rc2/orwynn/base/worker/worker.py
+-rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0rc2/orwynn/boot/__init__.py
+-rw-r--r--   0        0        0    12600 2023-07-10 13:48:28.037990 orwynn-1.0.0rc2/orwynn/boot/boot.py
+-rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0rc2/orwynn/boot/config.py
+-rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0rc2/orwynn/boot/errors.py
+-rw-r--r--   0        0        0     5375 2023-07-10 12:56:58.086353 orwynn-1.0.0rc2/orwynn/boot/test_main.py
+-rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0rc2/orwynn/bootscript/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-10 12:10:57.216627 orwynn-1.0.0rc2/orwynn/bootscript/bootscript.py
+-rw-r--r--   0        0        0      114 2023-07-10 13:25:24.969000 orwynn-1.0.0rc2/orwynn/bootscript/callable.py
+-rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0rc2/orwynn/bootscript/calltime.py
+-rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0rc2/orwynn/bootscript/errors.py
+-rw-r--r--   0        0        0     1384 2023-07-10 13:45:40.440312 orwynn-1.0.0rc2/orwynn/bootscript/test_main.py
+-rw-r--r--   0        0        0     2523 2023-07-10 13:45:40.438311 orwynn-1.0.0rc2/orwynn/bootscript/worker.py
+-rw-r--r--   0        0        0       31 2023-07-10 13:55:28.842455 orwynn-1.0.0rc2/orwynn/cli/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-11 07:12:44.820534 orwynn-1.0.0rc2/orwynn/cli/__main__.py
+-rw-r--r--   0        0        0     2298 2023-07-10 14:23:02.733708 orwynn-1.0.0rc2/orwynn/cli/cli.py
+-rw-r--r--   0        0        0      363 2023-07-10 14:08:27.708229 orwynn-1.0.0rc2/orwynn/cli/enums.py
+-rw-r--r--   0        0        0      394 2023-07-10 14:08:51.966173 orwynn-1.0.0rc2/orwynn/cli/models.py
+-rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0rc2/orwynn/context/__init__.py
+-rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/context/errors.py
+-rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0rc2/orwynn/context/manager.py
+-rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0rc2/orwynn/context/storage.py
+-rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0rc2/orwynn/di/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-06 09:39:22.689224 orwynn-1.0.0rc2/orwynn/di/acceptor.py
+-rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0rc2/orwynn/di/availability.py
+-rw-r--r--   0        0        0     1742 2023-07-10 11:27:13.013752 orwynn-1.0.0rc2/orwynn/di/collecting/acceptordependencies.py
+-rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0rc2/orwynn/di/collecting/errors.py
+-rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0rc2/orwynn/di/collecting/helpers.py
+-rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0rc2/orwynn/di/collecting/modulecollector.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/collect.py
+-rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/map.py
+-rw-r--r--   0        0        0     1759 2023-07-10 13:45:40.439311 orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/test_main.py
+-rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0rc2/orwynn/di/collecting/test_modules.py
+-rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0rc2/orwynn/di/constants.py
+-rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0rc2/orwynn/di/container.py
+-rw-r--r--   0        0        0     4694 2023-07-10 12:27:55.169185 orwynn-1.0.0rc2/orwynn/di/di.py
+-rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0rc2/orwynn/di/errors.py
+-rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0rc2/orwynn/di/init/acceptors.py
+-rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0rc2/orwynn/di/init/providers.py
+-rw-r--r--   0        0        0     3093 2023-07-10 13:45:40.439311 orwynn-1.0.0rc2/orwynn/di/init/test_acceptors.py
+-rw-r--r--   0        0        0      492 2023-07-10 13:45:40.436311 orwynn-1.0.0rc2/orwynn/di/init/test_providers.py
+-rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0rc2/orwynn/di/isacceptor.py
+-rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0rc2/orwynn/di/isprovider.py
+-rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0rc2/orwynn/di/object.py
+-rw-r--r--   0        0        0       45 2023-07-06 09:39:13.705327 orwynn-1.0.0rc2/orwynn/di/provider.py
+-rw-r--r--   0        0        0      535 2023-07-10 12:53:28.658639 orwynn-1.0.0rc2/orwynn/di/testing.py
+-rw-r--r--   0        0        0       93 2023-07-10 14:34:03.676610 orwynn-1.0.0rc2/orwynn/helpers/address/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-11 07:12:44.820534 orwynn-1.0.0rc2/orwynn/helpers/address/address.py
+-rw-r--r--   0        0        0      200 2023-07-10 14:27:26.222387 orwynn-1.0.0rc2/orwynn/helpers/address/errors.py
+-rw-r--r--   0        0        0      419 2023-07-11 07:13:16.868307 orwynn-1.0.0rc2/orwynn/helpers/address/regex.py
+-rw-r--r--   0        0        0     1076 2023-07-11 07:12:44.821534 orwynn-1.0.0rc2/orwynn/helpers/address/test_main.py
+-rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0rc2/orwynn/helpers/constants.py
+-rw-r--r--   0        0        0      813 2023-07-10 12:47:57.896389 orwynn-1.0.0rc2/orwynn/helpers/errors.py
+-rw-r--r--   0        0        0     1130 2023-07-10 16:06:16.709892 orwynn-1.0.0rc2/orwynn/helpers/web.py
+-rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0rc2/orwynn/http/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0rc2/orwynn/http/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0rc2/orwynn/http/context/__init__.py
+-rw-r--r--   0        0        0      959 2023-07-05 09:50:46.449134 orwynn-1.0.0rc2/orwynn/http/context/id.py
+-rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0rc2/orwynn/http/context/middleware/builtin.py
+-rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0rc2/orwynn/http/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0     1039 2023-07-10 13:45:40.440312 orwynn-1.0.0rc2/orwynn/http/context/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0rc2/orwynn/http/controller/__init__.py
+-rw-r--r--   0        0        0     5438 2023-07-10 16:06:16.713892 orwynn-1.0.0rc2/orwynn/http/controller/controller.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/__init__.py
+-rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/container.py
+-rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/endpoint.py
+-rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/response.py
+-rw-r--r--   0        0        0     2346 2023-07-10 12:57:39.935615 orwynn-1.0.0rc2/orwynn/http/controller/endpoint/test_main.py
+-rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/http/controller/errors.py
+-rw-r--r--   0        0        0     8099 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/http/controller/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0rc2/orwynn/http/cors/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0rc2/orwynn/http/cors/cors.py
+-rw-r--r--   0        0        0     3666 2023-07-10 13:45:40.443311 orwynn-1.0.0rc2/orwynn/http/cors/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0rc2/orwynn/http/errorhandler/__init__.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0rc2/orwynn/http/errorhandler/default.py
+-rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0rc2/orwynn/http/errorhandler/middleware.py
+-rw-r--r--   0        0        0     6448 2023-07-10 13:45:40.438311 orwynn-1.0.0rc2/orwynn/http/errorhandler/test_main.py
+-rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0rc2/orwynn/http/errors.py
+-rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0rc2/orwynn/http/log/logger.py
+-rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0rc2/orwynn/http/log/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0rc2/orwynn/http/middleware/__init__.py
+-rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0rc2/orwynn/http/middleware/builtinmiddleware.py
+-rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0rc2/orwynn/http/middleware/middleware.py
+-rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0rc2/orwynn/http/middleware/nextcall.py
+-rw-r--r--   0        0        0     2285 2023-07-10 12:11:25.635467 orwynn-1.0.0rc2/orwynn/http/middleware/test_main.py
+-rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0rc2/orwynn/http/requests.py
+-rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0rc2/orwynn/http/responses.py
+-rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0rc2/orwynn/http/schema/validationvalue.py
+-rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0rc2/orwynn/http/schema/value.py
+-rw-r--r--   0        0        0      928 2023-07-10 13:45:40.442311 orwynn-1.0.0rc2/orwynn/http/test_responses.py
+-rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0rc2/orwynn/http/testing.py
+-rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0rc2/orwynn/indication/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0rc2/orwynn/indication/default.py
+-rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/indication/errors.py
+-rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0rc2/orwynn/indication/indicatable.py
+-rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0rc2/orwynn/indication/indication.py
+-rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0rc2/orwynn/indication/indicator.py
+-rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0rc2/orwynn/indication/test_main.py
+-rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0rc2/orwynn/indication/type.py
+-rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0rc2/orwynn/log/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0rc2/orwynn/log/config.py
+-rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0rc2/orwynn/log/configure.py
+-rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0rc2/orwynn/log/constants.py
+-rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/log/errors.py
+-rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0rc2/orwynn/log/handler.py
+-rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0rc2/orwynn/log/helpers.py
+-rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0rc2/orwynn/log/log.py
+-rw-r--r--   0        0        0     1857 2023-07-10 13:48:38.598021 orwynn-1.0.0rc2/orwynn/log/test_main.py
+-rw-r--r--   0        0        0     3774 2023-07-10 12:05:44.416709 orwynn-1.0.0rc2/orwynn/log/test_middleware.py
+-rw-r--r--   0        0        0     1498 2023-07-10 12:05:51.324037 orwynn-1.0.0rc2/orwynn/log/test_websocketmiddleware.py
+-rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0rc2/orwynn/log/types.py
+-rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0rc2/orwynn/mapping/__init__.py
+-rw-r--r--   0        0        0      667 2023-07-05 09:49:27.438110 orwynn-1.0.0rc2/orwynn/mapping/errors.py
+-rw-r--r--   0        0        0     1808 2023-07-05 09:47:23.970713 orwynn-1.0.0rc2/orwynn/mapping/mapping.py
+-rw-r--r--   0        0        0      504 2023-07-05 09:49:15.096266 orwynn-1.0.0rc2/orwynn/mapping/test_main.py
+-rw-r--r--   0        0        0      216 2023-07-04 11:01:21.049070 orwynn-1.0.0rc2/orwynn/mongo/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0rc2/orwynn/mongo/clientsession.py
+-rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0rc2/orwynn/mongo/config.py
+-rw-r--r--   0        0        0     7634 2023-07-06 08:54:40.455677 orwynn-1.0.0rc2/orwynn/mongo/document/__init__.py
+-rw-r--r--   0        0        0      578 2023-07-06 07:33:03.897136 orwynn-1.0.0rc2/orwynn/mongo/document/errors.py
+-rw-r--r--   0        0        0     1134 2023-07-05 09:33:28.956933 orwynn-1.0.0rc2/orwynn/mongo/document/helpers.py
+-rw-r--r--   0        0        0     1367 2023-07-05 09:33:28.955933 orwynn-1.0.0rc2/orwynn/mongo/document/test_converttoobjectid.py
+-rw-r--r--   0        0        0      219 2023-07-10 13:45:40.437312 orwynn-1.0.0rc2/orwynn/mongo/document/test_create.py
+-rw-r--r--   0        0        0      742 2023-07-06 07:53:44.416182 orwynn-1.0.0rc2/orwynn/mongo/document/test_get.py
+-rw-r--r--   0        0        0      703 2023-07-06 08:55:42.984735 orwynn-1.0.0rc2/orwynn/mongo/document/test_inc.py
+-rw-r--r--   0        0        0      275 2023-07-06 07:46:04.044931 orwynn-1.0.0rc2/orwynn/mongo/document/test_refresh.py
+-rw-r--r--   0        0        0      230 2023-07-06 06:48:10.593442 orwynn-1.0.0rc2/orwynn/mongo/document/test_remove.py
+-rw-r--r--   0        0        0      829 2023-07-06 08:55:42.984735 orwynn-1.0.0rc2/orwynn/mongo/document/test_set.py
+-rw-r--r--   0        0        0     1312 2023-07-06 07:42:00.340990 orwynn-1.0.0rc2/orwynn/mongo/document/test_updateoperators.py
+-rw-r--r--   0        0        0      708 2023-07-06 08:51:37.969595 orwynn-1.0.0rc2/orwynn/mongo/document/testing.py
+-rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0rc2/orwynn/mongo/entity.py
+-rw-r--r--   0        0        0      882 2023-07-05 09:49:15.103266 orwynn-1.0.0rc2/orwynn/mongo/errors.py
+-rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0rc2/orwynn/mongo/mongo.py
+-rw-r--r--   0        0        0     1354 2023-07-04 11:01:22.010065 orwynn-1.0.0rc2/orwynn/mongo/test_main.py
+-rw-r--r--   0        0        0      430 2023-07-10 12:58:56.726342 orwynn-1.0.0rc2/orwynn/mongo/testing.py
+-rw-r--r--   0        0        0     2829 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/proxy/boot.py
+-rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0rc2/orwynn/proxy/indicationonly.py
+-rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0rc2/orwynn/router/__init__.py
+-rw-r--r--   0        0        0     4039 2023-07-11 07:16:51.954798 orwynn-1.0.0rc2/orwynn/router/errorhandlermanager.py
+-rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/router/errors.py
+-rw-r--r--   0        0        0    14253 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/router/register/controller.py
+-rw-r--r--   0        0        0     9646 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/router/register/middleware.py
+-rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0rc2/orwynn/router/router.py
+-rw-r--r--   0        0        0     2640 2023-07-10 13:45:40.441311 orwynn-1.0.0rc2/orwynn/router/test_globalroute.py
+-rw-r--r--   0        0        0       86 2023-07-11 07:49:30.101961 orwynn-1.0.0rc2/orwynn/server/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-11 07:41:29.452106 orwynn-1.0.0rc2/orwynn/server/engine.py
+-rw-r--r--   0        0        0     1834 2023-07-11 07:47:19.222962 orwynn-1.0.0rc2/orwynn/server/server.py
+-rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0rc2/orwynn/singleton/__init__.py
+-rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0rc2/orwynn/singleton/singleton.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0rc2/orwynn/sql/__init__.py
+-rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0rc2/orwynn/sql/config.py
+-rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0rc2/orwynn/sql/databasekind.py
+-rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0rc2/orwynn/sql/poolclass.py
+-rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0rc2/orwynn/sql/sql.py
+-rw-r--r--   0        0        0     2636 2023-07-05 09:50:46.449134 orwynn-1.0.0rc2/orwynn/sql/table.py
+-rw-r--r--   0        0        0     5895 2023-07-10 12:06:27.480702 orwynn-1.0.0rc2/orwynn/sql/test_main.py
+-rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0rc2/orwynn/testing/__init__.py
+-rw-r--r--   0        0        0    11287 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/testing/client.py
+-rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0rc2/orwynn/testing/embeddedclient.py
+-rw-r--r--   0        0        0     2180 2023-07-10 13:45:40.441311 orwynn-1.0.0rc2/orwynn/testing/test_main.py
+-rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0rc2/orwynn/testingtools/__init__.py
+-rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0rc2/orwynn/utils/basesubclassable.py
+-rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0rc2/orwynn/utils/crypto/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0rc2/orwynn/utils/dt/__init__.py
+-rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0rc2/orwynn/utils/fmt/__init__.py
+-rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0rc2/orwynn/utils/fmt/test_main.py
+-rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0rc2/orwynn/utils/klass/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0rc2/orwynn/utils/klass/errors.py
+-rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0rc2/orwynn/utils/klass/test_klass.py
+-rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0rc2/orwynn/utils/mp/__init__.py
+-rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0rc2/orwynn/utils/mp/dictpp.py
+-rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0rc2/orwynn/utils/mp/location.py
+-rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0rc2/orwynn/utils/mp/test_main.py
+-rw-r--r--   0        0        0      131 2023-07-05 09:50:46.441135 orwynn-1.0.0rc2/orwynn/utils/rnd/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-05 09:50:46.449134 orwynn-1.0.0rc2/orwynn/utils/rnd/test_main.py
+-rw-r--r--   0        0        0      171 2023-07-10 16:06:21.903818 orwynn-1.0.0rc2/orwynn/utils/scheme.py
+-rw-r--r--   0        0        0      423 2023-07-10 11:23:30.134562 orwynn-1.0.0rc2/orwynn/utils/types.py
+-rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0rc2/orwynn/utils/uio.py
+-rw-r--r--   0        0        0      680 2023-07-10 14:29:34.142049 orwynn-1.0.0rc2/orwynn/utils/url/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0rc2/orwynn/utils/url/helpers.py
+-rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0rc2/orwynn/utils/url/test_utils.py
+-rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0rc2/orwynn/utils/url/url.py
+-rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0rc2/orwynn/utils/url/utils.py
+-rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0rc2/orwynn/utils/url/vars.py
+-rw-r--r--   0        0        0     9565 2023-07-10 12:38:01.181313 orwynn-1.0.0rc2/orwynn/utils/validation/__init__.py
+-rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0rc2/orwynn/utils/validation/errors.py
+-rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0rc2/orwynn/utils/validation/validator.py
+-rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0rc2/orwynn/utils/yml/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0rc2/orwynn/utils/yml/errors.py
+-rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0rc2/orwynn/websocket/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0rc2/orwynn/websocket/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0rc2/orwynn/websocket/context/__init__.py
+-rw-r--r--   0        0        0     1028 2023-07-05 09:50:46.450135 orwynn-1.0.0rc2/orwynn/websocket/context/id.py
+-rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0rc2/orwynn/websocket/context/middleware/builtin.py
+-rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0rc2/orwynn/websocket/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0     1296 2023-07-10 13:45:40.444311 orwynn-1.0.0rc2/orwynn/websocket/context/test_main.py
+-rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0rc2/orwynn/websocket/controller/controller.py
+-rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0rc2/orwynn/websocket/controller/eventhandlermethod.py
+-rw-r--r--   0        0        0     4067 2023-07-10 13:45:40.446311 orwynn-1.0.0rc2/orwynn/websocket/controller/test_controller.py
+-rw-r--r--   0        0        0     3062 2023-07-10 12:08:27.941623 orwynn-1.0.0rc2/orwynn/websocket/controller/test_globalroute.py
+-rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0rc2/orwynn/websocket/errorhandler/default.py
+-rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0rc2/orwynn/websocket/errorhandler/middleware.py
+-rw-r--r--   0        0        0     1788 2023-07-10 16:06:16.720892 orwynn-1.0.0rc2/orwynn/websocket/errorhandler/test_default.py
+-rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0rc2/orwynn/websocket/log/logger.py
+-rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0rc2/orwynn/websocket/log/middleware.py
+-rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0rc2/orwynn/websocket/middleware/builtin.py
+-rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0rc2/orwynn/websocket/middleware/connectionbuiltin.py
+-rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0rc2/orwynn/websocket/middleware/middleware.py
+-rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0rc2/orwynn/websocket/middleware/nextcall.py
+-rw-r--r--   0        0        0     1108 2023-07-10 13:45:40.443311 orwynn-1.0.0rc2/orwynn/websocket/middleware/test_main.py
+-rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0rc2/orwynn/websocket/routing/dispatchfn.py
+-rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0rc2/orwynn/websocket/routing/genericfn.py
+-rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0rc2/orwynn/websocket/routing/handlers.py
+-rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0rc2/orwynn/websocket/routing/helpers.py
+-rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0rc2/orwynn/websocket/routing/nextcall.py
+-rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0rc2/orwynn/websocket/routing/stack.py
+-rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0rc2/orwynn/websocket/websocket.py
+-rw-r--r--   0        0        0      928 2023-07-11 07:50:01.310419 orwynn-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 orwynn-1.0.0rc2/PKG-INFO
```

### Comparing `orwynn-1.0.0rc1/LICENSE` & `orwynn-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/apiversion/__init__.py` & `orwynn-1.0.0rc2/orwynn/apiversion/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/apiversion/test_main.py` & `orwynn-1.0.0rc2/orwynn/apiversion/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.http import Endpoint, HttpController
 from orwynn.utils import validation
 
 from . import ApiVersion
 from .errors import UnsupportedVersionError
 
 # NOTE: By default there is no global route for backwards compatiblity.
 
-def test_versioned_global_route():
+@pytest.mark.asyncio
+async def test_versioned_global_route():
     class C(HttpController):
         ROUTE = "/message"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C]),
         global_http_route="/donuts/v{version}",
     )
 
     boot.app.client.get_jsonify(
         "/donuts/v1/user/message",
         200,
         is_global_route_used=False
     )
 
 
-def test_controller_version():
+@pytest.mark.asyncio
+async def test_controller_version():
     """
     HttpController can define older version of API than available.
     """
     class C1(HttpController):
         ROUTE = "/message"
         VERSION = 1
         ENDPOINTS = [Endpoint(method="get")]
@@ -45,15 +49,15 @@
         # latest.
         ROUTE = "/message"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello v2"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C1, C2]),
         global_http_route="/api/v{version}",
         api_version=ApiVersion(
             supported={1, 2}
         )
     )
 
@@ -70,24 +74,25 @@
     assert data["message"] == "hello v2"
 
     data = boot.app.client.get_jsonify(
         "/api/v3/user/message", 404, is_global_route_used=False
     )
 
 
-def test_controller_all_versions():
+@pytest.mark.asyncio
+async def test_controller_all_versions():
     class C1(HttpController):
         ROUTE = "/message"
         VERSION = "*"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C1]),
         global_http_route="/api/v{version}",
         api_version=ApiVersion(
             supported={1, 2, 3}
         )
     )
 
@@ -99,24 +104,25 @@
     data = boot.app.client.get_jsonify("/user/message", 200, api_version=2)
     assert data["message"] == "hello"
 
     data = boot.app.client.get_jsonify("/user/message", 200, api_version=3)
     assert data["message"] == "hello"
 
 
-def test_controller_several_versions():
+@pytest.mark.asyncio
+async def test_controller_several_versions():
     class C1(HttpController):
         ROUTE = "/message"
         VERSION = {2, 3}
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C1]),
         global_http_route="/api/v{version}",
         api_version=ApiVersion(
             supported={1, 2, 3}
         )
     )
 
@@ -127,46 +133,50 @@
     data = boot.app.client.get_jsonify("/user/message", 200, api_version=2)
     assert data["message"] == "hello"
 
     data = boot.app.client.get_jsonify("/user/message", 200, api_version=3)
     assert data["message"] == "hello"
 
 
-def test_controller_unsupported_version():
+@pytest.mark.asyncio
+async def test_controller_unsupported_version():
     class C1(HttpController):
         ROUTE = "/message"
         VERSION = 3
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    validation.expect(
-        Boot,
-        UnsupportedVersionError,
-        root_module=Module("/user", Controllers=[C1]),
-        global_http_route="/api/v{version}",
-        api_version=ApiVersion(
-            supported={1, 2}
-        )
+    await validation.expect_async(
+        Boot.create(
+            root_module=Module("/user", Controllers=[C1]),
+            global_http_route="/api/v{version}",
+            api_version=ApiVersion(
+                supported={1, 2}
+            )
+        ),
+        UnsupportedVersionError
     )
 
 
-def test_controller_unsupported_version_of_many():
+@pytest.mark.asyncio
+async def test_controller_unsupported_version_of_many():
     class C1(HttpController):
         ROUTE = "/message"
         # Some are supported, some are not
         VERSION = {2, 3}
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    validation.expect(
-        Boot,
-        UnsupportedVersionError,
-        root_module=Module("/user", Controllers=[C1]),
-        global_http_route="/api/v{version}",
-        api_version=ApiVersion(
-            supported={1, 2}
-        )
+    await validation.expect_async(
+        Boot.create(
+            root_module=Module("/user", Controllers=[C1]),
+            global_http_route="/api/v{version}",
+            api_version=ApiVersion(
+                supported={1, 2}
+            )
+        ),
+        UnsupportedVersionError
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/app/apiwebsocketroute.py` & `orwynn-1.0.0rc2/orwynn/app/apiwebsocketroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/app/app.py` & `orwynn-1.0.0rc2/orwynn/app/app.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/app/core.py` & `orwynn-1.0.0rc2/orwynn/app/core.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/app/test_main.py` & `orwynn-1.0.0rc2/orwynn/app/test_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import pytest
 from pytest import fixture
 
 from orwynn.app.app import App
 from orwynn.base.module import Module
 from orwynn.boot import Boot
 from orwynn.websocket import Websocket, WebsocketController
 
 
 @fixture
 def std_app(std_boot: Boot) -> App:
     return std_boot.app
 
 
-def test_openapi(run_endpoint):
+@pytest.mark.asyncio
+async def test_openapi(run_endpoint):
     data: dict = Boot.ie().app.client.get_jsonify("/openapi.json", 200)
 
     path: dict = data["paths"]["/"]["get"]
     assert path["deprecated"] is True
     assert path["tags"] == ["best-item", "buy-now"]
     assert \
         path["responses"]["201"]["description"] == "Best response description"
     assert \
         path["responses"]["201"]["description"] == "Best response description"
 
 
-def test_get_dependant_patch_against_websocket():
+@pytest.mark.asyncio
+async def test_get_dependant_patch_against_websocket():
     """
     Should correctly operate for websocket controllers and builtin middleware.
     """
 
     # FIXME:
     #   Due to strange reasons, this test works fine in orwynn environment,
     #   but gives an error related to fastapi.dependencies.utils.get_dependant
@@ -36,24 +39,25 @@
 
     class WsCtrl(WebsocketController):
         ROUTE = "/"
 
         async def main(self, websocket: Websocket) -> None:
             await websocket.send_json({"message": "hello"})
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[WsCtrl])
     )
 
     with boot.app.client.websocket("/") as ws:
         ws.receive_json()
 
 
-def test_custom_docs_route():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_custom_docs_route():
+    boot: Boot = await Boot.create(
         Module("/"),
         apprc={
             "prod": {
                 "App": {
                     "docs_route": "/mydocs"
                 }
             }
@@ -61,16 +65,17 @@
     )
 
     # TODO: maybe to add checking that this is truly OpenAPI page returned,
     #       but now i'm too lazy for this
     boot.app.client.get("/mydocs", 200)
 
 
-def test_custom_redoc_route():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_custom_redoc_route():
+    boot: Boot = await Boot.create(
         Module("/"),
         apprc={
             "prod": {
                 "App": {
                     "redoc_route": "/myredoc"
                 }
             }
```

### Comparing `orwynn-1.0.0rc1/orwynn/app/utils.py` & `orwynn-1.0.0rc2/orwynn/app/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/apprc/parse.py` & `orwynn-1.0.0rc2/orwynn/apprc/parse.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/apprc/test_main.py` & `orwynn-1.0.0rc2/orwynn/apprc/test_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -52,29 +52,31 @@
                     "fried_chicken": 5.0
                 }
             }
         }
     }
 
 
-def test_prod(raw_apprc: AppRc):
-    Boot(
+@pytest.mark.asyncio
+async def test_prod(raw_apprc: AppRc):
+    await Boot.create(
         root_module=Module("/", Providers=[BurgerShotConfig]),
         apprc=raw_apprc,
         mode=AppMode.PROD
     )
 
     assert validation.apply(
         Di.ie().find("BurgerShotConfig"),
         BurgerShotConfig
     ).dict() == mp_find("prod.BurgerShot", raw_apprc)
 
 
-def test_dev(raw_apprc: AppRc):
-    Boot(
+@pytest.mark.asyncio
+async def test_dev(raw_apprc: AppRc):
+    await Boot.create(
         root_module=Module("/", Providers=[BurgerShotConfig]),
         apprc=raw_apprc,
         mode=AppMode.DEV
     )
 
     assert validation.apply(
         Di.ie().find("BurgerShotConfig"),
@@ -87,16 +89,17 @@
             "cola": 1.8,
             "pizza": 4.1,
             "fried_chicken": 3.5
         }
     }
 
 
-def test_test(raw_apprc: AppRc):
-    Boot(
+@pytest.mark.asyncio
+async def test_test(raw_apprc: AppRc):
+    await Boot.create(
         root_module=Module("/", Providers=[BurgerShotConfig]),
         apprc=raw_apprc,
         mode=AppMode.TEST
     )
 
     assert validation.apply(
         Di.ie().find("BurgerShotConfig"),
```

### Comparing `orwynn-1.0.0rc1/orwynn/base/config/config.py` & `orwynn-1.0.0rc2/orwynn/base/config/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/controller/controller.py` & `orwynn-1.0.0rc2/orwynn/base/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/database/database.py` & `orwynn-1.0.0rc2/orwynn/base/database/database.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/database/errors.py` & `orwynn-1.0.0rc2/orwynn/base/database/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/error/code.py` & `orwynn-1.0.0rc2/orwynn/base/error/code.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/error/test_main.py` & `orwynn-1.0.0rc2/orwynn/base/error/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/error/utils.py` & `orwynn-1.0.0rc2/orwynn/base/error/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/errorhandler/errorhandler.py` & `orwynn-1.0.0rc2/orwynn/base/errorhandler/errorhandler.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import ClassVar
 
 from orwynn.base.error.errors import MalfunctionError
 from orwynn.helpers.web import GenericRequest, GenericResponse
 from orwynn.log.helpers import catch_error
 from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 
 
 class ErrorHandler:
     """
     Handles outcoming errors from the application.
     Method handle(...) should be redefined in subclass in order to work.
 
@@ -20,26 +20,26 @@
         PROTOCOL:
             Protocol the handler works with.
         IS_ERROR_CATCH_LOGGED:
             Whether the handled errors should be automatically logged by
             Log.catch. Defaults to True.
     """
     E: ClassVar[type[Exception] | None] = None
-    PROTOCOL: Protocol = Protocol.HTTP
+    PROTOCOL: Scheme = Scheme.HTTP
     IS_ERROR_CATCH_LOGGED: bool = True
 
     def __init__(self) -> None:
         if self.E is None:
             raise TypeError(
                 f"{self.__class__} error class is not set"
             )
         else:
             validation.validate(self.E, Exception)
 
-        validation.validate(self.PROTOCOL, Protocol)
+        validation.validate(self.PROTOCOL, Scheme)
 
     @classmethod
     def get_handled_exception_class(cls) -> type[Exception]:
         if cls.E is None:
             raise MalfunctionError(
                 f"error handler {cls} handled exception shouldn't be None"
             )
```

### Comparing `orwynn-1.0.0rc1/orwynn/base/middleware/middleware.py` & `orwynn-1.0.0rc2/orwynn/base/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/middleware/test_main.py` & `orwynn-1.0.0rc2/orwynn/base/middleware/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+import pytest
+
 from orwynn.base.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.di.di import Di
 from orwynn.http import HttpMiddleware
 from orwynn.utils import validation
 from orwynn.websocket import WebsocketMiddleware
 
 
-def test_http():
+@pytest.mark.asyncio
+async def test_http():
     """
     Should be able to add custom middleware globally.
     """
     class Mw(HttpMiddleware):
         def __init__(self, covered_routes: list[str]) -> None:
             self.covered_routes_ = covered_routes
             super().__init__(covered_routes)
 
-    Boot(
+    await Boot.create(
         Module(),
         global_middleware={
             Mw: ["/hello"]
         }
     )
 
     mw: Mw = validation.apply(Di.ie().find("Mw"), Mw)
     assert mw.covered_routes_ == ["/hello"]
 
 
-def test_websocket():
+@pytest.mark.asyncio
+async def test_websocket():
     """
     Should be able to add custom middleware globally.
     """
     class Mw(WebsocketMiddleware):
         def __init__(self, covered_routes: list[str]) -> None:
             self.covered_routes_ = covered_routes
             super().__init__(covered_routes)
 
-    Boot(
+    await Boot.create(
         Module(),
         global_middleware={
             Mw: ["/hello"]
         }
     )
 
     mw: Mw = validation.apply(Di.ie().find("Mw"), Mw)
```

### Comparing `orwynn-1.0.0rc1/orwynn/base/model/model.py` & `orwynn-1.0.0rc2/orwynn/base/model/model.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/model/test_model.py` & `orwynn-1.0.0rc2/orwynn/base/model/test_model.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/module/module.py` & `orwynn-1.0.0rc2/orwynn/base/module/module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/base/module/test_module.py` & `orwynn-1.0.0rc2/orwynn/base/module/test_module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/boot/boot.py` & `orwynn-1.0.0rc2/orwynn/boot/boot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import contextlib
 import os
 from copy import deepcopy
 from pathlib import Path
 from types import NoneType
+from typing import Self
 
 import dotenv
+from starlette.types import Receive, Scope, Send
 
 from orwynn.apiversion import ApiVersion
 from orwynn.app import App, AppMode
 from orwynn.apprc import AppRc, parse_apprc
 from orwynn.base.controller import Controller
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.base.middleware import GlobalMiddlewareSetup, Middleware
 from orwynn.base.module import Module
 from orwynn.base.worker import Worker
 from orwynn.bootscript import Bootscript, BootscriptWorker, CallTime
 from orwynn.bootscript.errors import NoScriptsForCallTimeError
 from orwynn.di.di import Di
 from orwynn.di.errors import MissingDiObjectError
+from orwynn.helpers.errors import DeprecatedFeatureError
 from orwynn.http import EndpointContainer
 from orwynn.indication import Indication, default_api_indication
 from orwynn.log import LogConfig, configure_log
 from orwynn.proxy.boot import BootProxy
 from orwynn.proxy.indicationonly import ApiIndicationOnlyProxy
 from orwynn.router import Router
 from orwynn.testing import Client
@@ -32,78 +35,24 @@
 
 class Boot(Worker):
     """Worker responsible of booting an application.
 
     General usage is to construct this class in the main.py with required
     parameters and then access Boot.app for your needs.
 
-    Attributes:
-        root_module:
-            Root module of the app.
-        dotenv_path (optional):
-            Path to .env file. Defaults to ".env".
-        api_indication (optional):
-            Indication object used as a convention for outcoming API
-            structures. Defaults to predefined by framework's indication
-            convention.
-        ErrorHandlers (optional):
-            List of exception handlers to add. By default framework adds
-            the builtin Exception and orwynn.Error handlers.
-        apprc (optional):
-            Application configuration. By default environ ORWYNN_APPRC_PATH is
-            checked if this arg is not given.
-        mode (optional):
-            Application mode. By default environ ORWYNN_MODE is
-            checked if this arg is not given.
-        global_http_route (optional):
-            Global route to be prepended to every controller's route. Defaults
-            to no route. Can accept formatting "{version}" for an API version
-            to be injected into route.
-        global_websocket_route (optional):
-            Global route to be prepended to every controller's route. Defaults
-            to no route. Can accept formatting "{version}" for an API version
-            to be injected into route.
-        global_imports (optional):
-            Modules available across all other modules imported into the
-            application. Note that no other instance can import a globally
-            available module.
-        global_middleware (optional):
-            Map of middleware and its covered routes to apply globally. Note
-            that every initialized Provider can be accessed from such
-            middleware.
-        api_version (optional):
-            Object describes API versioning rules for the project. By default
-            only v1 is supported.
-        bootscripts (optional):
-            List of bootscripts to be launched at different points of boot
-            time.
-
     Environs:
         - ORWYNN_MODE:
             Boot mode for application. Defaults to DEV. Alternatively you can
             pass arg "mode".
         - ORWYNN_ROOT_DIR:
             Root directory for application. Defaults to os.getcwd()
         - ORWYNN_APPRC_PATH:
             Path where app configuration file located. Defaults to
             "./apprc.yml". Alternatively you can pass a dictionary directly in
             "apprc" attribute.
-
-    Usage:
-    ```py
-    # main.py
-    from orwynn import Boot, App
-
-    # Import root module from your location
-    from .myproject.root_module import root_module
-
-    app: App = Boot(
-        root_module=root_module
-    ).app
-    ```
     """
     def __init__(
         self,
         root_module: Module,
         *,
         dotenv_path: Path | None = None,
         api_indication: Indication | None = None,
@@ -111,17 +60,19 @@
         apprc: AppRc | None = None,
         mode: AppMode | None = None,
         global_http_route: str | None = None,
         global_websocket_route: str | None = None,
         global_modules: list[Module] | None = None,
         global_middleware: GlobalMiddlewareSetup | None = None,
         api_version: ApiVersion | None = None,
-        bootscripts: list[Bootscript] | None = None
+        bootscripts: list[Bootscript] | None = None,
+        _fw_init_lock: bool = True
     ) -> None:
-        super().__init__()
+        self._check_init_lock(_fw_init_lock)
+
         if dotenv_path is None:
             dotenv_path = Path(".env")
         validate(dotenv_path, Path)
         validate(root_module, Module)
         if api_indication is None:
             api_indication = default_api_indication
         validate(api_indication, Indication)
@@ -174,15 +125,15 @@
             deepcopy(apprc)
         )
         self.__global_http_route: str = global_http_route
         self.__global_websocket_route: str = global_websocket_route
         self.__api_version: ApiVersion = api_version
 
         # Initialize bootscript
-        bootscript_worker: BootscriptWorker = BootscriptWorker(
+        self._bootscript_worker: BootscriptWorker = BootscriptWorker(
             bootscripts=bootscripts
         )
 
         self.__initialize_proxies(
             ErrorHandlers=ErrorHandlers,
             api_indication=api_indication
         )
@@ -197,17 +148,117 @@
 
         # Configure logging
         configure_log(
             validation.apply(self.__di.find("LogConfig"), LogConfig),
             app_mode_prod=AppMode.PROD
         )
 
+    async def __call__(
+        self, scope: Scope, receive: Receive, send: Send
+    ) -> None:
+        """
+        Propagates a call to the created application.
+        """
+        await self.app(scope, receive, send)
+
+    @classmethod
+    async def create(
+        cls,
+        root_module: Module,
+        *,
+        dotenv_path: Path | None = None,
+        api_indication: Indication | None = None,
+        ErrorHandlers: set[type[ErrorHandler]] | None = None,
+        apprc: AppRc | None = None,
+        mode: AppMode | None = None,
+        global_http_route: str | None = None,
+        global_websocket_route: str | None = None,
+        global_modules: list[Module] | None = None,
+        global_middleware: GlobalMiddlewareSetup | None = None,
+        api_version: ApiVersion | None = None,
+        bootscripts: list[Bootscript] | None = None
+    ) -> Self:
+        """
+        Creates a Boot instance.
+
+        This should be the only way to initialize a new Boot.
+
+        Idea of using this create() method instead of traditional __init__ is
+        to await important asynchronous coroutines every time a fresh boot
+        is created.
+
+        Args:
+            root_module:
+                Root module of the app.
+            dotenv_path (optional):
+                Path to .env file. Defaults to ".env".
+            api_indication (optional):
+                Indication object used as a convention for outcoming API
+                structures. Defaults to predefined by framework's indication
+                convention.
+            ErrorHandlers (optional):
+                List of exception handlers to add. By default framework adds
+                the builtin Exception and orwynn.Error handlers.
+            apprc (optional):
+                Application configuration. By default environ ORWYNN_APPRC_PATH
+                is checked if this arg is not given.
+            mode (optional):
+                Application mode. By default environ ORWYNN_MODE is
+                checked if this arg is not given.
+            global_http_route (optional):
+                Global route to be prepended to every controller's route.
+                Defaults to no route. Can accept formatting "{version}" for an
+                API version to be injected into route.
+            global_websocket_route (optional):
+                Global route to be prepended to every controller's route.
+                Defaults to no route. Can accept formatting "{version}" for an
+                API version to be injected into route.
+            global_imports (optional):
+                Modules available across all other modules imported into the
+                application. Note that no other instance can import a globally
+                available module.
+            global_middleware (optional):
+                Map of middleware and its covered routes to apply globally.
+                Note that every initialized Provider can be accessed from such
+                middleware.
+            api_version (optional):
+                Object describes API versioning rules for the project. By
+                default only v1 is supported.
+            bootscripts (optional):
+                List of bootscripts to be launched at different points of boot
+                time.
+        """
+
+        boot: Boot = Boot(
+            root_module,
+            dotenv_path=dotenv_path,
+            api_indication=api_indication,
+            ErrorHandlers=ErrorHandlers,
+            apprc=apprc,
+            mode=mode,
+            global_http_route=global_http_route,
+            global_websocket_route=global_websocket_route,
+            global_modules=global_modules,
+            global_middleware=global_middleware,
+            api_version=api_version,
+            bootscripts=bootscripts,
+            _fw_init_lock=False
+        )
+
+        await boot._call_bootscripts()
+
+        return boot
+
+    async def _call_bootscripts(self) -> None:
+        """
+        Calls bootscripts for all time frames.
+        """
         # AFTER_ALL bootscript call time
         with contextlib.suppress(NoScriptsForCallTimeError):
-            bootscript_worker.call_by_time(
+            await self._bootscript_worker.call_by_time(
                 CallTime.AFTER_ALL,
                 self.__di._fw_container
             )
 
     def __initialize_mode(
         self,
         input_mode: AppMode | None
@@ -304,7 +355,14 @@
 
         if not root_dir.is_dir():
             raise NotDirError(
                 f"{root_dir} is not a directory"
             )
 
         return root_dir
+
+    def _check_init_lock(self, lock: bool) -> None:
+        if lock:
+            raise DeprecatedFeatureError(
+                deprecated_feature="initializing Boot via __init__",
+                use_instead="Boot.create(...)"
+            )
```

### Comparing `orwynn-1.0.0rc1/orwynn/boot/config.py` & `orwynn-1.0.0rc2/orwynn/boot/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/boot/test_main.py` & `orwynn-1.0.0rc2/orwynn/boot/test_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 import pytest
-from pytest import fixture
+import pytest_asyncio
 
 from orwynn.app import AppMode
 from orwynn.apprc.apprc import AppRc
 from orwynn.base.module.errors import CircularDependencyError
 from orwynn.base.module.module import Module
 from orwynn.base.service.service import Service
 from orwynn.boot.boot import Boot
@@ -18,135 +18,147 @@
 
 
 class _GService(Service):
     def calculate(self, *args: int) -> int:
         return sum(args)
 
 
-@fixture
-def std_boot(std_struct: Module) -> Boot:
-    return Boot(
+@pytest_asyncio.fixture
+async def std_boot(std_struct: Module) -> Boot:
+    return await Boot.create(
         root_module=std_struct
     )
 
 
-@fixture
-def run_std(std_struct: Module):
-    Boot(std_struct)
+@pytest_asyncio.fixture
+async def run_std(std_struct: Module):
+    await Boot.create(std_struct)
 
 
-@fixture
-def std_mongo_boot(std_struct: Module) -> Boot:
-    return Boot(
+@pytest_asyncio.fixture
+async def std_mongo_boot(std_struct: Module) -> Boot:
+    return await Boot.create(
         root_module=std_struct
     )
 
 
-@fixture
+@pytest.fixture
 def set_prod_mode():
     os.environ["ORWYNN_MODE"] = "prod"
 
 
-@fixture
+@pytest.fixture
 def set_dev_mode():
     os.environ["ORWYNN_MODE"] = "dev"
 
 
-@fixture
+@pytest.fixture
 def set_test_mode():
     os.environ["ORWYNN_MODE"] = "test"
 
 
-@fixture
+@pytest.fixture
 def set_std_apprc_path_env() -> None:
     os.environ["ORWYNN_APPRC_PATH"] = os.path.join(
         os.getcwd(),
         "tests/std/apprc.yml"
     )
 
 
-def test_init_mode_default(std_struct: Module):
+@pytest.mark.asyncio
+async def test_init_mode_default(std_struct: Module):
     os.environ["ORWYNN_MODE"] = ""
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=std_struct
     )
     assert boot.mode == AppMode.DEV
 
 
-def test_init_mode_test(std_struct: Module):
+@pytest.mark.asyncio
+async def test_init_mode_test(std_struct: Module):
     os.environ["ORWYNN_MODE"] = "test"
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=std_struct
     )
     assert boot.mode == AppMode.TEST
 
 
-def test_init_mode_dev(std_struct: Module):
+@pytest.mark.asyncio
+async def test_init_mode_dev(std_struct: Module):
     os.environ["ORWYNN_MODE"] = "dev"
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=std_struct
     )
     assert boot.mode == AppMode.DEV
 
 
-def test_init_mode_prod(std_struct: Module):
+@pytest.mark.asyncio
+async def test_init_mode_prod(std_struct: Module):
     os.environ["ORWYNN_MODE"] = "prod"
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=std_struct
     )
     assert boot.mode == AppMode.PROD
 
 
-def test_init_incorrect_mode(std_struct: Module):
+@pytest.mark.asyncio
+async def test_init_incorrect_mode(std_struct: Module):
     os.environ["ORWYNN_MODE"] = "helloworld"
-    validation.expect(Boot, ValueError, root_module=std_struct)
+    await validation.expect_async(
+        Boot.create(root_module=std_struct),
+        ValueError
+    )
 
 
-def test_init_enable_mongo(std_struct: Module, set_std_apprc_path_env):
-    Boot(
+@pytest.mark.asyncio
+async def test_init_enable_mongo(std_struct: Module, set_std_apprc_path_env):
+    await Boot.create(
         root_module=std_struct
     )
 
     validation.validate(Di.ie().find("Mongo"), Mongo)
 
 
-def test_nested_configs_prod(
+@pytest.mark.asyncio
+async def test_nested_configs_prod(
     std_struct: Module,
     set_std_apprc_path_env,
     set_prod_mode
 ):
-    Boot(
+    await Boot.create(
         root_module=std_struct
     )
     app_rc: AppRc = BootProxy.ie().apprc
     text_config: TextConfig = Di.ie().find("TextConfig")
 
     assert app_rc["Text"]["words_amount"] == text_config.words_amount == 1
 
 
-def test_nested_configs_dev(
+@pytest.mark.asyncio
+async def test_nested_configs_dev(
     std_struct: Module,
     set_std_apprc_path_env,
     set_dev_mode
 ):
-    Boot(
+    await Boot.create(
         root_module=std_struct
     )
     app_rc: AppRc = BootProxy.ie().apprc
     text_config: TextConfig = Di.ie().find("TextConfig")
 
     assert app_rc["Text"]["words_amount"] == text_config.words_amount == 2
 
 
-def test_nested_configs_test(
+@pytest.mark.asyncio
+async def test_nested_configs_test(
     std_struct: Module,
     set_std_apprc_path_env,
     set_test_mode
 ):
-    Boot(
+    await Boot.create(
         root_module=std_struct
     )
     app_rc: AppRc = BootProxy.ie().apprc
     text_config: TextConfig = Di.ie().find("TextConfig")
 
     assert app_rc["Text"]["words_amount"] == text_config.words_amount == 3
 
@@ -155,53 +167,56 @@
 def __gmodule() -> Module:
     return Module(
         "/gmodule",
         Providers=[_GService],
         exports=[_GService]
     )
 
-def test_global_modules(
+@pytest.mark.asyncio
+async def test_global_modules(
     __gmodule: Module
 ):
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def __init__(self, gservice: _GService) -> None:
             super().__init__()
             self.__gservice: _GService = gservice
 
         def get(self) -> dict:
             return {"value": self.__gservice.calculate(1, 2, 3)}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/", Controllers=[C1]),
         global_modules=[__gmodule]
     )
 
     data: dict = boot.app.client.get_jsonify("/", 200)
 
     assert data["value"] == 6
 
 
-def test_global_modules_reimported(
+@pytest.mark.asyncio
+async def test_global_modules_reimported(
     __gmodule: Module
 ):
     """No module can import globally-defined modules."""
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def __init__(self, gservice: _GService) -> None:
             super().__init__()
             self.__gservice: _GService = gservice
 
         def get(self) -> dict:
             return {"value": self.__gservice.calculate(1, 2, 3)}
 
-    validation.expect(
-        Boot,
-        CircularDependencyError,
-        # Root module reimports globally defined module
-        root_module=Module("/", Controllers=[C1], imports=[__gmodule]),
-        global_modules=[__gmodule]
+    await validation.expect_async(
+        Boot.create(
+            # Root module reimports globally defined module
+            root_module=Module("/", Controllers=[C1], imports=[__gmodule]),
+            global_modules=[__gmodule]
+        ),
+        CircularDependencyError
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/bootscript/test_main.py` & `orwynn-1.0.0rc2/orwynn/bootscript/test_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from orwynn.base.module import Module
 from orwynn.base.service import Service
 from orwynn.boot import Boot
 from orwynn.bootscript.bootscript import Bootscript
 from orwynn.bootscript.calltime import CallTime
 from orwynn.di.di import Di
 from orwynn.utils import validation
@@ -9,24 +11,49 @@
 
 class SomeService(Service):
     def __init__(self) -> None:
         super().__init__()
         self.some_var: int = 0
 
 
-def some_bootscript(some_service: SomeService) -> None:
+def fn(some_service: SomeService) -> None:
     some_service.some_var = 1
 
 
-def test_basic():
-    Boot(
+async def async_fn(some_service: SomeService) -> None:
+    some_service.some_var = 5
+
+
+@pytest.mark.asyncio
+async def test_basic():
+    await Boot.create(
+        Module(Providers=[SomeService]),
+        bootscripts=[
+            Bootscript(
+                fn=fn,
+                call_time=CallTime.AFTER_ALL
+            )
+        ]
+    )
+
+    some_service: SomeService = validation.apply(
+        Di.ie().find("SomeService"),
+        SomeService
+    )
+
+    assert some_service.some_var == 1
+
+
+@pytest.mark.asyncio
+async def test_async():
+    await Boot.create(
         Module(Providers=[SomeService]),
         bootscripts=[
             Bootscript(
-                fn=some_bootscript,
+                fn=fn,
                 call_time=CallTime.AFTER_ALL
             )
         ]
     )
 
     some_service: SomeService = validation.apply(
         Di.ie().find("SomeService"),
```

### Comparing `orwynn-1.0.0rc1/orwynn/bootscript/worker.py` & `orwynn-1.0.0rc2/orwynn/bootscript/worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import inspect
+
 from orwynn.base.worker import Worker
 from orwynn.bootscript.bootscript import Bootscript
 from orwynn.bootscript.calltime import CallTime
 from orwynn.bootscript.errors import (
     NoScriptsForCallTimeError,
     ScriptsAlreadyCalledError,
 )
 from orwynn.di.collecting.acceptordependencies import (
     collect_dependencies_for_acceptor,
 )
 from orwynn.di.container import DiContainer
+from orwynn.di.provider import Provider
 
 _IsCallPerformed = bool
 # Represents bootscripts sorted by their call time and followed by
 # a flag signified whether the call was already performed
 _ScriptsState = tuple[list[Bootscript], _IsCallPerformed]
 _CallState = dict[CallTime, _ScriptsState]
 
@@ -33,15 +36,15 @@
 
         for bs in self.__bootscripts:
             state.setdefault(bs.call_time, ([], False))
             state[bs.call_time][0].append(bs)
 
         return state
 
-    def call_by_time(
+    async def call_by_time(
         self,
         call_time: CallTime,
         di_container: DiContainer
     ) -> None:
         try:
             scripts_state: _ScriptsState = \
                 self.__call_state[call_time]
@@ -52,22 +55,25 @@
         else:
             if scripts_state[1] is True:
                 raise ScriptsAlreadyCalledError(
                     f"scripts for time {call_time} were already called"
                 )
             else:
                 for script in scripts_state[0]:
-                    self.__call_script(script, di_container)
+                    await self.__call_script(script, di_container)
                 scripts_state = (scripts_state[0], True)
 
-    def __call_script(
+    async def __call_script(
         self,
         script: Bootscript,
         di_container: DiContainer
     ) -> None:
-        script.fn(
-            **collect_dependencies_for_acceptor(
-                acceptor_callable=script.fn,
-                container=di_container,
-                acceptor_module=None
-            )
+        dependencies: dict[str, Provider] = collect_dependencies_for_acceptor(
+            acceptor_callable=script.fn,
+            container=di_container,
+            acceptor_module=None
         )
+
+        if inspect.iscoroutinefunction(script.fn):
+            await script.fn(**dependencies)
+        else:
+            script.fn(**dependencies)  # type: ignore
```

### Comparing `orwynn-1.0.0rc1/orwynn/context/manager.py` & `orwynn-1.0.0rc2/orwynn/context/manager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/context/storage.py` & `orwynn-1.0.0rc2/orwynn/context/storage.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/availability.py` & `orwynn-1.0.0rc2/orwynn/di/availability.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/acceptordependencies.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/acceptordependencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import inspect
-from typing import Callable
+from typing import Callable, Coroutine
 
 from orwynn.base.middleware import Middleware
 from orwynn.base.module import Module
 from orwynn.di.availability import check_availability
 from orwynn.di.container import DiContainer
 from orwynn.di.object import DiObject
 from orwynn.di.provider import Provider
 
 
 def collect_dependencies_for_acceptor(
-    acceptor_callable: Callable,
+    acceptor_callable: Callable | Coroutine,
     container: DiContainer,
     acceptor_module: Module | None
 ) -> dict[str, Provider]:
     """
     Collects all dependencies for given acceptor.
 
     Note that availabily check won't be performed in any of two cases:
```

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/errors.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/helpers.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/modulecollector.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/modulecollector.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/collect.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/collect.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/map.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/map.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/test_main.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/providerdependencies/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 
-from pytest import fixture
+import pytest
 
 from orwynn.base.config import Config
 from orwynn.base.module import Module
 from orwynn.di.collecting.modulecollector import ModuleCollector
 from orwynn.di.collecting.providerdependencies.collect import (
     collect_provider_dependencies,
 )
@@ -13,15 +13,15 @@
 )
 from orwynn.di.isprovider import is_provider
 from orwynn.di.provider import Provider
 from orwynn.log import LogConfig
 from tests.std.assertion import Assertion
 
 
-@fixture
+@pytest.fixture
 def std_provider_dependencies_map(
     std_modules: list[Module]
 ) -> ProviderDependenciesMap:
     return collect_provider_dependencies(std_modules)
 
 
 def test_std(std_struct: Module):
```

### Comparing `orwynn-1.0.0rc1/orwynn/di/collecting/test_modules.py` & `orwynn-1.0.0rc2/orwynn/di/collecting/test_modules.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/constants.py` & `orwynn-1.0.0rc2/orwynn/di/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/container.py` & `orwynn-1.0.0rc2/orwynn/di/container.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/di.py` & `orwynn-1.0.0rc2/orwynn/di/di.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/errors.py` & `orwynn-1.0.0rc2/orwynn/di/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/init/acceptors.py` & `orwynn-1.0.0rc2/orwynn/di/init/acceptors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/init/providers.py` & `orwynn-1.0.0rc2/orwynn/di/init/providers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/di/init/test_acceptors.py` & `orwynn-1.0.0rc2/orwynn/di/init/test_acceptors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+import pytest
+
 from orwynn.base.module import Module
 from orwynn.base.service import Service
 from orwynn.boot.boot import Boot
 from orwynn.di.container import DiContainer
 from orwynn.di.errors import ProviderAvailabilityError
 from orwynn.di.init.acceptors import init_other_acceptors
 from orwynn.http import Endpoint, HttpController, HttpMiddleware
 from orwynn.utils import validation
 from tests.std.assertion import Assertion
 
 
-def test_std(
+@pytest.mark.asyncio
+async def test_std(
     std_di_container: DiContainer,
     std_modules: list[Module]
 ):
     init_other_acceptors(std_di_container, std_modules)
 
     for A in Assertion.COLLECTED_OTHER_ACCEPTORS:
         isinstance(std_di_container.find(A.__name__), A)
 
 
-def test_controller_dependency_unavailability():
+@pytest.mark.asyncio
+async def test_controller_dependency_unavailability():
     """
     Controller shouldn't be allowed to request unavailable modules.
     """
     class UnavailableService(Service):
         pass
 
     class Ctrl1(HttpController):
@@ -37,22 +41,24 @@
 
         def get(self) -> dict:
             return {}
 
     key_module: Module = Module("/key", Controllers=[Ctrl1])
     unavailable_module: Module = Module(Providers=[UnavailableService])
 
-    validation.expect(
-        Boot,
-        ProviderAvailabilityError,
-        root_module=Module("/", imports=[key_module, unavailable_module])
+    await validation.expect_async(
+        Boot.create(
+            root_module=Module("/", imports=[key_module, unavailable_module])
+        ),
+        ProviderAvailabilityError
     )
 
 
-def test_middleware_dependency_unavailability():
+@pytest.mark.asyncio
+async def test_middleware_dependency_unavailability():
     """
     Middleware shouldn't be allowed to request unavailable modules.
     """
     class UnavailableService(Service):
         pass
 
     class Mw1(HttpMiddleware):
@@ -60,22 +66,24 @@
             self, covered_routes: list[str], sv: UnavailableService
         ) -> None:
             super().__init__(covered_routes)
 
     key_module: Module = Module("/key", Middleware=[Mw1])
     unavailable_module: Module = Module(Providers=[UnavailableService])
 
-    validation.expect(
-        Boot,
-        ProviderAvailabilityError,
-        root_module=Module("/", imports=[key_module, unavailable_module])
+    await validation.expect_async(
+        Boot.create(
+            root_module=Module("/", imports=[key_module, unavailable_module])
+        ),
+        ProviderAvailabilityError
     )
 
 
-def test_unavailability_imported_but_not_exported():
+@pytest.mark.asyncio
+async def test_unavailability_imported_but_not_exported():
     """
     Check that a provider is not available if it's not exported from an
     imported module
     """
     class UnavailableService(Service):
         pass
 
@@ -92,12 +100,13 @@
             return {}
 
     unavailable_module: Module = Module(Providers=[UnavailableService])
     key_module: Module = Module(
         "/key", Controllers=[Ctrl1], imports=[unavailable_module]
     )
 
-    validation.expect(
-        Boot,
-        ProviderAvailabilityError,
-        root_module=Module("/", imports=[key_module, unavailable_module])
+    await validation.expect_async(
+        Boot.create(
+            root_module=Module("/", imports=[key_module, unavailable_module])
+        ),
+        ProviderAvailabilityError
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/helpers/constants.py` & `orwynn-1.0.0rc2/orwynn/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/helpers/web.py` & `orwynn-1.0.0rc2/orwynn/helpers/web.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A request of any supported protocol
 from enum import Enum
 from typing import TYPE_CHECKING, Union
 
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 
 if TYPE_CHECKING:
     from orwynn.http import HttpRequest, HttpResponse
     from orwynn.websocket import Websocket
 
 
 GenericRequest = Union[
@@ -31,20 +31,20 @@
     PUT = "put"
     DELETE = "delete"
     PATCH = "patch"
     OPTIONS = "options"
     WEBSOCKET = "websocket"
 
 
-REQUEST_METHOD_BY_PROTOCOL: dict[Protocol, list[RequestMethod]] = {
-    Protocol.HTTP: [
+REQUEST_METHOD_BY_PROTOCOL: dict[Scheme, list[RequestMethod]] = {
+    Scheme.HTTP: [
         RequestMethod.GET,
         RequestMethod.POST,
         RequestMethod.PUT,
         RequestMethod.DELETE,
         RequestMethod.PATCH,
         RequestMethod.OPTIONS,
     ],
-    Protocol.WEBSOCKET: [
+    Scheme.WEBSOCKET: [
         RequestMethod.WEBSOCKET
     ]
 }
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/__init__.py` & `orwynn-1.0.0rc2/orwynn/http/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/constants.py` & `orwynn-1.0.0rc2/orwynn/http/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/context/id.py` & `orwynn-1.0.0rc2/orwynn/http/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/context/middleware/builtin.py` & `orwynn-1.0.0rc2/orwynn/http/context/middleware/builtin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/context/middleware/contextbuiltin.py` & `orwynn-1.0.0rc2/orwynn/http/context/middleware/contextbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/context/test_main.py` & `orwynn-1.0.0rc2/orwynn/http/context/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.context.errors import UndefinedStorageError
 from orwynn.http import (
     Endpoint,
     HttpController,
     HttpRequestContextId,
     LogMiddleware,
 )
 from orwynn.utils import validation
 
 
-def test_basic():
+@pytest.mark.asyncio
+async def test_basic():
     """Request id should be fetchable from context within request-response
     cycle and unfetchable outside this cycle.
     """
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"request_id": HttpRequestContextId().get()}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(
             "/",
             Controllers=[C1],
             Middleware=[LogMiddleware]
         )
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/controller/controller.py` & `orwynn-1.0.0rc2/orwynn/http/controller/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, ClassVar, Literal
 
 from orwynn.helpers.web import REQUEST_METHOD_BY_PROTOCOL, RequestMethod
 
 from .endpoint.endpoint import Endpoint
 from orwynn.base.controller.controller import Controller
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 from orwynn.http.errors import UnsupportedHttpMethodError
 from .errors import \
     DefinedTwiceControllerMethodError
 from orwynn.base.controller.errors import \
     MissingControllerClassAttributeError
 from .endpoint.container import EndpointContainer
 from orwynn.utils import validation
@@ -59,15 +59,15 @@
             )
             collected_str_methods: list[str] = []
             for endpoint in self.ENDPOINTS:
                 str_method = endpoint.method.lower()
 
                 http_methods: list[RequestMethod] = [
                     method.value
-                    for method in REQUEST_METHOD_BY_PROTOCOL[Protocol.HTTP]
+                    for method in REQUEST_METHOD_BY_PROTOCOL[Scheme.HTTP]
                 ]
                 if str_method not in http_methods:
                     raise UnsupportedHttpMethodError(
                         f"method {str_method} is not supported"
                     )
                 if str_method in collected_str_methods:
                     raise DefinedTwiceControllerMethodError(
@@ -76,15 +76,15 @@
                     )
 
                 collected_str_methods.append(str_method)
                 http_method: RequestMethod = RequestMethod(str_method)
 
                 if (
                     http_method
-                    not in REQUEST_METHOD_BY_PROTOCOL[Protocol.HTTP]
+                    not in REQUEST_METHOD_BY_PROTOCOL[Scheme.HTTP]
                 ):
                     raise ValueError(f"cannot accept method {http_method}")
 
                 self._methods.append(http_method)
 
                 EndpointContainer.ie().add(
                     self.get_fn_by_http_method(http_method),
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/controller/endpoint/container.py` & `orwynn-1.0.0rc2/orwynn/http/controller/endpoint/container.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/controller/endpoint/endpoint.py` & `orwynn-1.0.0rc2/orwynn/http/controller/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/controller/endpoint/test_main.py` & `orwynn-1.0.0rc2/orwynn/http/controller/endpoint/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from pytest import fixture
+import pytest
+import pytest_asyncio
 
 from orwynn import mongo
 from orwynn.base.model.model import Model
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.http import Endpoint, EndpointResponse, HttpController
 from orwynn.router.errors import (
     UnmatchedEndpointEntityError,
 )
 from orwynn.utils import validation
 
 
-@fixture
-def run_endpoint():
+@pytest_asyncio.fixture
+async def run_endpoint():
     class Item(Model):
         name: str
         price: int
 
     class Response400(Model):
         message: str
         power: float
@@ -43,15 +44,15 @@
                 ]
             )
         ]
 
         def get(self) -> Item:
             return Item(name="hello", price=1)
 
-    Boot(
+    await Boot.create(
         Module(
             route="/",
             Controllers=[C1],
             imports=[mongo.module]
         ),
         apprc={
             "test": {
@@ -59,15 +60,16 @@
                     "database_name": "orwynn-test"
                 }
             }
         }
     )
 
 
-def test_not_matched_spec_to_return_type():
+@pytest.mark.asyncio
+async def test_not_matched_spec_to_return_type():
     class WrongItem(Model):
         name: str
         doubt: int
 
     class Item(Model):
         name: str
         price: float
@@ -80,15 +82,16 @@
                 responses=[EndpointResponse(status_code=200, Entity=WrongItem)]
             )
         ]
 
         def get(self) -> Item:
             return Item(name="hello", price=1.2)
 
-    validation.expect(
-        Boot,
-        UnmatchedEndpointEntityError,
-        Module(
-            route="/",
-            Controllers=[C1]
-        )
+    await validation.expect_async(
+        Boot.create(
+            Module(
+                route="/",
+                Controllers=[C1]
+            )
+        ),
+        UnmatchedEndpointEntityError
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/controller/test_main.py` & `orwynn-1.0.0rc2/orwynn/http/controller/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import pytest
 from fastapi import Query, Request
 
 from orwynn.apiversion import ApiVersion
 from orwynn.base.controller.errors import (
     AlreadyRegisteredMethodError,
     MissingControllerClassAttributeError,
 )
@@ -13,118 +14,148 @@
 from orwynn.helpers.web import REQUEST_METHOD_BY_PROTOCOL
 from orwynn.http import Endpoint, HttpController
 from orwynn.http.controller.errors import DefinedTwiceControllerMethodError
 from orwynn.http.errors import HttpException, UnsupportedHttpMethodError
 from orwynn.proxy.boot import BootProxy
 from orwynn.testing import Client
 from orwynn.utils import validation
-from orwynn.utils.protocol import Protocol
-from orwynn.utils.validation import expect, validate_re
+from orwynn.utils.scheme import Scheme
+from orwynn.utils.validation import validate_re
 from orwynn.utils.validation.errors import (
     RequestValidationException,
     ReValidationError,
     ValidationError,
 )
 from tests.std.text import DEFAULT_ID, Text
 
 
 def test_http_methods():
-    for method in REQUEST_METHOD_BY_PROTOCOL[Protocol.HTTP]:
+    for method in REQUEST_METHOD_BY_PROTOCOL[Scheme.HTTP]:
         assert hasattr(HttpController, method.value)
 
 
-def test_undefined_route():
+@pytest.mark.asyncio
+async def test_undefined_route():
     class C1(HttpController):
         ENDPOINTS = [Endpoint(method="get")]
 
     m1 = Module(route="/", Controllers=[C1])
-    expect(Boot, MissingControllerClassAttributeError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        MissingControllerClassAttributeError
+    )
 
 
-def test_invalid_route():
+@pytest.mark.asyncio
+async def test_invalid_route():
     class C1(HttpController):
         ROUTE = "i don't like rules"
         ENDPOINTS = [Endpoint(method="get")]
 
     m1 = Module(route="/", Controllers=[C1])
-    expect(Boot, ReValidationError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        ReValidationError
+    )
 
 
-def test_undefined_endpoints():
+@pytest.mark.asyncio
+async def test_undefined_endpoints():
     class C1(HttpController):
         ROUTE = "/c1"
 
     m1 = Module(route="/", Controllers=[C1])
-    expect(Boot, MissingControllerClassAttributeError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        MissingControllerClassAttributeError
+    )
 
 
-def test_empty_endpoints():
+@pytest.mark.asyncio
+async def test_empty_endpoints():
     class C1(HttpController):
         ROUTE = "/c1"
         ENDPOINTS = []
 
     m1 = Module(route="/", Controllers=[C1])
-    expect(Boot, ValidationError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        ValidationError
+    )
 
 
-def test_unsupported_method():
+@pytest.mark.asyncio
+async def test_unsupported_method():
     class C1(HttpController):
         ROUTE = "/c1"
         ENDPOINTS = [Endpoint(method="donuts")]
 
     m1 = Module(route="/", Controllers=[C1])
-    expect(Boot, UnsupportedHttpMethodError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        UnsupportedHttpMethodError
+    )
 
 
-def test_defined_twice_method():
+@pytest.mark.asyncio
+async def test_defined_twice_method():
     class C1(HttpController):
         ROUTE = "/c1"
         ENDPOINTS = [Endpoint(method="get"), Endpoint(method="get")]
 
     m1 = Module(route="/", Controllers=[C1])
-    expect(Boot, DefinedTwiceControllerMethodError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        DefinedTwiceControllerMethodError
+    )
 
 
-def test_uppercase_methods():
+@pytest.mark.asyncio
+async def test_uppercase_methods():
     class C1(HttpController):
         ROUTE = "/c1"
         ENDPOINTS = [
             Endpoint(method="GET"),
             Endpoint(method="POST")
         ]
 
     m1 = Module(route="/", Controllers=[C1])
-    Boot(m1)
+    await Boot.create(m1)
 
 
-def test_already_registered():
+@pytest.mark.asyncio
+async def test_already_registered():
     class C1(HttpController):
         ROUTE = "/hello"
         ENDPOINTS = [Endpoint(method="get")]
 
     class C2(HttpController):
         ROUTE = "/hello"
         ENDPOINTS = [Endpoint(method="get")]
 
     m1 = Module(route="/", Controllers=[C1, C2])
-    expect(Boot, AlreadyRegisteredMethodError, m1)
+    await validation.expect_async(
+        Boot.create(m1),
+        AlreadyRegisteredMethodError
+    )
 
 
 def test_std_routes(std_boot: Boot, std_http: Client):
     json: dict = std_http.get_jsonify("/text")
     text: Text = Text.recover(json)
     validate_re(text.text, DEFAULT_ID + r"\: .+")
 
 
-def test_default_404():
+@pytest.mark.asyncio
+async def test_default_404():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1])
     )
 
     data: dict = boot.app.client.get_jsonify(
         "/pizza",
         404
     )
@@ -137,29 +168,30 @@
         HttpException
     )
 
     assert recovered_exception.status_code == 404
     assert recovered_exception.detail == "Not Found"
 
 
-def test_default_request_validation_error():
+@pytest.mark.asyncio
+async def test_default_request_validation_error():
     class Item(Model):
         name: str
         price: float
 
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="post")]
 
         def post(self, item: Item) -> dict:
             return {}
 
-    data: dict = Boot(
+    data: dict = (await Boot.create(
         Module(route="/", Controllers=[C1])
-    ).app.client.post_jsonify(
+    )).app.client.post_jsonify(
         "/",
         422,
         json={
             "name": 222,
             "price": "hello"
         }
     )
@@ -171,25 +203,26 @@
             RequestValidationException,
             data
         ),
         RequestValidationException
     )
 
 
-def test_default_method_not_allowed():
+@pytest.mark.asyncio
+async def test_default_method_not_allowed():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {}
 
-    data: dict = Boot(
+    data: dict = (await Boot.create(
         Module(route="/", Controllers=[C1])
-    ).app.client.post_jsonify(
+    )).app.client.post_jsonify(
         "/",
         405
     )
 
     recovered_exception: HttpException = validation.apply(
         BootProxy.ie().api_indication.recover(
             HttpException,
@@ -198,43 +231,45 @@
         HttpException
     )
 
     assert recovered_exception.status_code == 405
     assert recovered_exception.detail == "Method Not Allowed"
 
 
-def test_final_routes():
+@pytest.mark.asyncio
+async def test_final_routes():
     class _Ctrl(HttpController):
         ROUTE = "/{id}/tasty"
         ENDPOINTS = [
             Endpoint(method="get")
         ]
 
-    Boot(
+    await Boot.create(
         Module("/donuts", Controllers=[_Ctrl]),
         global_http_route="/api/v{version}"
     )
 
     ctrl: HttpController = validation.apply(
         Di.ie().find("_Ctrl"),
         HttpController
     )
 
     assert "/api/v1/donuts/{id}/tasty" in ctrl.final_routes
 
 
-def test_is_matching_route():
+@pytest.mark.asyncio
+async def test_is_matching_route():
     class _Ctrl(HttpController):
         ROUTE = "/{id}/tasty"
         ENDPOINTS = [
             Endpoint(method="get")
         ]
         VERSION = 2
 
-    Boot(
+    await Boot.create(
         Module("/donuts", Controllers=[_Ctrl]),
         global_http_route="/api/v{version}",
         api_version=ApiVersion(supported={1, 2, 3})
     )
 
     ctrl: HttpController = validation.apply(
         Di.ie().find("_Ctrl"),
@@ -251,15 +286,16 @@
 
     assert ctrl.is_matching_route("/api/v2/donuts/e67840v/tasty/gogo") is False
     assert ctrl.is_matching_route("/api/v2/donuts/tasty") is False
     assert ctrl.is_matching_route("/api/donuts/eb00v/tasty") is False
     assert ctrl.is_matching_route("/donuts/eb00v/tasty") is False
 
 
-def test_multiple_query_params():
+@pytest.mark.asyncio
+async def test_multiple_query_params():
     """
     Should correctly parse list of query params.
     """
     class _Ctrl(HttpController):
         ROUTE = "/items"
         ENDPOINTS = [
             Endpoint(method="get")
@@ -270,15 +306,15 @@
             request: Request,
             q: list[str] | None = Query(None)
         ) -> dict:
             return {
                 "q": q
             }
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[_Ctrl])
     )
 
     data: dict = boot.client.get_jsonify(
         "/items?q=1&q=2",
         200
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/cors/test_main.py` & `orwynn-1.0.0rc2/orwynn/http/cors/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.http.controller.controller import HttpController
 from orwynn.http.controller.endpoint.endpoint import Endpoint
 from orwynn.testing.client import Client
 
 
-def test_basic():
+@pytest.mark.asyncio
+async def test_basic():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self):
             return {}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1]),
         apprc={
             "prod": {
                 "App": {
                     "cors": {
                         "is_enabled": True,
                         "allow_origins": ["*"]
@@ -35,23 +38,24 @@
             "access-control-request-method": "GET"
         }
     )
 
     assert r.headers.get("access-control-allow-origin") == "*"
 
 
-def test_correct_origin():
+@pytest.mark.asyncio
+async def test_correct_origin():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1]),
         apprc={
             "prod": {
                 "App": {
                     "cors": {
                         "is_enabled": True,
                         "allow_origins": ["hello"]
@@ -70,20 +74,21 @@
             "access-control-request-method": "POST"
         }
     )
 
     assert r.headers.get("access-control-allow-origin") == "hello"
 
 
-def test_wrong_origin():
+@pytest.mark.asyncio
+async def test_wrong_origin():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1]),
         apprc={
             "prod": {
                 "App": {
                     "cors": {
                         "is_enabled": True,
                         "allow_origins": ["nothello"]
@@ -101,26 +106,27 @@
             "access-control-request-method": "POST"
         }
     )
 
     assert r.headers.get("access-control-allow-origin") is None
 
 
-def test_unsuccessful():
+@pytest.mark.asyncio
+async def test_unsuccessful():
     """
     Unsuccessful responses should also contain according CORS headers.
     """
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self):
             raise ValueError("cors test")
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1]),
         apprc={
             "prod": {
                 "App": {
                     "cors": {
                         "is_enabled": True,
                         "allow_origins": ["*"]
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/errorhandler/default.py` & `orwynn-1.0.0rc2/orwynn/http/errorhandler/default.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/errorhandler/middleware.py` & `orwynn-1.0.0rc2/orwynn/http/errorhandler/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/errorhandler/test_main.py` & `orwynn-1.0.0rc2/orwynn/http/errorhandler/test_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from orwynn.base.error.errors import ExceptionAlreadyHandledError
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.base.module import Module
 from orwynn.base.service.service import Service
 from orwynn.boot.boot import Boot
 from orwynn.http.context.middleware.contextbuiltin import (
     HttpRequestContextBuiltinMiddleware,
@@ -38,23 +40,24 @@
     ROUTE = "/"
     ENDPOINTS = [Endpoint(method="get")]
 
     def get(self):
         raise ValueError("hello")
 
 
-def test_custom_handler():
+@pytest.mark.asyncio
+async def test_custom_handler():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self):
             raise ValueError("whoops!")
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1]),
         ErrorHandlers={GeneralEh}
     )
     http: Client = boot.app.client
 
     r: TestHttpResponse = http.get("/", 401)
 
@@ -62,38 +65,40 @@
         BootProxy.ie().api_indication.recover(ValueError, r.json()),
         ValueError
     )
 
     assert recovered_error.args[0] == "whoops!"
 
 
-def test_default_exception():
+@pytest.mark.asyncio
+async def test_default_exception():
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self):
             raise TypeError("whoops!")
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1])
     )
     http: Client = boot.app.client
 
     r: TestHttpResponse = http.get("/", 400)
 
     recovered_exception: TypeError = validation.apply(
         BootProxy.ie().api_indication.recover(TypeError, r.json()),
         TypeError
     )
 
     assert recovered_exception.args[0] == "whoops!"
 
 
-def test_as_acceptor():
+@pytest.mark.asyncio
+async def test_as_acceptor():
     """
     Tests if an error handler can truly accept Providers.
     """
     ASSERTED_TEXT: str = "Hello, world!"
 
     class CoolService(Service):
         def do_something(
@@ -119,26 +124,27 @@
             request: HttpRequest,
             error: Exception
         ) -> HttpResponse:
             data: dict = BootProxy.ie().api_indication.digest(error)
             data["__test_meta_info"] = self.__cool_service.do_something()
             return JsonHttpResponse(data, 400)
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Providers=[CoolService], Controllers=[C1]),
         ErrorHandlers={Eh1}
     )
     client: Client = boot.app.client
 
     data: dict = client.get_jsonify("/", 400)
 
     assert data["__test_meta_info"] == ASSERTED_TEXT
 
 
-def test_default_in_middleware():
+@pytest.mark.asyncio
+async def test_default_in_middleware():
     """
     Should handle exceptions occured in middleware.
     """
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
@@ -149,29 +155,30 @@
         async def process(
             self,
             request: HttpRequest,
             call_next: HttpNextCall
         ) -> HttpResponse:
             raise ValueError("whoops!")
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1], Middleware=[M1])
     )
 
     r: TestHttpResponse = boot.app.client.get("/", 400)
 
     recovered_exception: Exception = validation.apply(
         BootProxy.ie().api_indication.recover(Exception, r.json()),
         Exception
     )
 
     assert recovered_exception.args[0] == "whoops!"
 
 
-def test_custom_in_middleware():
+@pytest.mark.asyncio
+async def test_custom_in_middleware():
     """
     Should handle exceptions occured in middleware.
     """
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
@@ -182,45 +189,48 @@
         async def process(
             self,
             request: HttpRequest,
             call_next: HttpNextCall
         ) -> HttpResponse:
             raise ValueError("whoops!")
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(route="/", Controllers=[C1], Middleware=[M1]),
         ErrorHandlers={GeneralEh}
     )
 
     r: TestHttpResponse = boot.app.client.get("/", 401)
 
     recovered: ValueError = validation.apply(
         BootProxy.ie().api_indication.recover(ValueError, r.json()),
         ValueError
     )
 
     assert recovered.args[0] == "whoops!"
 
 
-def test_exception_handled_twice():
+@pytest.mark.asyncio
+async def test_exception_handled_twice():
     """
     Should raise an error for twice-handled exceptions.
     """
     class Eh1(ErrorHandler):
         E = Exception
 
-    validation.expect(
-        Boot,
-        ExceptionAlreadyHandledError,
-        Module("/", Controllers=[RaiseErrorController]),
-        ErrorHandlers={GeneralEh, Eh1}
+    await validation.expect_async(
+        Boot.create(
+            Module("/", Controllers=[RaiseErrorController]),
+            ErrorHandlers={GeneralEh, Eh1}
+        ),
+        ExceptionAlreadyHandledError
     )
 
 
-def test_pydantic_validation_error_is_catched():
+@pytest.mark.asyncio
+async def test_pydantic_validation_error_is_catched():
     """
     Should catch pydantic.ValidationError too, despite it's internal multiple
     inheritance.
     """
     class _Ctrl(HttpController):
         ROUTE = "/"
         ENDPOINTS = [
@@ -228,12 +238,12 @@
         ]
 
         def get(self) -> dict:
             # Invoke a validation error
             Item(name="item", price="whocares")  # type: ignore
             return {}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[_Ctrl])
     )
 
     boot.app.client.get_jsonify("/", 400)
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/log/logger.py` & `orwynn-1.0.0rc2/orwynn/http/log/logger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/log/middleware.py` & `orwynn-1.0.0rc2/orwynn/http/log/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/middleware/middleware.py` & `orwynn-1.0.0rc2/orwynn/http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/middleware/test_main.py` & `orwynn-1.0.0rc2/orwynn/http/middleware/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Callable
 
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.http import (
     Endpoint,
     HttpController,
     HttpMiddleware,
     HttpRequest,
@@ -18,69 +20,72 @@
         self, request: HttpRequest, call_next: Callable
     ) -> HttpResponse:
         response: HttpResponse = await call_next(request)
         response.headers["x-test"] = "hello"
         return response
 
 
-def test_basic():
+@pytest.mark.asyncio
+async def test_basic():
     """
     Should work in general cases.
     """
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self):
             return {"message": "hello"}
 
-    boot: Boot = Boot(Module(
+    boot: Boot = await Boot.create(Module(
         route="/hello/world",
         Controllers=[C1],
         Middleware=[Mw1]
     ))
     http: Client = boot.app.client
     response: TestHttpResponse = http.get("/hello/world")
 
     assert response.headers["x-test"] == "hello"
 
 
-def test_variable_route():
+@pytest.mark.asyncio
+async def test_variable_route():
     """Should work with variable routes.
     """
     class C1(HttpController):
         ROUTE = "/{id}"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self, id: str):
             return {"value": id}
 
-    boot: Boot = Boot(Module(
+    boot: Boot = await Boot.create(Module(
         route="/",
         Controllers=[C1],
         Middleware=[Mw1]
     ))
     http: Client = boot.app.client
     response: TestHttpResponse = http.get("/e201")
 
     assert response.json()["value"] == "e201"
     assert response.headers["x-test"] == "hello"
 
 
-def test_file_path_route():
+@pytest.mark.asyncio
+async def test_file_path_route():
     """Should be OK with file paths.
     """
     class C1(HttpController):
         ROUTE = "/{file_path:path}"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self, file_path: str):
             return {"value": file_path}
 
-    boot: Boot = Boot(Module(
+    boot: Boot = await Boot.create(Module(
         route="/",
         Controllers=[C1],
         Middleware=[Mw1]
     ))
     http: Client = boot.app.client
     response: TestHttpResponse = http.get("/doc/pdf/1234.pdf")
```

### Comparing `orwynn-1.0.0rc1/orwynn/http/responses.py` & `orwynn-1.0.0rc2/orwynn/http/responses.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/http/test_responses.py` & `orwynn-1.0.0rc2/orwynn/http/test_responses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import pytest
+
 from orwynn.base import Module
 from orwynn.boot import Boot
 from orwynn.http import Endpoint, HttpController
 from orwynn.http.log.middleware import LogMiddleware
 from orwynn.http.responses import RedirectHttpResponse, TestHttpResponse
 
 
-def test_redirect():
+@pytest.mark.asyncio
+async def test_redirect():
     class LocalController(HttpController):
         ROUTE = "/"
         ENDPOINTS = [
             Endpoint(
                 method="get"
             )
         ]
 
         def get(self) -> RedirectHttpResponse:
             return RedirectHttpResponse("https://google.com")
 
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[LocalController]),
         global_middleware={
             LogMiddleware: ["*"]
         }
     )  # type: ignore
 
     response: TestHttpResponse = boot.app.client.get(
```

### Comparing `orwynn-1.0.0rc1/orwynn/indication/indication.py` & `orwynn-1.0.0rc2/orwynn/indication/indication.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/indication/test_main.py` & `orwynn-1.0.0rc2/orwynn/indication/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/log/configure.py` & `orwynn-1.0.0rc2/orwynn/log/configure.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/log/handler.py` & `orwynn-1.0.0rc2/orwynn/log/handler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/log/helpers.py` & `orwynn-1.0.0rc2/orwynn/log/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/log/test_main.py` & `orwynn-1.0.0rc2/orwynn/log/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,48 +19,53 @@
 @pytest.fixture
 def log_apprc_sink_to_writer(writer: Writer) -> dict:
     def __check(message: LogMessage) -> None:
         writer.write(message)
     return get_log_apprc(__check)
 
 
-def test_logged_request_id(writer: Writer, log_apprc_sink_to_writer: dict):
+@pytest.mark.asyncio
+async def test_logged_request_id(
+    writer: Writer,
+    log_apprc_sink_to_writer: dict
+):
     class C1(HttpController):
         ROUTE = "/"
         ENDPOINTS = [
             Endpoint(method="get")
         ]
 
         def get(self) -> dict:
             Log.info("hello")
             return {}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[C1]),
         apprc=log_apprc_sink_to_writer
     )
 
     boot.app.client.get("/", 200)
     data: dict = json.loads(str(writer.read()))
     extra: dict = data["record"]["extra"]
 
     assert isinstance(extra["http.request_id"], str)
 
 
-def test_logged_websocket_request_id(
+@pytest.mark.asyncio
+async def test_logged_websocket_request_id(
     writer: Writer,
     log_apprc_sink_to_writer: dict
 ):
     class C1(WebsocketController):
         ROUTE = "/"
 
         async def main(self, websocket: Websocket) -> None:
             Log.info("hello")
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[C1]),
         apprc=log_apprc_sink_to_writer
     )  # type: ignore #worker
 
     with boot.app.client.websocket("/"):
         pass
```

### Comparing `orwynn-1.0.0rc1/orwynn/log/test_websocketmiddleware.py` & `orwynn-1.0.0rc2/orwynn/log/test_websocketmiddleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.log.log import Log
 from orwynn.testing import Writer
 from orwynn.testing.client import Client
 from orwynn.websocket import Websocket, WebsocketController
 from orwynn.websocket.log.middleware import LogWebsocketMiddleware
 
 
-def test_get(
+@pytest.mark.asyncio
+async def test_get(
     writer: Writer,
     log_apprc_sink_to_writer: dict
 ):
     class C1(WebsocketController):
         ROUTE = "/"
 
         async def main(self, websocket: Websocket) -> None:
             await websocket.close()
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(
             route="/", Controllers=[C1], Middleware=[LogWebsocketMiddleware]
         ),
         apprc=log_apprc_sink_to_writer
     )
     client: Client = boot.app.client
```

### Comparing `orwynn-1.0.0rc1/orwynn/mapping/errors.py` & `orwynn-1.0.0rc2/orwynn/mapping/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mapping/mapping.py` & `orwynn-1.0.0rc2/orwynn/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/__init__.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/errors.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/helpers.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/test_converttoobjectid.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/test_converttoobjectid.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/test_get.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/test_get.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/test_inc.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/test_inc.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/test_set.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/test_set.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/test_updateoperators.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/test_updateoperators.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/document/testing.py` & `orwynn-1.0.0rc2/orwynn/mongo/document/testing.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/errors.py` & `orwynn-1.0.0rc2/orwynn/mongo/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/mongo.py` & `orwynn-1.0.0rc2/orwynn/mongo/mongo.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/mongo/test_main.py` & `orwynn-1.0.0rc2/orwynn/mongo/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/proxy/boot.py` & `orwynn-1.0.0rc2/orwynn/proxy/boot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from orwynn.base.worker import Worker
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 
 if TYPE_CHECKING:
     from orwynn.apiversion import ApiVersion
     from orwynn.app import AppMode
     from orwynn.apprc import AppRc
     from orwynn.base.errorhandler.errorhandler import ErrorHandler
     from orwynn.indication.indication import Indication
@@ -83,17 +83,17 @@
 
     @property
     def data(self) -> dict:
         return dict(**self.boot_config_data, **{})
 
     def get_global_route_for_protocol(
         self,
-        protocol: Protocol
+        protocol: Scheme
     ) -> str:
-        if protocol is Protocol.HTTP:
+        if protocol is Scheme.HTTP:
             return self.__global_http_route
-        elif protocol is Protocol.WEBSOCKET:
+        elif protocol is Scheme.WEBSOCKET:
             return self.__global_websocket_route
         else:
             raise TypeError(
                 f"unrecognized protocol {protocol}"
             )
```

### Comparing `orwynn-1.0.0rc1/orwynn/router/errorhandlermanager.py` & `orwynn-1.0.0rc2/orwynn/router/errorhandlermanager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 from orwynn.base.error.errors import (ExceptionAlreadyHandledError,
                                       MalfunctionError)
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.http import DEFAULT_HTTP_ERROR_HANDLERS
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 from orwynn.websocket import DEFAULT_WEBSOCKET_EXCEPTION_HANDLERS
 
 
 class ErrorHandlerManager:
     """
     Controls the error flow setup for the system.
 
     Attributes:
         register_by_protocol:
             Dictionary of register functions for each protocol.
     """
     def get_populated_handlers_by_protocol(
         self,
         exception_handlers: set[ErrorHandler]
-    ) -> dict[Protocol, set[ErrorHandler]]:
+    ) -> dict[Scheme, set[ErrorHandler]]:
         """
         Forms a set of handlers populated with default ones if required.
 
         Args:
             exception_handlers:
                 Set of error handlers to register.
 
         Returns:
             Populated set of exception handlers by their protocol.
         """
-        handlers_by_protocol: dict[Protocol, set[ErrorHandler]] = {}
+        handlers_by_protocol: dict[Scheme, set[ErrorHandler]] = {}
 
         # Populate and register handlers separately for each protocol
-        for protocol in Protocol:
+        for scheme in Scheme:
+            if scheme is not Scheme.HTTP and scheme is not Scheme.WEBSOCKET:
+                continue
+
             populated_handlers: set[ErrorHandler] = \
                 self.__populate_handlers(
                     self.__get_handlers_for_protocol(
-                        protocol,
+                        scheme,
                         exception_handlers
                     ),
-                    protocol
+                    scheme
                 )
 
-            if protocol in handlers_by_protocol:
+            if scheme in handlers_by_protocol:
                 raise ValueError(
-                    f"protocol {protocol} handled twice"
+                    f"protocol {scheme} handled twice"
                 )
-            handlers_by_protocol[protocol] = populated_handlers
+            handlers_by_protocol[scheme] = populated_handlers
 
         return handlers_by_protocol
 
     def __get_handlers_for_protocol(
         self,
-        protocol: Protocol,
+        protocol: Scheme,
         error_handlers: set[ErrorHandler]
     ) -> set[ErrorHandler]:
         """
         Collects all handlers for the given protocol.
         """
         final_set: set[ErrorHandler] = set()
 
@@ -64,15 +67,15 @@
                 final_set.add(eh)
 
         return final_set
 
     def __populate_handlers(
         self,
         error_handlers: set[ErrorHandler],
-        protocol: Protocol
+        protocol: Scheme
     ) -> set[ErrorHandler]:
         """
         Traverses handlers to find handled Python-builtin exceptions.
 
         Returns:
             Set of populated handlers.
         """
@@ -98,17 +101,17 @@
 
             populated_handlers.add(eh)
 
         # Add default handlers for errors for which the custom's handlers were
         # not added
         DEFAULT_HANDLERS: set[type[ErrorHandler]]
         match protocol:
-            case Protocol.HTTP:
+            case Scheme.HTTP:
                 DEFAULT_HANDLERS = DEFAULT_HTTP_ERROR_HANDLERS
-            case Protocol.WEBSOCKET:
+            case Scheme.WEBSOCKET:
                 DEFAULT_HANDLERS = DEFAULT_WEBSOCKET_EXCEPTION_HANDLERS
             case _:
                 raise TypeError(
                     f"unrecognized protocol {protocol}"
                 )
 
         for GenericDefaultErrorHandler in DEFAULT_HANDLERS:
```

### Comparing `orwynn-1.0.0rc1/orwynn/router/register/controller.py` & `orwynn-1.0.0rc2/orwynn/router/register/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 from orwynn.indication.indication import Indication
 from orwynn.proxy.boot import BootProxy
 from orwynn.router.errors import (
     UnmatchedEndpointEntityError,
 )
 from orwynn.utils import validation
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 from orwynn.utils.url import join_routes
 from orwynn.websocket import (
     WebsocketController,
     WebsocketStack,
     routing_handlers,
 )
 
@@ -151,15 +151,15 @@
 
         # At least one method found
         is_method_found: bool = False
         for http_method in RequestMethod:
             # Don't register unused methods
             if (
                 http_method in controller.methods
-                and http_method in REQUEST_METHOD_BY_PROTOCOL[Protocol.HTTP]
+                and http_method in REQUEST_METHOD_BY_PROTOCOL[Scheme.HTTP]
             ):
                 is_method_found = True
 
                 for route in routes:
                     self.__register_http_route(
                         route=route,
                         fn=controller.get_fn_by_http_method(http_method),
```

### Comparing `orwynn-1.0.0rc1/orwynn/router/register/middleware.py` & `orwynn-1.0.0rc2/orwynn/router/register/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     DefaultHttpErrorHandler,
     ErrorHandlerHttpMiddleware,
     HttpMiddleware,
 )
 from orwynn.http.errors import HttpException
 from orwynn.router.errorhandlermanager import ErrorHandlerManager
 from orwynn.utils import validation
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 from orwynn.websocket import (
     BUILTIN_WEBSOCKET_MIDDLEWARE,
     BuiltinWebsocketMiddleware,
     ErrorHandlerWebsocketMiddleware,
     WebsocketMiddleware,
     WebsocketStack,
     routing_handlers,
@@ -56,33 +56,33 @@
         self.__is_websocket_middleware_added: bool = False
 
     def register_all(self) -> None:
         """
         Registers all middleware to the system.
         """
         populated_handlers_py_protocol: dict[
-            Protocol, set[ErrorHandler]
+            Scheme, set[ErrorHandler]
         ] = ErrorHandlerManager().get_populated_handlers_by_protocol(
             self.__exception_handlers
         )
 
         # FIXME: Here below the builtin middleware are created directly without
         #   the Di notifying which may raise a confusion in the next calls.
         #   Also it might become harder to support if an builtin middleware
         #   requests any Di-related dependency.
 
         http_builtin_middleware: Sequence[
             BuiltinHttpMiddleware
         ] = self.__collect_http_builtin_middleware(
-            populated_handlers_py_protocol[Protocol.HTTP]
+            populated_handlers_py_protocol[Scheme.HTTP]
         )
         websocket_builtin_middleware: Sequence[
             BuiltinWebsocketMiddleware
         ] = self.__collect_websocket_builtin_middleware(
-            populated_handlers_py_protocol[Protocol.WEBSOCKET]
+            populated_handlers_py_protocol[Scheme.WEBSOCKET]
         )
 
         self.__register_middleware_arr(
             # Add builtin middlewares first, and others second. No matters the
             # order between middleware of different protocols.
             http_builtin_middleware
             + websocket_builtin_middleware
```

### Comparing `orwynn-1.0.0rc1/orwynn/router/router.py` & `orwynn-1.0.0rc2/orwynn/router/router.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/router/test_globalroute.py` & `orwynn-1.0.0rc2/orwynn/router/test_globalroute.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,97 @@
+import pytest
+
 from orwynn.apiversion import ApiVersion
 from orwynn.base.module import Module
 from orwynn.boot import Boot
 from orwynn.http import Endpoint, HttpController
 
 
-def test_default():
+@pytest.mark.asyncio
+async def test_default():
     """
     By default a client should use the global route.
     """
     class C(HttpController):
         ROUTE = "/message"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C]),
         global_http_route="/donuts"
     )
 
     boot.app.client.get_jsonify("/user/message", 200)
 
 
-def test_default_version():
+@pytest.mark.asyncio
+async def test_default_version():
     """
     By default a client should use the latest api version available.
     """
     class C(HttpController):
         ROUTE = "/message"
         ENDPOINTS = [Endpoint(method="get")]
         VERSION = 3
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C]),
         global_http_route="/api/v{version}",
         api_version=ApiVersion(
             supported={1, 2, 3}
         )
     )
 
     boot.app.client.get_jsonify("/user/message", 200)
 
 
-def test_not_used():
+@pytest.mark.asyncio
+async def test_not_used():
     """
     The global route can be disabled.
     """
     class C(HttpController):
         ROUTE = "/message"
         ENDPOINTS = [Endpoint(method="get")]
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C]),
         global_http_route="/donuts"
     )
 
     boot.app.client.get_jsonify(
         "/donuts/user/message",
         200,
         is_global_route_used=False
     )
 
 
-def test_pass_version():
+@pytest.mark.asyncio
+async def test_pass_version():
     """
     A client is able to not specify global route, but pass own api version.
     """
     class C(HttpController):
         ROUTE = "/message"
         ENDPOINTS = [Endpoint(method="get")]
         VERSION = 2
 
         def get(self) -> dict:
             return {"message": "hello"}
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/user", Controllers=[C]),
         global_http_route="/api/v{version}",
         api_version=ApiVersion(
             supported={1, 2, 3}
         )
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/singleton/singleton.py` & `orwynn-1.0.0rc2/orwynn/singleton/singleton.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/sql/config.py` & `orwynn-1.0.0rc2/orwynn/sql/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/sql/sql.py` & `orwynn-1.0.0rc2/orwynn/sql/sql.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/sql/table.py` & `orwynn-1.0.0rc2/orwynn/sql/table.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/sql/test_main.py` & `orwynn-1.0.0rc2/orwynn/sql/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,16 +223,17 @@
         s.commit()
 
         assert validation.check(s.get(Item, 1)).color == Color.RED
         assert validation.check(s.get(Item, 2)).color == Color.BLUE
         assert validation.check(s.get(Item, 3)).color == Color.GREEN
 
 
-def test_config_poolclass():
-    Boot(
+@pytest.mark.asyncio
+async def test_config_poolclass():
+    await Boot.create(
         Module(imports=[sql.module]),
         apprc={
             "prod": {
                 "Sql": {
                     "database_kind": "sqlite",
                     "database_path": ":memory:",
                     "poolclass": "StaticPool"
```

### Comparing `orwynn-1.0.0rc1/orwynn/testing/__init__.py` & `orwynn-1.0.0rc2/orwynn/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/testing/client.py` & `orwynn-1.0.0rc2/orwynn/testing/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from orwynn.apiversion import ApiVersion
 from orwynn.base.model.model import Model
 from orwynn.proxy.boot import BootProxy
 
 from orwynn.testing.embeddedclient import EmbeddedTestClient
 from orwynn.utils import validation
 from orwynn.utils.validation import validate
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 from orwynn.utils.url import join_routes
 
 if TYPE_CHECKING:
     from orwynn.http import TestHttpResponse
 
 # If ever you get to Python3.12, see if PEP 696 introduced, then apply
 # but for now it is in the next form
@@ -250,15 +250,15 @@
             case _:
                 raise ValueError(f"Method {method} is not supported")
 
         # Get finalized data
         finalized: _FinalizedRequestData = self._process_request_data(
             route=route,
             request_kwargs=request_kwargs,
-            protocol=Protocol.HTTP
+            protocol=Scheme.HTTP
         )
 
         # Make a request
         response: "TestHttpResponse" = test_client_method(
             finalized.route,
             **finalized.kwargs
         )
@@ -273,15 +273,15 @@
         return response
 
     def _process_request_data(
         self,
         *,
         route: str,
         request_kwargs: dict,
-        protocol: Protocol
+        protocol: Scheme
     ) -> _FinalizedRequestData:
         """
         Processes a given route and request kwargs and returns finalized
         versions of them.
         """
         request_kwargs = request_kwargs.copy()
 
@@ -319,15 +319,15 @@
 
     def _get_final_route(
         self,
         route: str,
         *,
         is_global_route_used: bool,
         api_version: int | None,
-        protocol: Protocol
+        protocol: Scheme
     ) -> str:
         if not is_global_route_used and api_version is not None:
             raise ValueError(
                 f"the global route is disabled and api version is also passed"
                 " which doesn't make sense"
             )
         elif not is_global_route_used:
@@ -365,14 +365,14 @@
         self,
         route: str,
         **request_kwargs
     ) -> Any:
         finalized: _FinalizedRequestData = self._process_request_data(
             route=route,
             request_kwargs=request_kwargs,
-            protocol=Protocol.WEBSOCKET
+            protocol=Scheme.WEBSOCKET
         )
 
         return self._embedded_client.websocket_connect(
             finalized.route,
             **finalized.kwargs
         )
```

### Comparing `orwynn-1.0.0rc1/orwynn/testing/test_main.py` & `orwynn-1.0.0rc2/orwynn/testing/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 from fastapi import Header
 
 from orwynn.base.module.module import Module
 from orwynn.boot import Boot
 from orwynn.http import Endpoint, HttpController
 from orwynn.testing.client import Client
 from orwynn.testingtools import HeadersGetController
@@ -32,48 +33,51 @@
     ) -> dict:
         return {
             "x-testing": x_testing or None,
             "x-tmp": x_tmp or None
         }
 
 
-def test_bind_headers():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_bind_headers():
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[_Ctrl1])
     )
 
     binded: Client = boot.app.client.bind_headers({
         "x-testing": "hello"
     })
 
     data: dict = binded.get_jsonify("/")
     assert data["x-testing"] == "hello"
 
 
-def test_bind_headers_accumulate():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_bind_headers_accumulate():
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[_Ctrl2])
     )
 
     binded: Client = boot.app.client.bind_headers({
         "x-testing": "hello"
     }).bind_headers({
         "x-tmp": "world"
     })
 
     data: dict = binded.get_jsonify("/")
     assert data["x-testing"] == "hello"
     assert data["x-tmp"] == "world"
 
-def test_multiple_bind_headers():
+@pytest.mark.asyncio
+async def test_multiple_bind_headers():
     """
     Shouldn't stack bind headers in the original client for subsequent
     bind_headers() calls.
     """
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[HeadersGetController])
     )
 
     binded_1: Client = boot.app.client.bind_headers({
         "x-testing": "hello"
     })
```

### Comparing `orwynn-1.0.0rc1/orwynn/testingtools/__init__.py` & `orwynn-1.0.0rc2/orwynn/testingtools/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/crypto/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/fmt/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/fmt/test_main.py` & `orwynn-1.0.0rc2/orwynn/utils/fmt/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/klass/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/klass/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/klass/test_klass.py` & `orwynn-1.0.0rc2/orwynn/utils/klass/test_klass.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/mp/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/mp/location.py` & `orwynn-1.0.0rc2/orwynn/utils/mp/location.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/mp/test_main.py` & `orwynn-1.0.0rc2/orwynn/utils/mp/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/url/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/url/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,9 +24,7 @@
             result += route
         result.removesuffix("/")
 
     if result == "":
         result = "/"
 
     return result
-
-
```

### Comparing `orwynn-1.0.0rc1/orwynn/utils/url/helpers.py` & `orwynn-1.0.0rc2/orwynn/utils/url/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/url/test_utils.py` & `orwynn-1.0.0rc2/orwynn/utils/url/test_utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/validation/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/validation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing
 from inspect import isclass
 from pathlib import Path
 from typing import Any, Callable, Optional, Sized, TypeVar
 
 from pydantic import ValidationError as _PydanticValidationError
 from pydantic import validator as _pydantic_validator
+from orwynn.utils.types import AnyCoro
 
 from orwynn.utils.validation.validator import Validator
 from orwynn.utils.validation.errors import (ExpectationError,
                                             ReValidationError,
                                             UnknownValidatorError,
                                             ValidationError)
 
@@ -238,15 +239,16 @@
 
 def expect(
     fn: Callable,
     ErrorToExpect: type[Exception],
     *args,
     **kwargs
 ) -> None:
-    """Expects given function to raise given error if function is called with
+    """
+    Expects given function to raise given error if function is called with
     given args and kwargs.
 
     Args:
         fn:
             Function to call.
         ErrorToExpect:
             Exception class to expect.
@@ -265,14 +267,31 @@
         pass
     else:
         raise ExpectationError(
             f"error {ErrorToExpect} expected on call of function {fn}"
         )
 
 
+async def expect_async(
+    coro: AnyCoro,
+    ErrorToExpect: type[Exception]
+) -> None:
+    """
+    Works same as validation.expect, but with async coroutine being tested.
+    """
+    try:
+        await coro
+    except ErrorToExpect:
+        pass
+    else:
+        raise ExpectationError(
+            f"error {ErrorToExpect} expected on call of coro {coro}"
+        )
+
+
 CheckedObj = TypeVar("CheckedObj")
 def check(obj: Optional[CheckedObj]) -> CheckedObj:
     """Checks if given object is not None.
 
     Raises:
         ValidationError:
             If given object is None.
```

### Comparing `orwynn-1.0.0rc1/orwynn/utils/validation/errors.py` & `orwynn-1.0.0rc2/orwynn/utils/validation/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/utils/yml/__init__.py` & `orwynn-1.0.0rc2/orwynn/utils/yml/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/__init__.py` & `orwynn-1.0.0rc2/orwynn/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/constants.py` & `orwynn-1.0.0rc2/orwynn/websocket/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/context/id.py` & `orwynn-1.0.0rc2/orwynn/websocket/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/context/middleware/builtin.py` & `orwynn-1.0.0rc2/orwynn/websocket/context/middleware/builtin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/context/middleware/contextbuiltin.py` & `orwynn-1.0.0rc2/orwynn/websocket/context/middleware/contextbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/context/test_main.py` & `orwynn-1.0.0rc2/orwynn/websocket/context/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.context.errors import UndefinedStorageError
 from orwynn.utils import validation
 from orwynn.websocket.context.id import (
     WebsocketRequestContextId,
 )
 from orwynn.websocket.controller.controller import (
     WebsocketController,
 )
 from orwynn.websocket.log.middleware import LogWebsocketMiddleware
 from orwynn.websocket.websocket import Websocket
 
 
-def test_basic():
+@pytest.mark.asyncio
+async def test_basic():
     """Request id should be fetchable from context within request-response
     cycle and unfetchable outside this cycle.
     """
     class C1(WebsocketController):
         ROUTE = "/"
 
         async def main(self, websocket: Websocket) -> None:
             await websocket.send_json(
                 {"request_id": WebsocketRequestContextId().get()}
             )
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         Module(
             "/",
             Controllers=[C1],
             Middleware=[LogWebsocketMiddleware]
         )
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/controller/controller.py` & `orwynn-1.0.0rc2/orwynn/websocket/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/controller/test_controller.py` & `orwynn-1.0.0rc2/orwynn/websocket/controller/test_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from orwynn.apiversion import ApiVersion
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.di.di import Di
 from orwynn.utils import validation
 from orwynn.websocket import Websocket, WebsocketController
 
@@ -30,53 +32,56 @@
         await ws.send_json({
             "user_id": user_id,
             "message": message,
             "order": order
         })
 
 
-def test_main_route():
+@pytest.mark.asyncio
+async def test_main_route():
     class WS1(WebsocketController):
         ROUTE = "/hello"
 
         async def main(self, ws: Websocket) -> None:
             await ws.send_json({"message": "Hello!"})
             await ws.close()
 
-    client = Boot(Module(
+    client = (await Boot.create(Module(
         route="/",
         Controllers=[WS1]
-    )).app.client
+    ))).app.client
 
     with client.websocket("/hello") as ws:
         data = ws.receive_json()
 
     assert data == {"message": "Hello!"}
 
 
-def test_custom_route():
+@pytest.mark.asyncio
+async def test_custom_route():
     class WS1(WebsocketController):
         ROUTE = "/hello"
 
         async def on_message(self, ws: Websocket) -> None:
             await ws.send_json({"message": "Hello!"})
             await ws.close()
 
-    client = Boot(Module(
+    client = (await Boot.create(Module(
         route="/",
         Controllers=[WS1]
-    )).app.client
+    ))).app.client
 
     with client.websocket("/hello/message") as ws:
         data = ws.receive_json()
 
     assert data == {"message": "Hello!"}
 
 
-def test_several_routes():
+@pytest.mark.asyncio
+async def test_several_routes():
     class WS1(WebsocketController):
         ROUTE = "/hello"
 
         async def main(self, ws: Websocket) -> None:
             await ws.send_json({"message": "main"})
             await ws.close()
 
@@ -84,61 +89,64 @@
             await ws.send_json({"message": "message"})
             await ws.close()
 
         async def on_hello(self, ws: Websocket) -> None:
             await ws.send_json({"message": "hello"})
             await ws.close()
 
-    client = Boot(Module(
+    client = (await Boot.create(Module(
         route="/",
         Controllers=[WS1]
-    )).app.client
+    ))).app.client
 
     with client.websocket("/hello") as ws:
         data = ws.receive_json()
         assert data == {"message": "main"}
 
     with client.websocket("/hello/message") as ws:
         data = ws.receive_json()
         assert data == {"message": "message"}
 
     with client.websocket("/hello/hello") as ws:
         data = ws.receive_json()
         assert data == {"message": "hello"}
 
 
-def test_arguments():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_arguments():
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[ArgumentedCtrl])
     )
 
     with boot.client.websocket("/user/eg1?message=hello&order=2") as ws:
         data: dict = ws.receive_json()
 
         assert data["user_id"] == "eg1"
         assert data["message"] == "hello"
         assert data["order"] == 2
 
 
-def test_default_query():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_default_query():
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[ArgumentedCtrl])
     )
 
     with boot.client.websocket("/user/eg1") as ws:
         data: dict = ws.receive_json()
 
         assert data["user_id"] == "eg1"
         assert data["message"] == "welcome"
         assert data["order"] is None
 
 
 
-def test_final_routes():
-    Boot(
+@pytest.mark.asyncio
+async def test_final_routes():
+    await Boot.create(
         Module(
             "/",
             Controllers=[WsCtrl]
         ),
         api_version=ApiVersion(supported={1, 2, 3}),
         global_websocket_route="/ws/v{version}"
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/controller/test_globalroute.py` & `orwynn-1.0.0rc2/orwynn/websocket/controller/test_globalroute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 import starlette.websockets
 
 from orwynn.apiversion import ApiVersion
 from orwynn.base.module.module import Module
 from orwynn.boot import Boot
 from orwynn.websocket.controller.controller import (
     WebsocketController,
@@ -12,79 +13,83 @@
 class WsCtrl(WebsocketController):
     ROUTE = "/message"
 
     async def main(self, ws: Websocket) -> None:
         await ws.send_json({"message": "hello"})
 
 
-def test_default():
+@pytest.mark.asyncio
+async def test_default():
     """
     By default a client should use the global route.
     """
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/", Controllers=[WsCtrl]),
         global_websocket_route="/donuts"
     )
 
     with boot.app.client.websocket("/message") as ws:
         data: dict = ws.receive_json()
         assert data["message"] == "hello"
 
 
-def test_default_version():
+@pytest.mark.asyncio
+async def test_default_version():
     """
     By default a client should use the latest api version available.
     """
     class _C(WsCtrl):
         VERSION = 3
 
         async def main(self, ws: Websocket) -> None:
             return await super().main(ws)
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/", Controllers=[_C]),
         global_websocket_route="/ws/v{version}",
         api_version=ApiVersion(
             supported={1, 2, 3}
         )
     )
 
     with boot.app.client.websocket("/message") as ws:
         data: dict = ws.receive_json()
         assert data["message"] == "hello"
 
 
-def test_not_used():
+@pytest.mark.asyncio
+async def test_not_used():
     """
     The global route can be disabled.
     """
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/", Controllers=[WsCtrl]),
         global_websocket_route="/donuts"
     )
 
     with boot.app.client.websocket(
         "/donuts/message",
         is_global_route_used=False
     ) as ws:
         data: dict = ws.receive_json()
         assert data["message"] == "hello"
 
 
-def test_pass_version():
+@pytest.mark.asyncio
+async def test_pass_version():
     """
     A client is able to not specify global route, but pass own api version.
     """
     class _C(WsCtrl):
         VERSION = 2
 
         async def main(self, ws: Websocket) -> None:
             return await super().main(ws)
 
-    boot: Boot = Boot(
+    boot: Boot = await Boot.create(
         root_module=Module("/", Controllers=[_C]),
         global_websocket_route="/ws/v{version}",
         api_version=ApiVersion(
             supported={1, 2, 3}
         )
     )
```

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/errorhandler/middleware.py` & `orwynn-1.0.0rc2/orwynn/websocket/errorhandler/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/errorhandler/test_default.py` & `orwynn-1.0.0rc2/orwynn/websocket/errorhandler/test_default.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import pytest
+
 from orwynn.base.errorhandler.errorhandler import ErrorHandler
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
-from orwynn.utils.protocol import Protocol
+from orwynn.utils.scheme import Scheme
 from orwynn.websocket import Websocket, WebsocketController
 
 
 class SomeWebsocketError(Exception):
     pass
 
 
@@ -16,26 +18,27 @@
 
     async def main(self, ws: Websocket) -> None:
         raise SomeWebsocketError("hello")
 
 
 class Eh(ErrorHandler):
     E = SomeWebsocketError
-    PROTOCOL = Protocol.WEBSOCKET
+    PROTOCOL = Scheme.WEBSOCKET
 
     async def handle(
         self, request: Websocket, error: SomeWebsocketError
     ) -> None:
         data: dict = BootProxy.ie().api_indication.digest(error)
         data["value"]["message"] = "handled"
         await request.send_json(data)
 
 
-def test_default():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_default():
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[Wc])
     )
 
     with boot.app.client.websocket("/") as ws:
         data: dict = ws.receive_json()
 
         err = validation.apply(
@@ -44,16 +47,17 @@
                 data
             ),
             SomeWebsocketError
         )
         assert err.args[0] == "hello"
 
 
-def test_one_handler():
-    boot: Boot = Boot(
+@pytest.mark.asyncio
+async def test_one_handler():
+    boot: Boot = await Boot.create(
         Module("/", Controllers=[Wc]),
         ErrorHandlers={Eh}
     )
 
     with boot.app.client.websocket("/") as ws:
         data: dict = ws.receive_json()
```

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/log/logger.py` & `orwynn-1.0.0rc2/orwynn/websocket/log/logger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/log/middleware.py` & `orwynn-1.0.0rc2/orwynn/websocket/log/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/middleware/connectionbuiltin.py` & `orwynn-1.0.0rc2/orwynn/websocket/middleware/connectionbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/middleware/middleware.py` & `orwynn-1.0.0rc2/orwynn/websocket/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/middleware/test_main.py` & `orwynn-1.0.0rc2/orwynn/websocket/middleware/test_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from orwynn.base.module.module import Module
 from orwynn.boot.boot import Boot
 from orwynn.testing.client import Client
 from orwynn.websocket import (
     Websocket,
     WebsocketController,
     WebsocketMiddleware,
@@ -21,16 +23,17 @@
     ROUTE = "/"
 
     async def on_message(self, websocket: Websocket) -> None:
         await websocket.send_json({"value": "hello"})
         await websocket.close()
 
 
-def test_basic():
-    boot: Boot = Boot(Module(
+@pytest.mark.asyncio
+async def test_basic():
+    boot: Boot = await Boot.create(Module(
         route="/hello",
         Controllers=[Ws1],
         Middleware=[Mw1]
     ))
     client: Client = boot.app.client
 
     with client.websocket("/hello/message") as ws:
```

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/routing/helpers.py` & `orwynn-1.0.0rc2/orwynn/websocket/routing/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/routing/nextcall.py` & `orwynn-1.0.0rc2/orwynn/websocket/routing/nextcall.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/orwynn/websocket/routing/stack.py` & `orwynn-1.0.0rc2/orwynn/websocket/routing/stack.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0rc1/pyproject.toml` & `orwynn-1.0.0rc2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orwynn"
-version = "1.0.0rc1"
+version = "1.0.0rc2"
 description = "Scalable web-framework with out-of-the-box architecture"
 authors = ["ryzhovalex <thed4rkof@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.88.0"
```

### Comparing `orwynn-1.0.0rc1/PKG-INFO` & `orwynn-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orwynn
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Scalable web-framework with out-of-the-box architecture
 Author: ryzhovalex
 Author-email: thed4rkof@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

