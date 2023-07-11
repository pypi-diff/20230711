# Comparing `tmp/nopasaran-0.2.6.tar.gz` & `tmp/nopasaran-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.6.tar", last modified: Sun Jul  9 12:11:15 2023, max compression
+gzip compressed data, was "nopasaran-0.2.7.tar", last modified: Tue Jul 11 10:33:52 2023, max compression
```

## Comparing `nopasaran-0.2.6.tar` & `nopasaran-0.2.7.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 12:11:07.000000 nopasaran-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-09 12:11:15.164183 nopasaran-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-09 12:11:07.000000 nopasaran-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/control_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/errors/parsing_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/action_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/condition_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/machines/action_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/machines/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/parsers/interpreter_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/parsers/state_machine_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/action_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/action_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/control_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/event_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/io_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/ip_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/nested_machine_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/tcp_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/udp_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/condition_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/variable_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/assignment_transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/transition_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 12:11:15.164183 nopasaran-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-09 12:11:14.000000 nopasaran-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.221585 nopasaran-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 10:33:43.000000 nopasaran-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-11 10:33:52.217585 nopasaran-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-11 10:33:43.000000 nopasaran-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.201585 nopasaran-0.2.7/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.205585 nopasaran-0.2.7/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.205585 nopasaran-0.2.7/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.205585 nopasaran-0.2.7/nopasaran/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/errors/parsing_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.213585 nopasaran-0.2.7/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/primitives/action_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/action_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/control_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/dns_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/event_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/io_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/ip_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/nested_machine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/tcp_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/udp_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/condition_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/variable_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/assignment_transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.201585 nopasaran-0.2.7/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:33:52.221585 nopasaran-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 10:33:51.000000 nopasaran-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/tests/__init__.py
```

### Comparing `nopasaran-0.2.6/LICENSE` & `nopasaran-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/PKG-INFO` & `nopasaran-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.6
+Version: 0.2.7
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.6/README.md` & `nopasaran-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/__main__.py` & `nopasaran-0.2.7/nopasaran/__main__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/controllers/controller.py` & `nopasaran-0.2.7/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/controllers/factory.py` & `nopasaran-0.2.7/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/controllers/protocol.py` & `nopasaran-0.2.7/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/decorators.py` & `nopasaran-0.2.7/nopasaran/decorators.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/definitions/control_channel.py` & `nopasaran-0.2.7/nopasaran/definitions/control_channel.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/errors/parsing_error.py` & `nopasaran-0.2.7/nopasaran/errors/parsing_error.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.7/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.2.7/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/interpreters/interpreter.py` & `nopasaran-0.2.7/nopasaran/interpreters/interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.7/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.7/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/machines/action_queue.py` & `nopasaran-0.2.7/nopasaran/machines/action_queue.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/machines/state_machine.py` & `nopasaran-0.2.7/nopasaran/machines/state_machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.7/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/parsers/state_machine_parser.py` & `nopasaran-0.2.7/nopasaran/parsers/state_machine_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/action_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/action_primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from nopasaran.primitives.action_primitives.data_channel_primitives import DataChannelPrimitives
 from nopasaran.primitives.action_primitives.control_channel_primitives import ControlChannelPrimitives
 from nopasaran.primitives.action_primitives.event_primitives import EventPrimitives
 from nopasaran.primitives.action_primitives.io_primitives import IOPrimitives
 from nopasaran.primitives.action_primitives.ip_primitives import IPPrimitives
 from nopasaran.primitives.action_primitives.tcp_primitives import TCPPrimitives
 from nopasaran.primitives.action_primitives.udp_primitives import UDPPrimitives
+from nopasaran.primitives.action_primitives.dns_primitives import DNSPrimitives
 
 class ActionPrimitives(Primitives):
     """
     Class containing action primitives for the state machine.
     """
     classes = [
         DataManipulationPrimitives, 
         NestedMachinePrimitives, 
         DataChannelPrimitives, 
         ControlChannelPrimitives, 
         EventPrimitives, 
         IOPrimitives, 
         IPPrimitives, 
         TCPPrimitives, 
-        UDPPrimitives
+        UDPPrimitives,
+        DNSPrimitives
         ]
```

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/control_channel_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/control_channel_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_channel_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_channel_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             outputs (List[str]): The list of output variable names.
             
             state_machine: The state machine object.
 
         Returns:
             None
         """
-        state_machine.set_sniffer_filter(state_machine.get_variable_value(inputs[0]))
+        state_machine.update_sniffer_filter(state_machine.get_variable_value(inputs[0]))
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0)
     def wait_packet_signal(inputs, outputs, state_machine):
         """
         Wait for a packet to be available in the sniffer's packet stack stored in the machine's state.
         The sniffer's packet stack is created and populated in the 'listen' primitive.
```

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_manipulation.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/event_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/event_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/io_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/io_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/ip_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/ip_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/nested_machine_utils.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/nested_machine_utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/tcp_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/tcp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/action_primitives/udp_primitives.py` & `nopasaran-0.2.7/nopasaran/primitives/action_primitives/udp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/condition_primitives/variable_comparisons.py` & `nopasaran-0.2.7/nopasaran/primitives/condition_primitives/variable_comparisons.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/primitives/transition_primitives/assignment_transitions.py` & `nopasaran-0.2.7/nopasaran/primitives/transition_primitives/assignment_transitions.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.7/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran/utils.py` & `nopasaran-0.2.7/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.6/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.7/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.6
+Version: 0.2.7
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.6/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.7/nopasaran.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 nopasaran/primitives/__init__.py
 nopasaran/primitives/primitives.py
 nopasaran/primitives/action_primitives/__init__.py
 nopasaran/primitives/action_primitives/action_primitives.py
 nopasaran/primitives/action_primitives/control_channel_primitives.py
 nopasaran/primitives/action_primitives/data_channel_primitives.py
 nopasaran/primitives/action_primitives/data_manipulation.py
+nopasaran/primitives/action_primitives/dns_primitives.py
 nopasaran/primitives/action_primitives/event_primitives.py
 nopasaran/primitives/action_primitives/io_primitives.py
 nopasaran/primitives/action_primitives/ip_primitives.py
 nopasaran/primitives/action_primitives/nested_machine_utils.py
 nopasaran/primitives/action_primitives/tcp_primitives.py
 nopasaran/primitives/action_primitives/udp_primitives.py
 nopasaran/primitives/condition_primitives/__init__.py
```

### Comparing `nopasaran-0.2.6/setup.py` & `nopasaran-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.6',
+    version='0.2.7',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

