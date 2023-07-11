# Comparing `tmp/neon-skill-weather-1.0.0.tar.gz` & `tmp/neon-skill-weather-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-weather-1.0.0.tar", last modified: Thu Jun 29 02:22:38 2023, max compression
+gzip compressed data, was "neon-skill-weather-1.0.1a1.tar", last modified: Mon Jul 10 23:59:38 2023, max compression
```

## Comparing `neon-skill-weather-1.0.0.tar` & `neon-skill-weather-1.0.1a1.tar`

### file list

```diff
@@ -1,1550 +1,1550 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.566186 neon-skill-weather-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-29 02:22:38.566186 neon-skill-weather-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    50316 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.442186 neon-skill-weather-1.0.0/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.454186 neon-skill-weather-1.0.0/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.454186 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.454186 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.458186 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ca-es/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.446186 neon-skill-weather-1.0.0/locale/da-dk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/da-dk/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.462186 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.466186 neon-skill-weather-1.0.0/locale/da-dk/regex/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/da-dk/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.446186 neon-skill-weather-1.0.0/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.470186 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.474186 neon-skill-weather-1.0.0/locale/de-de/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/weekly/weekly-condition.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.478186 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.482186 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.482186 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.482186 neon-skill-weather-1.0.0/locale/de-de/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.482186 neon-skill-weather-1.0.0/locale/de-de/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/de-de/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.446186 neon-skill-weather-1.0.0/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.482186 neon-skill-weather-1.0.0/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.482186 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/clear-sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/clouds.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.486186 neon-skill-weather-1.0.0/locale/en-us/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/current-wind-strong-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/current/currrent-clouds-alternative-local.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.486186 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.486186 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/error/no-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/error/seven-days-available.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/weekly/weekly-condition.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.490186 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/few.voc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/number-days.voc
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/like.voc
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/location.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/outside.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/en-us/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/en-us/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/en-us/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.446186 neon-skill-weather-1.0.0/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/current/current-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/daily/daily-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.494186 neon-skill-weather-1.0.0/locale/es-es/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.498186 neon-skill-weather-1.0.0/locale/es-es/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/sunset.voc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/es-es/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.446186 neon-skill-weather-1.0.0/locale/eu-eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.498186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.498186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/clear-sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/clouds.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.498186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/current-wind-strong-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/current/currrent-clouds-alternative-local.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.502186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.502186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.502186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/error/no-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/error/seven-days-available.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.502186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.502186 neon-skill-weather-1.0.0/locale/eu-eu/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.502186 neon-skill-weather-1.0.0/locale/eu-eu/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/few.voc
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/number-days.voc
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.506186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/current/current-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/daily/daily-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/sunset.voc
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/fr-fr/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.510186 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/percentage-number.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.514186 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.514186 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.514186 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.514186 neon-skill-weather-1.0.0/locale/gl-es/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-condition-expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/gl-es/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.518186 neon-skill-weather-1.0.0/locale/it-it/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.522186 neon-skill-weather-1.0.0/locale/it-it/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.522186 neon-skill-weather-1.0.0/locale/it-it/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.522186 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.522186 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.522186 neon-skill-weather-1.0.0/locale/it-it/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/it-it/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/it-it/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/current/current-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.526186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/daily/daily-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/direction/southwest.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/sunset.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/nl-nl/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.530186 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-temperature-high.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.534186 neon-skill-weather-1.0.0/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/pt-br/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.450186 neon-skill-weather-1.0.0/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.538186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/clear-sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/clouds.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.542186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-wind-strong-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/error/no-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/error/seven-days-available.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/weekly/weekly-condition.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.546186 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/few.voc
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/number-days.voc
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/like.voc
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/location.voc
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/outside.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.454186 neon-skill-weather-1.0.0/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.550186 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.554186 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.554186 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.554186 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.554186 neon-skill-weather-1.0.0/locale/sv-se/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.554186 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/fog.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/locale/sv-se/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.558186 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-29 02:22:38.000000 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    67906 2023-06-29 02:22:38.000000 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 02:22:38.000000 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 02:22:38.000000 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 02:22:38.000000 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 02:22:38.000000 neon-skill-weather-1.0.0/neon_skill_weather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:22:38.566186 neon-skill-weather-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.562186 neon-skill-weather-1.0.0/skill/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.562186 neon-skill-weather-1.0.0/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/DailyColumn.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/DailyColumnScalable.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/DailyDelegateScalable.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/HourlyColumn.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/WeatherDate.qml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/WeatherDelegateMarkII.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/WeatherDelegateScalable.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/WeatherImage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/WeatherLabel.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/WeatherLocation.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.562186 neon-skill-weather-1.0.0/ui/animations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4829 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/clouds.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5635 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/fog.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     8559 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/partial_clouds.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    64205 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/rain.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    30103 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/sleet.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    46868 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/snow.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/storm.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/animations/sun.json
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/current_1_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/current_1_scalable.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/current_2_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/current_2_scalable.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/daily_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/daily_scalable.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/hourly_mark_ii.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:22:38.562186 neon-skill-weather-1.0.0/ui/images/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/clouds.svg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/fog.svg
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/high_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/humidity.svg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/low_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/moon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/partial_clouds_day.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/partial_clouds_night.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/rain.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/snow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/storm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/sun.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/sunrise.svg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/sunset.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/images/wind.svg
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/single_day_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/ui/sunrise_sunset_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 02:22:34.000000 neon-skill-weather-1.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.733481 neon-skill-weather-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 23:59:38.733481 neon-skill-weather-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.613478 neon-skill-weather-1.0.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.593478 neon-skill-weather-1.0.1a1/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.617478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.617478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.617478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.617478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.621478 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.625479 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.625479 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.625479 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.625479 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ca-es/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.597478 neon-skill-weather-1.0.1a1/locale/da-dk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.625479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.625479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.629479 neon-skill-weather-1.0.1a1/locale/da-dk/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/da-dk/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.601478 neon-skill-weather-1.0.1a1/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.633479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.637479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.637479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/weekly/weekly-condition.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.641479 neon-skill-weather-1.0.1a1/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/de-de/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.605478 neon-skill-weather-1.0.1a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.645479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/clear-sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/clouds.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.649479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/current/currrent-clouds-alternative-local.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/error/no-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/error/seven-days-available.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/weekly/weekly-condition.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.653479 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/few.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/number-days.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/like.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/location.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/outside.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/en-us/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.605478 neon-skill-weather-1.0.1a1/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/current/current-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.657479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/daily/daily-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/sunset.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/es-es/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.605478 neon-skill-weather-1.0.1a1/locale/eu-eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.661479 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/clear-sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/clouds.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.665480 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/current/currrent-clouds-alternative-local.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.665480 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/error/no-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/error/seven-days-available.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.669479 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/few.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/number-days.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.605478 neon-skill-weather-1.0.1a1/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/current/current-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/daily/daily-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.673480 neon-skill-weather-1.0.1a1/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/sunset.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/fr-fr/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.609478 neon-skill-weather-1.0.1a1/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/percentage-number.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.677480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.681480 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/gl-es/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.609478 neon-skill-weather-1.0.1a1/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.685480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.689480 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/it-it/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.609478 neon-skill-weather-1.0.1a1/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/current/current-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/daily/daily-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/direction/southwest.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.693480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/sunset.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/nl-nl/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.609478 neon-skill-weather-1.0.1a1/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.697480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-temperature-high.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.701480 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/pt-br/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.613478 neon-skill-weather-1.0.1a1/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.705480 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/clear-sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/clouds.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.709480 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/error/no-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/error/seven-days-available.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/weekly/weekly-condition.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.713481 neon-skill-weather-1.0.1a1/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/few.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/number-days.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/like.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/location.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/outside.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.613478 neon-skill-weather-1.0.1a1/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.717481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.721481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.721481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.721481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.721481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.725481 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.729481 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.729481 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/locale/sv-se/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.729481 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 23:59:38.000000 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    67906 2023-07-10 23:59:38.000000 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:59:38.000000 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 23:59:38.000000 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 23:59:38.000000 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 23:59:38.000000 neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:59:38.733481 neon-skill-weather-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.729481 neon-skill-weather-1.0.1a1/skill/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.729481 neon-skill-weather-1.0.1a1/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/DailyColumn.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/DailyColumnScalable.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/DailyDelegateScalable.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/HourlyColumn.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/WeatherDate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/WeatherDelegateMarkII.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/WeatherDelegateScalable.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/WeatherImage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/WeatherLabel.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/WeatherLocation.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.733481 neon-skill-weather-1.0.1a1/ui/animations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4829 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/clouds.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5635 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/fog.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8559 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/partial_clouds.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64205 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/rain.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30103 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/sleet.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46868 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/snow.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/storm.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/animations/sun.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/current_1_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/current_1_scalable.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/current_2_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/current_2_scalable.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/daily_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/daily_scalable.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/hourly_mark_ii.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:59:38.733481 neon-skill-weather-1.0.1a1/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/clouds.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/fog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/high_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/humidity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/low_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/moon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/partial_clouds_day.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/partial_clouds_night.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/rain.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/snow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/storm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/sun.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/sunrise.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/sunset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/images/wind.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/single_day_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/ui/sunrise_sunset_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-10 23:59:33.000000 neon-skill-weather-1.0.1a1/version.py
```

### Comparing `neon-skill-weather-1.0.0/LICENSE` & `neon-skill-weather-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/LICENSE.md` & `neon-skill-weather-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/PKG-INFO` & `neon-skill-weather-1.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-weather
-Version: 1.0.0
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-weather
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-weather-1.0.0/README.md` & `neon-skill-weather-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/__init__.py` & `neon-skill-weather-1.0.1a1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,30 +46,30 @@
 proxies its calls to the API through Mycroft's officially supported API,
 Selene.  The Selene API is also used to get geographical information about the
 city name provided in the request.
 """
 
 from datetime import datetime
 from pathlib import Path
-from time import sleep, time
+from threading import Event
+from time import time
 from typing import List, Tuple, Optional
 
 from requests import HTTPError
-from mycroft_bus_client import Message
+from ovos_bus_client.message import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.signal_utils import wait_for_signal_clear
 from neon_utils.user_utils import get_user_prefs
+from lingua_franca.parse import extract_number
 
 from mycroft.skills import intent_handler, skill_api_method
 from mycroft.skills.intent_services.adapt_service import AdaptIntent
-from mycroft.messagebus.message import Message
-from mycroft.util.parse import extract_number
 
 from .skill import (
     CurrentDialog,
     DAILY,
     DailyDialog,
     DailyWeather,
     HOURLY,
@@ -714,42 +714,45 @@
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
         weather = self._get_weather(intent_data)
         weather_config = self._get_weather_config(message)
         if weather is not None:
-            weather_location = self._build_display_location(intent_data, weather_config)
+            weather_location = self._build_display_location(intent_data,
+                                                            weather_config)
             self._display_current_conditions(weather, weather_location)
             gui_start = time()
+            gui_waiter = Event()
             dialog = CurrentDialog(intent_data, weather_config, weather.current)
             dialog.build_weather_dialog()
             wait_for_signal_clear('isSpeaking')
             self._speak_weather(dialog)
+            # TODO: Refactor out `self.platform` checks
             if self.gui.connected and self.platform != MARK_II:
                 # Make sure the GUI page is shown for at least 10 seconds
-                while time() - gui_start < 10:
-                    sleep(1)
+                gui_waiter.wait(10 - (time() - gui_start))
                 wait_for_signal_clear('isSpeaking')
                 self._display_more_current_conditions(weather, weather_location)
-            dialog = CurrentDialog(intent_data, weather_config, weather.current)
+            # dialog = CurrentDialog(intent_data, weather_config, weather.current)
             dialog.build_high_low_temperature_dialog()
             self._speak_weather(dialog)
             if self.gui.connected:
                 # Make sure the GUI page is shown for at least 10 seconds
-                while time() - gui_start < 10:
-                    sleep(1)
+                gui_waiter.wait(10 - (time() - gui_start))
                 wait_for_signal_clear('isSpeaking')
                 if self.platform == MARK_II:
-                    self._display_more_current_conditions(weather, weather_location)
-                    sleep(10)
+                    self._display_more_current_conditions(weather,
+                                                          weather_location)
+                    gui_waiter.wait(10)
                     self._display_hourly_forecast(weather, weather_location)
                 else:
                     four_day_forecast = weather.daily[1:5]
-                    self._display_multi_day_forecast(four_day_forecast, intent_data)
+                    self._display_multi_day_forecast(four_day_forecast,
+                                                     intent_data)
 
     def _display_current_conditions(
         self, weather: WeatherReport, weather_location: str
     ):
         """Display current weather conditions on a screen.
 
         This is the first screen that shows.  Others will follow.
@@ -1055,18 +1058,19 @@
                     day=day.date_time.strftime("%a"),
                     highTemperature=day.temperature.high,
                     lowTemperature=day.temperature.low,
                 )
             )
         self.gui.clear()
         self.gui["dailyForecast"] = dict(days=daily_forecast[:4])
-        self.gui["weatherLocation"] = self._build_display_location(intent_data, WeatherConfig())
+        self.gui["weatherLocation"] = \
+            self._build_display_location(intent_data, WeatherConfig())
         self.gui.show_page(page_name)
         if len(forecast) > 4:
-            sleep(15)
+            Event().wait(15)
             self.gui.clear()
             self.gui["dailyForecast"] = dict(days=daily_forecast[4:])
             self.gui.show_page(page_name)
 
     def _display_multi_day_scalable(self, forecast: List[DailyWeather]):
         """Display daily forecast data on GUI devices other than the Mark II.
```

### Comparing `neon-skill-weather-1.0.0/locale/ca-es/dialog/daily/daily-weather-local.dialog` & `neon-skill-weather-1.0.1a1/locale/ca-es/dialog/daily/daily-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/da-dk/dialog/current/current-weather-location.dialog` & `neon-skill-weather-1.0.1a1/locale/da-dk/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-weather-local.dialog` & `neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/da-dk/dialog/daily/daily-weather-location.dialog` & `neon-skill-weather-1.0.1a1/locale/da-dk/dialog/daily/daily-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/da-dk/dialog/hourly/hourly-weather-location.dialog` & `neon-skill-weather-1.0.1a1/locale/da-dk/dialog/hourly/hourly-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/es-es/dialog/current/current-weather-local.dialog` & `neon-skill-weather-1.0.1a1/locale/es-es/dialog/current/current-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/es-es/dialog/current/current-weather-location.dialog` & `neon-skill-weather-1.0.1a1/locale/es-es/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/eu-eu/vocabulary/location.voc` & `neon-skill-weather-1.0.1a1/locale/eu-eu/vocabulary/location.voc`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/fr-fr/dialog/current/current-weather-local.dialog` & `neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/current/current-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/fr-fr/dialog/current/current-weather-location.dialog` & `neon-skill-weather-1.0.1a1/locale/fr-fr/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/nl-nl/dialog/current/current-weather-local.dialog` & `neon-skill-weather-1.0.1a1/locale/nl-nl/dialog/current/current-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/ru-ru/dialog/current/current-weather-location.dialog` & `neon-skill-weather-1.0.1a1/locale/ru-ru/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/ru-ru/vocabulary/date-time/number-days.voc` & `neon-skill-weather-1.0.1a1/locale/ru-ru/vocabulary/date-time/number-days.voc`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/locale/sv-se/dialog/daily/daily-weather-local.dialog` & `neon-skill-weather-1.0.1a1/locale/sv-se/dialog/daily/daily-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/neon_skill_weather.egg-info/PKG-INFO` & `neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-weather
-Version: 1.0.0
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-weather
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-weather-1.0.0/neon_skill_weather.egg-info/SOURCES.txt` & `neon-skill-weather-1.0.1a1/neon_skill_weather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/setup.py` & `neon-skill-weather-1.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/__init__.py` & `neon-skill-weather-1.0.1a1/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/api.py` & `neon-skill-weather-1.0.1a1/skill/api.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/config.py` & `neon-skill-weather-1.0.1a1/skill/config.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/dialog.py` & `neon-skill-weather-1.0.1a1/skill/dialog.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/intent.py` & `neon-skill-weather-1.0.1a1/skill/intent.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/util.py` & `neon-skill-weather-1.0.1a1/skill/util.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill/weather.py` & `neon-skill-weather-1.0.1a1/skill/weather.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/skill.json` & `neon-skill-weather-1.0.1a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/DailyColumn.qml` & `neon-skill-weather-1.0.1a1/ui/DailyColumn.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/DailyColumnScalable.qml` & `neon-skill-weather-1.0.1a1/ui/DailyColumnScalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/DailyDelegateScalable.qml` & `neon-skill-weather-1.0.1a1/ui/DailyDelegateScalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/HourlyColumn.qml` & `neon-skill-weather-1.0.1a1/ui/HourlyColumn.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/WeatherDate.qml` & `neon-skill-weather-1.0.1a1/ui/WeatherDate.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/WeatherDelegateMarkII.qml` & `neon-skill-weather-1.0.1a1/ui/WeatherDelegateMarkII.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/WeatherDelegateScalable.qml` & `neon-skill-weather-1.0.1a1/ui/WeatherDelegateScalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/WeatherImage.qml` & `neon-skill-weather-1.0.1a1/ui/WeatherImage.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/WeatherLabel.qml` & `neon-skill-weather-1.0.1a1/ui/WeatherLabel.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/WeatherLocation.qml` & `neon-skill-weather-1.0.1a1/ui/WeatherLocation.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/clouds.json` & `neon-skill-weather-1.0.1a1/ui/animations/clouds.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/fog.json` & `neon-skill-weather-1.0.1a1/ui/animations/fog.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/partial_clouds.json` & `neon-skill-weather-1.0.1a1/ui/animations/partial_clouds.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/rain.json` & `neon-skill-weather-1.0.1a1/ui/animations/rain.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/sleet.json` & `neon-skill-weather-1.0.1a1/ui/animations/sleet.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/snow.json` & `neon-skill-weather-1.0.1a1/ui/animations/snow.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/storm.json` & `neon-skill-weather-1.0.1a1/ui/animations/storm.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/animations/sun.json` & `neon-skill-weather-1.0.1a1/ui/animations/sun.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/current_1_mark_ii.qml` & `neon-skill-weather-1.0.1a1/ui/current_1_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/current_1_scalable.qml` & `neon-skill-weather-1.0.1a1/ui/current_1_scalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/current_2_mark_ii.qml` & `neon-skill-weather-1.0.1a1/ui/current_2_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/current_2_scalable.qml` & `neon-skill-weather-1.0.1a1/ui/current_2_scalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/daily_mark_ii.qml` & `neon-skill-weather-1.0.1a1/ui/daily_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/daily_scalable.qml` & `neon-skill-weather-1.0.1a1/ui/daily_scalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/hourly_mark_ii.qml` & `neon-skill-weather-1.0.1a1/ui/hourly_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/clouds.svg` & `neon-skill-weather-1.0.1a1/ui/images/clouds.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/fog.svg` & `neon-skill-weather-1.0.1a1/ui/images/fog.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/high_temperature.svg` & `neon-skill-weather-1.0.1a1/ui/images/high_temperature.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/humidity.svg` & `neon-skill-weather-1.0.1a1/ui/images/humidity.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/low_temperature.svg` & `neon-skill-weather-1.0.1a1/ui/images/low_temperature.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/partial_clouds_day.svg` & `neon-skill-weather-1.0.1a1/ui/images/partial_clouds_day.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/partial_clouds_night.svg` & `neon-skill-weather-1.0.1a1/ui/images/partial_clouds_night.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/rain.svg` & `neon-skill-weather-1.0.1a1/ui/images/rain.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/snow.svg` & `neon-skill-weather-1.0.1a1/ui/images/snow.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/storm.svg` & `neon-skill-weather-1.0.1a1/ui/images/storm.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/sun.svg` & `neon-skill-weather-1.0.1a1/ui/images/sun.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/sunrise.svg` & `neon-skill-weather-1.0.1a1/ui/images/sunrise.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/sunset.svg` & `neon-skill-weather-1.0.1a1/ui/images/sunset.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/images/wind.svg` & `neon-skill-weather-1.0.1a1/ui/images/wind.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/single_day_mark_ii.qml` & `neon-skill-weather-1.0.1a1/ui/single_day_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/ui/sunrise_sunset_mark_ii.qml` & `neon-skill-weather-1.0.1a1/ui/sunrise_sunset_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-1.0.0/version.py` & `neon-skill-weather-1.0.1a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1a1"
```

