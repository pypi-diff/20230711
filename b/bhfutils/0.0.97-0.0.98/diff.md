# Comparing `tmp/bhfutils-0.0.97.tar.gz` & `tmp/bhfutils-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhfutils-0.0.97.tar", last modified: Sun Apr  2 07:36:29 2023, max compression
+gzip compressed data, was "bhfutils-0.0.98.tar", last modified: Tue Jul 11 14:02:34 2023, max compression
```

## Comparing `bhfutils-0.0.97.tar` & `bhfutils-0.0.98.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.699142 bhfutils-0.0.97/
--rw-r--r--   0 16707506 (850592629) 646495703       19 2023-02-05 14:53:08.000000 bhfutils-0.0.97/MANIFEST.in
--rw-r--r--   0 16707506 (850592629) 646495703     2221 2023-04-02 07:36:29.698735 bhfutils-0.0.97/PKG-INFO
--rw-r--r--   0 16707506 (850592629) 646495703     1835 2023-01-21 10:38:32.000000 bhfutils-0.0.97/README.rst
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.638301 bhfutils-0.0.97/bhfutils/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/__init__.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.648769 bhfutils-0.0.97/bhfutils/crawler/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703       53 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/bhf_signals.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.649498 bhfutils-0.0.97/bhfutils/crawler/config/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/config/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703     1805 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/config/file_pusher.py
--rwxr-xr-x   0 16707506 (850592629) 646495703      774 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/custom_cookies.py
--rw-r--r--   0 16707506 (850592629) 646495703    25391 2023-01-21 10:44:56.000000 bhfutils-0.0.97/bhfutils/crawler/distributed_scheduler.py
--rw-r--r--   0 16707506 (850592629) 646495703      788 2023-03-19 16:23:31.000000 bhfutils-0.0.97/bhfutils/crawler/items.py
--rw-r--r--   0 16707506 (850592629) 646495703     6788 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/log_retry_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     2137 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/meta_passthrough_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     8076 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/pipelines.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.651646 bhfutils-0.0.97/bhfutils/crawler/playwright/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/__init__.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.652395 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/
--rw-r--r--   0 16707506 (850592629) 646495703      163 2023-03-04 19:56:56.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/__init__.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.655043 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_async/
--rw-r--r--   0 16707506 (850592629) 646495703      162 2023-03-05 09:05:37.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_async/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703      215 2023-03-05 05:25:21.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_async/_mouse_helper.py
--rw-r--r--   0 16707506 (850592629) 646495703     6150 2023-03-05 10:59:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_async/_spoof.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.657106 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_sync/
--rw-r--r--   0 16707506 (850592629) 646495703      134 2023-03-05 07:34:51.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_sync/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703      196 2023-03-05 05:25:21.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_sync/_mouse_helper.py
--rw-r--r--   0 16707506 (850592629) 646495703     5882 2023-03-04 19:56:56.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_sync/_spoof.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.657787 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/js/
--rw-r--r--   0 16707506 (850592629) 646495703     2665 2023-03-04 19:19:33.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/js/mouseHelper.js
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.659750 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/shared/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-03-04 19:21:38.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/shared/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703     2670 2023-03-05 07:10:12.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/shared/math.py
--rw-r--r--   0 16707506 (850592629) 646495703     2141 2023-03-05 09:40:34.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/shared/spoof.py
--rw-r--r--   0 16707506 (850592629) 646495703    17941 2023-04-02 07:36:19.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/handler.py
--rw-r--r--   0 16707506 (850592629) 646495703     1502 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/headers.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.674495 bhfutils-0.0.97/bhfutils/crawler/playwright/js/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/__init__.py
--rwxr-xr-x   0 16707506 (850592629) 646495703     2021 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.app.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      990 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.csi.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     4448 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.loadtimes.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     9629 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.runtime.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      470 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/hairline.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     3328 2023-03-05 18:13:06.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/iframe.contentWindow.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     5962 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/magic-arrays.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     1688 2023-03-05 18:15:49.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/media.codecs.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      171 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.deviceMemory.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      258 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.hardwareConcurrency.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      268 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.languages.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      543 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.permissions.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      158 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.platform.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     3291 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.plugins.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      206 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.userAgent.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      152 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.vendor.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      293 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.webdriver.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     1271 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/screen.touch.js
--rwxr-xr-x   0 16707506 (850592629) 646495703      146 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/user-agent-override.js
--rwxr-xr-x   0 16707506 (850592629) 646495703    19464 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/utils.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     1053 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/webgl.vendor.js
--rwxr-xr-x   0 16707506 (850592629) 646495703     1024 2023-02-05 14:53:08.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/js/window.dimensions.js
--rw-r--r--   0 16707506 (850592629) 646495703     1518 2023-03-05 08:49:03.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/page.py
--rw-r--r--   0 16707506 (850592629) 646495703     6068 2023-03-08 08:19:27.000000 bhfutils-0.0.97/bhfutils/crawler/playwright/stealth.py
--rw-r--r--   0 16707506 (850592629) 646495703     2396 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/redis_domain_max_page_filter.py
--rw-r--r--   0 16707506 (850592629) 646495703     1084 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/redis_dupefilter.py
--rw-r--r--   0 16707506 (850592629) 646495703     2903 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/redis_global_page_per_domain_filter.py
--rw-r--r--   0 16707506 (850592629) 646495703      931 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/redis_retry_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     6273 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/redis_stats_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     5645 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/settings_template.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.675292 bhfutils-0.0.97/bhfutils/crawler/spiders/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/spiders/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703     1952 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/spiders/redis_spider.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.681855 bhfutils-0.0.97/bhfutils/crawler/tests/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703     5288 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/online.py
--rw-r--r--   0 16707506 (850592629) 646495703    19519 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_distributed_scheduler.py
--rw-r--r--   0 16707506 (850592629) 646495703     2858 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_link_spider.py
--rw-r--r--   0 16707506 (850592629) 646495703     1907 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_log_retry_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     1743 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_meta_passthrough_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     7835 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_pipelines.py
--rw-r--r--   0 16707506 (850592629) 646495703      729 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_dupefilter.py
--rw-r--r--   0 16707506 (850592629) 646495703     1647 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_page_limit_filters.py
--rw-r--r--   0 16707506 (850592629) 646495703      772 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_retry_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     5200 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_stats_middleware.py
--rw-r--r--   0 16707506 (850592629) 646495703     2062 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/crawler/tests/test_wandering_spider.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.686163 bhfutils-0.0.97/bhfutils/examples/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703     1850 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_ah.py
--rw-r--r--   0 16707506 (850592629) 646495703     1769 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_lf.py
--rw-r--r--   0 16707506 (850592629) 646495703      538 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_mt.py
--rw-r--r--   0 16707506 (850592629) 646495703     1877 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_rq.py
--rw-r--r--   0 16707506 (850592629) 646495703     2895 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_rtq.py
--rw-r--r--   0 16707506 (850592629) 646495703     2411 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_sc.py
--rw-r--r--   0 16707506 (850592629) 646495703     1149 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_sw.py
--rw-r--r--   0 16707506 (850592629) 646495703     2806 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/examples/example_zw.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.691171 bhfutils-0.0.97/bhfutils/scutils/
--rw-r--r--   0 16707506 (850592629) 646495703      302 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703     1012 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/argparse_helper.py
--rw-r--r--   0 16707506 (850592629) 646495703    11413 2023-02-01 12:42:01.000000 bhfutils-0.0.97/bhfutils/scutils/log_factory.py
--rw-r--r--   0 16707506 (850592629) 646495703     1782 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/method_timer.py
--rw-r--r--   0 16707506 (850592629) 646495703     4335 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/redis_queue.py
--rw-r--r--   0 16707506 (850592629) 646495703     8131 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/redis_throttled_queue.py
--rw-r--r--   0 16707506 (850592629) 646495703     3570 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/settings_wrapper.py
--rw-r--r--   0 16707506 (850592629) 646495703    21536 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/stats_collector.py
--rw-r--r--   0 16707506 (850592629) 646495703    14093 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/scutils/zookeeper_watcher.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.698081 bhfutils-0.0.97/bhfutils/tests/
--rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/__init__.py
--rw-r--r--   0 16707506 (850592629) 646495703       55 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/default_settings.py
--rw-r--r--   0 16707506 (850592629) 646495703    16092 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/online.py
--rw-r--r--   0 16707506 (850592629) 646495703      154 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/override_defaults.py
--rw-r--r--   0 16707506 (850592629) 646495703     2448 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_argparse_helper.py
--rw-r--r--   0 16707506 (850592629) 646495703    11075 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_log_factory.py
--rw-r--r--   0 16707506 (850592629) 646495703      918 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_method_timer.py
--rw-r--r--   0 16707506 (850592629) 646495703     3457 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_redis_queue.py
--rw-r--r--   0 16707506 (850592629) 646495703     2672 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_redis_throttled_queue.py
--rw-r--r--   0 16707506 (850592629) 646495703     2118 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_settings_wrapper.py
--rw-r--r--   0 16707506 (850592629) 646495703     2493 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_stats_collector.py
--rw-r--r--   0 16707506 (850592629) 646495703     3072 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/test_zookeeper_watcher.py
--rw-r--r--   0 16707506 (850592629) 646495703     2642 2023-01-21 10:38:32.000000 bhfutils-0.0.97/bhfutils/tests/throttled_queue.py
-drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-04-02 07:36:29.640228 bhfutils-0.0.97/bhfutils.egg-info/
--rw-r--r--   0 16707506 (850592629) 646495703     2221 2023-04-02 07:36:29.000000 bhfutils-0.0.97/bhfutils.egg-info/PKG-INFO
--rw-r--r--   0 16707506 (850592629) 646495703     4532 2023-04-02 07:36:29.000000 bhfutils-0.0.97/bhfutils.egg-info/SOURCES.txt
--rw-r--r--   0 16707506 (850592629) 646495703        1 2023-04-02 07:36:29.000000 bhfutils-0.0.97/bhfutils.egg-info/dependency_links.txt
--rw-r--r--   0 16707506 (850592629) 646495703      415 2023-04-02 07:36:29.000000 bhfutils-0.0.97/bhfutils.egg-info/requires.txt
--rw-r--r--   0 16707506 (850592629) 646495703        9 2023-04-02 07:36:29.000000 bhfutils-0.0.97/bhfutils.egg-info/top_level.txt
--rw-r--r--   0 16707506 (850592629) 646495703        1 2023-03-08 08:30:24.000000 bhfutils-0.0.97/bhfutils.egg-info/zip-safe
--rw-r--r--   0 16707506 (850592629) 646495703       38 2023-04-02 07:36:29.699239 bhfutils-0.0.97/setup.cfg
--rw-r--r--   0 16707506 (850592629) 646495703     1440 2023-04-02 07:36:19.000000 bhfutils-0.0.97/setup.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.847216 bhfutils-0.0.98/
+-rw-r--r--   0 16707506 (850592629) 646495703       19 2023-02-05 14:53:08.000000 bhfutils-0.0.98/MANIFEST.in
+-rw-r--r--   0 16707506 (850592629) 646495703     2221 2023-07-11 14:02:34.846721 bhfutils-0.0.98/PKG-INFO
+-rw-r--r--   0 16707506 (850592629) 646495703     1835 2023-01-21 10:38:32.000000 bhfutils-0.0.98/README.rst
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.703993 bhfutils-0.0.98/bhfutils/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/__init__.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.723416 bhfutils-0.0.98/bhfutils/crawler/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703       53 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/bhf_signals.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.725912 bhfutils-0.0.98/bhfutils/crawler/config/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/config/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1805 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/config/file_pusher.py
+-rwxr-xr-x   0 16707506 (850592629) 646495703      774 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/custom_cookies.py
+-rw-r--r--   0 16707506 (850592629) 646495703    25391 2023-01-21 10:44:56.000000 bhfutils-0.0.98/bhfutils/crawler/distributed_scheduler.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1367 2023-07-11 14:00:38.000000 bhfutils-0.0.98/bhfutils/crawler/items.py
+-rw-r--r--   0 16707506 (850592629) 646495703     6788 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/log_retry_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2137 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/meta_passthrough_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     8076 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/pipelines.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.733671 bhfutils-0.0.98/bhfutils/crawler/playwright/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/__init__.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.734672 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/
+-rw-r--r--   0 16707506 (850592629) 646495703      163 2023-03-04 19:56:56.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/__init__.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.739536 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_async/
+-rw-r--r--   0 16707506 (850592629) 646495703      162 2023-03-05 09:05:37.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_async/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703      215 2023-03-05 05:25:21.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_async/_mouse_helper.py
+-rw-r--r--   0 16707506 (850592629) 646495703     6150 2023-03-05 10:59:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_async/_spoof.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.746072 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_sync/
+-rw-r--r--   0 16707506 (850592629) 646495703      134 2023-03-05 07:34:51.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_sync/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703      196 2023-03-05 05:25:21.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_sync/_mouse_helper.py
+-rw-r--r--   0 16707506 (850592629) 646495703     5882 2023-03-04 19:56:56.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_sync/_spoof.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.747768 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/js/
+-rw-r--r--   0 16707506 (850592629) 646495703     2665 2023-03-04 19:19:33.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/js/mouseHelper.js
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.753806 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/shared/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-03-04 19:21:38.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/shared/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2670 2023-03-05 07:10:12.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/shared/math.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2141 2023-03-05 09:40:34.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/shared/spoof.py
+-rw-r--r--   0 16707506 (850592629) 646495703    17938 2023-04-02 13:02:10.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/handler.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1502 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/headers.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.797344 bhfutils-0.0.98/bhfutils/crawler/playwright/js/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/__init__.py
+-rwxr-xr-x   0 16707506 (850592629) 646495703     2021 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.app.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      990 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.csi.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     4448 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.loadtimes.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     9629 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.runtime.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      470 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/hairline.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     3328 2023-03-05 18:13:06.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/iframe.contentWindow.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     5962 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/magic-arrays.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     1688 2023-03-05 18:15:49.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/media.codecs.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      171 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.deviceMemory.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      258 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.hardwareConcurrency.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      268 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.languages.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      543 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.permissions.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      158 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.platform.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     3291 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.plugins.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      206 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.userAgent.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      152 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.vendor.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      293 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.webdriver.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     1271 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/screen.touch.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703      146 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/user-agent-override.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703    19464 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/utils.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     1053 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/webgl.vendor.js
+-rwxr-xr-x   0 16707506 (850592629) 646495703     1024 2023-02-05 14:53:08.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/js/window.dimensions.js
+-rw-r--r--   0 16707506 (850592629) 646495703     1518 2023-03-05 08:49:03.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/page.py
+-rw-r--r--   0 16707506 (850592629) 646495703     6068 2023-03-08 08:19:27.000000 bhfutils-0.0.98/bhfutils/crawler/playwright/stealth.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2396 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/redis_domain_max_page_filter.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1084 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/redis_dupefilter.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2903 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/redis_global_page_per_domain_filter.py
+-rw-r--r--   0 16707506 (850592629) 646495703      931 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/redis_retry_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     6273 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/redis_stats_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     5645 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/settings_template.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.799757 bhfutils-0.0.98/bhfutils/crawler/spiders/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/spiders/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1952 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/spiders/redis_spider.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.816717 bhfutils-0.0.98/bhfutils/crawler/tests/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703     5288 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/online.py
+-rw-r--r--   0 16707506 (850592629) 646495703    19519 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_distributed_scheduler.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2858 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_link_spider.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1907 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_log_retry_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1743 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_meta_passthrough_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     7835 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_pipelines.py
+-rw-r--r--   0 16707506 (850592629) 646495703      729 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_dupefilter.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1647 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_page_limit_filters.py
+-rw-r--r--   0 16707506 (850592629) 646495703      772 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_retry_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     5200 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_stats_middleware.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2062 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/crawler/tests/test_wandering_spider.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.823035 bhfutils-0.0.98/bhfutils/examples/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1850 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_ah.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1769 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_lf.py
+-rw-r--r--   0 16707506 (850592629) 646495703      538 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_mt.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1877 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_rq.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2895 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_rtq.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2411 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_sc.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1149 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_sw.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2806 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/examples/example_zw.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.832868 bhfutils-0.0.98/bhfutils/scutils/
+-rw-r--r--   0 16707506 (850592629) 646495703      302 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1012 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/argparse_helper.py
+-rw-r--r--   0 16707506 (850592629) 646495703    11413 2023-02-01 12:42:01.000000 bhfutils-0.0.98/bhfutils/scutils/log_factory.py
+-rw-r--r--   0 16707506 (850592629) 646495703     1782 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/method_timer.py
+-rw-r--r--   0 16707506 (850592629) 646495703     4335 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/redis_queue.py
+-rw-r--r--   0 16707506 (850592629) 646495703     8131 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/redis_throttled_queue.py
+-rw-r--r--   0 16707506 (850592629) 646495703     3570 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/settings_wrapper.py
+-rw-r--r--   0 16707506 (850592629) 646495703    21536 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/stats_collector.py
+-rw-r--r--   0 16707506 (850592629) 646495703    14093 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/scutils/zookeeper_watcher.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.845997 bhfutils-0.0.98/bhfutils/tests/
+-rw-r--r--   0 16707506 (850592629) 646495703        0 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/__init__.py
+-rw-r--r--   0 16707506 (850592629) 646495703       55 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/default_settings.py
+-rw-r--r--   0 16707506 (850592629) 646495703    16092 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/online.py
+-rw-r--r--   0 16707506 (850592629) 646495703      154 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/override_defaults.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2448 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_argparse_helper.py
+-rw-r--r--   0 16707506 (850592629) 646495703    11075 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_log_factory.py
+-rw-r--r--   0 16707506 (850592629) 646495703      918 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_method_timer.py
+-rw-r--r--   0 16707506 (850592629) 646495703     3457 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_redis_queue.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2672 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_redis_throttled_queue.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2118 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_settings_wrapper.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2493 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_stats_collector.py
+-rw-r--r--   0 16707506 (850592629) 646495703     3072 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/test_zookeeper_watcher.py
+-rw-r--r--   0 16707506 (850592629) 646495703     2642 2023-01-21 10:38:32.000000 bhfutils-0.0.98/bhfutils/tests/throttled_queue.py
+drwxr-xr-x   0 16707506 (850592629) 646495703        0 2023-07-11 14:02:34.707204 bhfutils-0.0.98/bhfutils.egg-info/
+-rw-r--r--   0 16707506 (850592629) 646495703     2221 2023-07-11 14:02:34.000000 bhfutils-0.0.98/bhfutils.egg-info/PKG-INFO
+-rw-r--r--   0 16707506 (850592629) 646495703     4532 2023-07-11 14:02:34.000000 bhfutils-0.0.98/bhfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 16707506 (850592629) 646495703        1 2023-07-11 14:02:34.000000 bhfutils-0.0.98/bhfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 16707506 (850592629) 646495703      415 2023-07-11 14:02:34.000000 bhfutils-0.0.98/bhfutils.egg-info/requires.txt
+-rw-r--r--   0 16707506 (850592629) 646495703        9 2023-07-11 14:02:34.000000 bhfutils-0.0.98/bhfutils.egg-info/top_level.txt
+-rw-r--r--   0 16707506 (850592629) 646495703        1 2023-03-08 08:30:24.000000 bhfutils-0.0.98/bhfutils.egg-info/zip-safe
+-rw-r--r--   0 16707506 (850592629) 646495703       38 2023-07-11 14:02:34.847319 bhfutils-0.0.98/setup.cfg
+-rw-r--r--   0 16707506 (850592629) 646495703     1440 2023-07-11 14:00:38.000000 bhfutils-0.0.98/setup.py
```

### Comparing `bhfutils-0.0.97/PKG-INFO` & `bhfutils-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhfutils
-Version: 0.0.97
+Version: 0.0.98
 Summary: Utilities that are used by any spider of Behoof project
 Home-page: https://behoof.app/
 Author: Teplygin Vladimir
 Author-email: vvteplygin@gmail.com
 License: MIT
 Keywords: behoof,scrapy-cluster,utilities
 Description-Content-Type: text/x-rst
```

### Comparing `bhfutils-0.0.97/README.rst` & `bhfutils-0.0.98/README.rst`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/config/file_pusher.py` & `bhfutils-0.0.98/bhfutils/crawler/config/file_pusher.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/custom_cookies.py` & `bhfutils-0.0.98/bhfutils/crawler/custom_cookies.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/distributed_scheduler.py` & `bhfutils-0.0.98/bhfutils/crawler/distributed_scheduler.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/items.py` & `bhfutils-0.0.98/bhfutils/crawler/items.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,30 +10,56 @@
     crawlid = Field()
     url = Field()
     responseUrl = Field()
     statusCode = Field()
     success = Field()
     exception = Field()
     encoding = Field()
-    playgroundId = Field()
     attrs = Field()
 
 
 class MenuResponseItem(RawResponseItem):
+    playgroundId = Field()
     groupCategoryName = Field()
     groupName = Field()
     groupUrl = Field()
 
 
 class ProductResponseItem(RawResponseItem):
+    playgroundId = Field()
     productUrl = Field()
     groupId = Field()
     price = Field()
 
 
 class ProductDetailsResponseItem(RawResponseItem):
+    playgroundId = Field()
     productUrl = Field()
     groupId = Field()
     imageUrl = Field()
     name = Field()
     description = Field()
     details = Field()
+
+
+class ReviewResponseItem(RawResponseItem):
+    technoBlogId = Field()
+    reviewUrl = Field()
+    name = Field()
+    imageUrl = Field()
+
+
+class ReviewDetailsResponseItem(RawResponseItem):
+    technoBlogId = Field()
+    reviewUrl = Field()
+    createDate = Field()
+    author = Field()
+    name = Field()
+    description = Field()
+    pros = Field()
+    cons = Field()
+    productName = Field()
+    productParameters = Field()
+    verdict = Field()
+    baseParameters = Field()
+    keywords = Field()
+    category = Field()
```

### Comparing `bhfutils-0.0.97/bhfutils/crawler/log_retry_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/log_retry_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/meta_passthrough_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/meta_passthrough_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/pipelines.py` & `bhfutils-0.0.98/bhfutils/crawler/pipelines.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_async/_spoof.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_async/_spoof.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/do_sync/_spoof.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/do_sync/_spoof.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/js/mouseHelper.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/js/mouseHelper.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/shared/math.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/shared/math.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/cursor/shared/spoof.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/cursor/shared/spoof.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/handler.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         self.playwright = await self.playwright_context_manager.start()
         logger.info("Launching browser")
         browser_launcher = getattr(self.playwright, self.browser_type).launch
         self.browser = await browser_launcher(**self.launch_options)
         logger.info(f"Browser {self.browser_type} launched")
 
     async def _plan_context_rotation(self) -> None:
-        logger.warning("Re create browser: Before acquire")
+        logger.info("Re create browser: Before acquire")
         await self.context_semaphore.acquire()
         logger.info("Re create browser: After acquire")
 
         await self._close()
         await self._launch_browser()
         self.context_rotation_idx = self.context_rotation_idx + 1
         if self.context_rotation_idx >= len(self.dynamic_contexts_kwargs):
```

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/headers.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/headers.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.app.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.app.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.csi.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.csi.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.loadtimes.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.loadtimes.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/chrome.runtime.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/iframe.contentWindow.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/iframe.contentWindow.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/magic-arrays.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/magic-arrays.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/media.codecs.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/media.codecs.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.permissions.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/navigator.plugins.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/navigator.plugins.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/screen.touch.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/screen.touch.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/utils.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/utils.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/webgl.vendor.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/webgl.vendor.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/js/window.dimensions.js` & `bhfutils-0.0.98/bhfutils/crawler/playwright/js/window.dimensions.js`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/page.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/page.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/playwright/stealth.py` & `bhfutils-0.0.98/bhfutils/crawler/playwright/stealth.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/redis_domain_max_page_filter.py` & `bhfutils-0.0.98/bhfutils/crawler/redis_domain_max_page_filter.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/redis_dupefilter.py` & `bhfutils-0.0.98/bhfutils/crawler/redis_dupefilter.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/redis_global_page_per_domain_filter.py` & `bhfutils-0.0.98/bhfutils/crawler/redis_global_page_per_domain_filter.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/redis_retry_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/redis_retry_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/redis_stats_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/redis_stats_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/settings_template.py` & `bhfutils-0.0.98/bhfutils/crawler/settings_template.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/spiders/redis_spider.py` & `bhfutils-0.0.98/bhfutils/crawler/spiders/redis_spider.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/online.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/online.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_distributed_scheduler.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_distributed_scheduler.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_link_spider.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_link_spider.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_log_retry_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_log_retry_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_meta_passthrough_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_meta_passthrough_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_pipelines.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_dupefilter.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_dupefilter.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_page_limit_filters.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_page_limit_filters.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_retry_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_retry_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_redis_stats_middleware.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_redis_stats_middleware.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/crawler/tests/test_wandering_spider.py` & `bhfutils-0.0.98/bhfutils/crawler/tests/test_wandering_spider.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_ah.py` & `bhfutils-0.0.98/bhfutils/examples/example_ah.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_lf.py` & `bhfutils-0.0.98/bhfutils/examples/example_lf.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_mt.py` & `bhfutils-0.0.98/bhfutils/examples/example_mt.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_rq.py` & `bhfutils-0.0.98/bhfutils/examples/example_rq.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_rtq.py` & `bhfutils-0.0.98/bhfutils/examples/example_rtq.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_sc.py` & `bhfutils-0.0.98/bhfutils/examples/example_sc.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_sw.py` & `bhfutils-0.0.98/bhfutils/examples/example_sw.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/examples/example_zw.py` & `bhfutils-0.0.98/bhfutils/examples/example_zw.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/argparse_helper.py` & `bhfutils-0.0.98/bhfutils/scutils/argparse_helper.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/log_factory.py` & `bhfutils-0.0.98/bhfutils/scutils/log_factory.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/method_timer.py` & `bhfutils-0.0.98/bhfutils/scutils/method_timer.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/redis_queue.py` & `bhfutils-0.0.98/bhfutils/scutils/redis_queue.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/redis_throttled_queue.py` & `bhfutils-0.0.98/bhfutils/scutils/redis_throttled_queue.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/settings_wrapper.py` & `bhfutils-0.0.98/bhfutils/scutils/settings_wrapper.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/stats_collector.py` & `bhfutils-0.0.98/bhfutils/scutils/stats_collector.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/scutils/zookeeper_watcher.py` & `bhfutils-0.0.98/bhfutils/scutils/zookeeper_watcher.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/online.py` & `bhfutils-0.0.98/bhfutils/tests/online.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_argparse_helper.py` & `bhfutils-0.0.98/bhfutils/tests/test_argparse_helper.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_log_factory.py` & `bhfutils-0.0.98/bhfutils/tests/test_log_factory.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_method_timer.py` & `bhfutils-0.0.98/bhfutils/tests/test_method_timer.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_redis_queue.py` & `bhfutils-0.0.98/bhfutils/tests/test_redis_queue.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_redis_throttled_queue.py` & `bhfutils-0.0.98/bhfutils/tests/test_redis_throttled_queue.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_settings_wrapper.py` & `bhfutils-0.0.98/bhfutils/tests/test_settings_wrapper.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_stats_collector.py` & `bhfutils-0.0.98/bhfutils/tests/test_stats_collector.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/test_zookeeper_watcher.py` & `bhfutils-0.0.98/bhfutils/tests/test_zookeeper_watcher.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils/tests/throttled_queue.py` & `bhfutils-0.0.98/bhfutils/tests/throttled_queue.py`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/bhfutils.egg-info/PKG-INFO` & `bhfutils-0.0.98/bhfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhfutils
-Version: 0.0.97
+Version: 0.0.98
 Summary: Utilities that are used by any spider of Behoof project
 Home-page: https://behoof.app/
 Author: Teplygin Vladimir
 Author-email: vvteplygin@gmail.com
 License: MIT
 Keywords: behoof,scrapy-cluster,utilities
 Description-Content-Type: text/x-rst
```

### Comparing `bhfutils-0.0.97/bhfutils.egg-info/SOURCES.txt` & `bhfutils-0.0.98/bhfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bhfutils-0.0.97/setup.py` & `bhfutils-0.0.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 }
 
 if 'nosetests' in sys.argv[1:]:
     setup_requires.append('nose')
 
 setup(
     name='bhfutils',
-    version='0.0.97',
+    version='0.0.98',
     description='Utilities that are used by any spider of Behoof project',
     long_description=readme(),
     long_description_content_type='text/x-rst',
     author='Teplygin Vladimir',
     author_email='vvteplygin@gmail.com',
     license='MIT',
     url='https://behoof.app/',
```

