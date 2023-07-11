# Comparing `tmp/mobile-env-2.0.0.tar.gz` & `tmp/mobile-env-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobile-env-2.0.0.tar", last modified: Fri Apr 28 17:28:46 2023, max compression
+gzip compressed data, was "mobile-env-2.0.1.tar", last modified: Tue Jul 11 19:58:16 2023, max compression
```

## Comparing `mobile-env-2.0.0.tar` & `mobile-env-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 17:28:36.000000 mobile-env-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-28 17:28:46.061926 mobile-env-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-28 17:28:36.000000 mobile-env-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.057926 mobile-env-2.0.0/mobile_env/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/arrival.py
--rw-r--r--   0 runner    (1001) docker     (123)    28237 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/central.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/handlers/multi_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/large.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/scenarios/small.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/mobile_env/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-28 17:28:36.000000 mobile-env-2.0.0/mobile_env/wrappers/multi_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.057926 mobile-env-2.0.0/mobile_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 17:28:46.000000 mobile-env-2.0.0/mobile_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 17:28:46.061926 mobile-env-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 17:28:36.000000 mobile-env-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:46.061926 mobile-env-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:28:36.000000 mobile-env-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-28 17:28:36.000000 mobile-env-2.0.0/tests/test_central_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 17:28:36.000000 mobile-env-2.0.0/tests/test_env_stepping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.055362 mobile-env-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 19:58:05.000000 mobile-env-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-07-11 19:58:16.055362 mobile-env-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-11 19:58:05.000000 mobile-env-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.051362 mobile-env-2.0.1/mobile_env/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.051362 mobile-env-2.0.1/mobile_env/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/arrival.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28236 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.051362 mobile-env-2.0.1/mobile_env/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/handlers/central.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/handlers/multi_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.051362 mobile-env-2.0.1/mobile_env/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/scenarios/large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/scenarios/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/scenarios/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/scenarios/small.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.051362 mobile-env-2.0.1/mobile_env/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-11 19:58:05.000000 mobile-env-2.0.1/mobile_env/wrappers/multi_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.051362 mobile-env-2.0.1/mobile_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-07-11 19:58:15.000000 mobile-env-2.0.1/mobile_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-11 19:58:15.000000 mobile-env-2.0.1/mobile_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:58:15.000000 mobile-env-2.0.1/mobile_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:58:15.000000 mobile-env-2.0.1/mobile_env.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 19:58:15.000000 mobile-env-2.0.1/mobile_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 19:58:15.000000 mobile-env-2.0.1/mobile_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 19:58:16.055362 mobile-env-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 19:58:05.000000 mobile-env-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:16.055362 mobile-env-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:05.000000 mobile-env-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-11 19:58:05.000000 mobile-env-2.0.1/tests/test_central_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-11 19:58:05.000000 mobile-env-2.0.1/tests/test_env_stepping.py
```

### Comparing `mobile-env-2.0.0/LICENSE` & `mobile-env-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/PKG-INFO` & `mobile-env-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobile-env
-Version: 2.0.0
+Version: 2.0.1
 Summary: mobile-env: An Open Environment for Autonomous Coordination in Wireless Mobile Networks
 Home-page: https://github.com/stefanbschneider/mobile-env
 Author: Stefan Schneider, Stefan Werner
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,18 @@
 [![Documentation](https://readthedocs.org/projects/mobile-env/badge/?version=latest)](https://mobile-env.readthedocs.io/en/latest/?badge=latest)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)
 
 
 # mobile-env: An Open Environment for Autonomous Coordination in Mobile Networks
 
-mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks.
+mobile-env is an open, minimalist environment for training and evaluating coordination algorithms in wireless mobile networks.
 The environment allows modeling users moving around an area and can connect to one or multiple base stations.
-Using the Gym interface, the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
+Using the [Gymnasium](https://gymnasium.farama.org/) ([previously Gym](https://www.gymlibrary.dev/)) interface,
+the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
 The environment is highly configurable and can be easily extended (e.g., regarding users, movement patterns, channel models, etc.).
 
 mobile-env supports multi-agent and centralized reinforcement learning policies. It provides various choices for rewards and observations. mobile-env is also easily extendable, so that anyone may add another channel models (e.g. path loss), movement patterns, utility functions, etc.
 
 As an example, mobile-env can be used to study multi-cell selection in coordinated multipoint.
 Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally.
 To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates.
@@ -88,18 +89,18 @@
 
 If you want to run tests or examples, also install the requirements in `tests`.
 For dependencies for building docs, install the requirements in `docs`.
 
 ## Example Usage
 
 ```python
-import gymnasium as gym
+import gymnasium
 import mobile_env
 
-env = gym.make("mobile-medium-central-v0")
+env = gymnasium.make("mobile-medium-central-v0")
 obs, info = env.reset()
 done = False
 
 while not done:
     action = ... # Your agent code here
     obs, reward, terminated, truncated, info = env.step(action)
     done = terminated or truncated
@@ -108,15 +109,15 @@
 
 ## Customization
 
 mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions.
 For example, replacing the default [Okumura–Hata](https://en.wikipedia.org/wiki/Hata_model) channel model by a (simplified) path loss model can be as easy as this:
 
 ```python
-import gymnasium as gym
+import gymnasium
 import numpy as np
 from mobile_env.core.base import MComCore
 from mobile_env.core.channel import Channel
 
 
 class PathLoss(Channel):
     def __init__(self, gamma, **kwargs):
@@ -135,15 +136,15 @@
 config = MComCore.default_config()
 config['channel'] = PathLoss
 
 # pass init parameters to custom channel class!
 config['channel_params'].update({'gamma': 2.0})
 
 # create environment with custom channel model
-env = gym.make('mobile-small-central-v0', config=config)
+env = gymnasium.make('mobile-small-central-v0', config=config)
 # ...
 ```
 
 ## Projects Using mobile-env
 
 If you are using `movile-env`, please let us know and we are happy to link to your project from the readme. You can also open a pull request yourself.
```

### Comparing `mobile-env-2.0.0/README.md` & `mobile-env-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 [![Documentation](https://readthedocs.org/projects/mobile-env/badge/?version=latest)](https://mobile-env.readthedocs.io/en/latest/?badge=latest)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)
 
 
 # mobile-env: An Open Environment for Autonomous Coordination in Mobile Networks
 
-mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks.
+mobile-env is an open, minimalist environment for training and evaluating coordination algorithms in wireless mobile networks.
 The environment allows modeling users moving around an area and can connect to one or multiple base stations.
-Using the Gym interface, the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
+Using the [Gymnasium](https://gymnasium.farama.org/) ([previously Gym](https://www.gymlibrary.dev/)) interface,
+the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
 The environment is highly configurable and can be easily extended (e.g., regarding users, movement patterns, channel models, etc.).
 
 mobile-env supports multi-agent and centralized reinforcement learning policies. It provides various choices for rewards and observations. mobile-env is also easily extendable, so that anyone may add another channel models (e.g. path loss), movement patterns, utility functions, etc.
 
 As an example, mobile-env can be used to study multi-cell selection in coordinated multipoint.
 Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally.
 To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates.
@@ -74,18 +75,18 @@
 
 If you want to run tests or examples, also install the requirements in `tests`.
 For dependencies for building docs, install the requirements in `docs`.
 
 ## Example Usage
 
 ```python
-import gymnasium as gym
+import gymnasium
 import mobile_env
 
-env = gym.make("mobile-medium-central-v0")
+env = gymnasium.make("mobile-medium-central-v0")
 obs, info = env.reset()
 done = False
 
 while not done:
     action = ... # Your agent code here
     obs, reward, terminated, truncated, info = env.step(action)
     done = terminated or truncated
@@ -94,15 +95,15 @@
 
 ## Customization
 
 mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions.
 For example, replacing the default [Okumura–Hata](https://en.wikipedia.org/wiki/Hata_model) channel model by a (simplified) path loss model can be as easy as this:
 
 ```python
-import gymnasium as gym
+import gymnasium
 import numpy as np
 from mobile_env.core.base import MComCore
 from mobile_env.core.channel import Channel
 
 
 class PathLoss(Channel):
     def __init__(self, gamma, **kwargs):
@@ -121,15 +122,15 @@
 config = MComCore.default_config()
 config['channel'] = PathLoss
 
 # pass init parameters to custom channel class!
 config['channel_params'].update({'gamma': 2.0})
 
 # create environment with custom channel model
-env = gym.make('mobile-small-central-v0', config=config)
+env = gymnasium.make('mobile-small-central-v0', config=config)
 # ...
 ```
 
 ## Projects Using mobile-env
 
 If you are using `movile-env`, please let us know and we are happy to link to your project from the readme. You can also open a pull request yourself.
```

### Comparing `mobile-env-2.0.0/mobile_env/core/arrival.py` & `mobile-env-2.0.1/mobile_env/core/arrival.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/base.py` & `mobile-env-2.0.1/mobile_env/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import string
 from collections import Counter, defaultdict
 from typing import Dict, List, Set, Tuple
 
-import gymnasium as gym
+import gymnasium
 import matplotlib.patheffects as pe
 import matplotlib.pyplot as plt
 import numpy as np
 import pygame
 from matplotlib import cm
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 from pygame import Surface
@@ -19,15 +19,15 @@
 from mobile_env.core.movement import RandomWaypointMovement
 from mobile_env.core.schedules import ResourceFair
 from mobile_env.core.util import BS_SYMBOL, deep_dict_merge
 from mobile_env.core.utilities import BoundedLogUtility
 from mobile_env.handlers.central import MComCentralHandler
 
 
-class MComCore(gym.Env):
+class MComCore(gymnasium.Env):
     NOOP_ACTION = 0
     metadata = {"render_modes": ["rgb_array", "human"]}
 
     def __init__(self, stations, users, config={}, render_mode=None):
         super().__init__()
 
         self.render_mode = render_mode
```

### Comparing `mobile-env-2.0.0/mobile_env/core/channels.py` & `mobile-env-2.0.1/mobile_env/core/channels.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/entities.py` & `mobile-env-2.0.1/mobile_env/core/entities.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/logging.py` & `mobile-env-2.0.1/mobile_env/core/logging.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/metrics.py` & `mobile-env-2.0.1/mobile_env/core/metrics.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/movement.py` & `mobile-env-2.0.1/mobile_env/core/movement.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/schedules.py` & `mobile-env-2.0.1/mobile_env/core/schedules.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/util.py` & `mobile-env-2.0.1/mobile_env/core/util.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/core/utilities.py` & `mobile-env-2.0.1/mobile_env/core/utilities.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/handlers/central.py` & `mobile-env-2.0.1/mobile_env/handlers/central.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/handlers/handler.py` & `mobile-env-2.0.1/mobile_env/handlers/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from typing import Dict
 
 from gymnasium.spaces.space import Space
 
 
 class Handler:
-    """Defines Gym interface methods called by core simulation."""
+    """Defines Gymnasium interface methods called by core simulation."""
 
     @classmethod
     @abc.abstractmethod
     def action_space(cls, env) -> Space:
         """Defines action space for passed environment."""
         pass
```

### Comparing `mobile-env-2.0.0/mobile_env/handlers/multi_agent.py` & `mobile-env-2.0.1/mobile_env/handlers/multi_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-import gymnasium as gym
+import gymnasium
 import numpy as np
 
 from mobile_env.handlers.handler import Handler
 
 
 class MComMAHandler(Handler):
     features = [
@@ -16,31 +16,31 @@
     ]
 
     @classmethod
     def ue_obs_size(cls, env) -> int:
         return sum(env.feature_sizes[ftr] for ftr in cls.features)
 
     @classmethod
-    def action_space(cls, env) -> gym.spaces.Dict:
-        return gym.spaces.Dict(
+    def action_space(cls, env) -> gymnasium.spaces.Dict:
+        return gymnasium.spaces.Dict(
             {
-                ue.ue_id: gym.spaces.Discrete(env.NUM_STATIONS + 1)
+                ue.ue_id: gymnasium.spaces.Discrete(env.NUM_STATIONS + 1)
                 for ue in env.users.values()
             }
         )
 
     @classmethod
-    def observation_space(cls, env) -> gym.spaces.Dict:
+    def observation_space(cls, env) -> gymnasium.spaces.Dict:
         size = cls.ue_obs_size(env)
         space = {
-            ue_id: gym.spaces.Box(low=-1, high=1, shape=(size,), dtype=np.float32)
+            ue_id: gymnasium.spaces.Box(low=-1, high=1, shape=(size,), dtype=np.float32)
             for ue_id in env.users
         }
 
-        return gym.spaces.Dict(space)
+        return gymnasium.spaces.Dict(space)
 
     @classmethod
     def reward(cls, env):
         """UE's reward is their utility and the avg. utility of nearby BSs."""
         # compute average utility of UEs for each BS
         # set to lower bound if no UEs are connected
         bs_utilities = env.station_utilities()
@@ -64,15 +64,15 @@
         return rewards
 
     @classmethod
     def observation(cls, env) -> Dict[int, np.ndarray]:
         """Select features for MA setting & flatten each UE's features."""
 
         # get features for currently active UEs
-        active = set([ue.ue_id for ue in env.active if not env.done])
+        active = set([ue.ue_id for ue in env.active if not env.time_is_up])
         features = env.features()
         features = {ue_id: obs for ue_id, obs in features.items() if ue_id in active}
 
         # select observations for multi-agent setting from base feature set
         obs = {
             ue_id: [obs_dict[key] for key in cls.features]
             for ue_id, obs_dict in features.items()
```

### Comparing `mobile-env-2.0.0/mobile_env/scenarios/large.py` & `mobile-env-2.0.1/mobile_env/scenarios/large.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/scenarios/medium.py` & `mobile-env-2.0.1/mobile_env/scenarios/medium.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/scenarios/registry.py` & `mobile-env-2.0.1/mobile_env/scenarios/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import itertools
 
-import gymnasium as gym
+import gymnasium
 
 from mobile_env.handlers.central import MComCentralHandler
 from mobile_env.handlers.multi_agent import MComMAHandler
 from mobile_env.scenarios.large import MComLarge
 from mobile_env.scenarios.medium import MComMedium
 from mobile_env.scenarios.small import MComSmall
 
 scenarios = {"small": MComSmall, "medium": MComMedium, "large": MComLarge}
 handlers = {"ma": MComMAHandler, "central": MComCentralHandler}
 
 for scenario, handler in itertools.product(scenarios, handlers):
     env_name = scenarios[scenario].__name__
     config = {"handler": handlers[handler]}
-    gym.envs.register(
+    gymnasium.envs.register(
         id=f"mobile-{scenario}-{handler}-v0",
         entry_point=f"mobile_env.scenarios.{scenario}:{env_name}",
         kwargs={"config": config},
     )
```

### Comparing `mobile-env-2.0.0/mobile_env/scenarios/small.py` & `mobile-env-2.0.1/mobile_env/scenarios/small.py`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/mobile_env/wrappers/multi_agent.py` & `mobile-env-2.0.1/mobile_env/wrappers/multi_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple
 
-import gymnasium as gym
+import gymnasium
 import numpy as np
 from ray.rllib.env.multi_agent_env import MultiAgentEnv
 from ray.rllib.utils.typing import MultiAgentDict
 
 
 class RLlibMAWrapper(MultiAgentEnv):
     def __init__(self, env):
@@ -15,17 +15,17 @@
         self.num_agents = len(self.env.users)
         # set max. number of steps for RLlib trainer
         self.max_episode_steps = self.env.EP_MAX_TIME
 
         # override action and observation space defined for wrapped environment
         # RLlib expects the action and observation space
         # to be defined per actor, i.e, per UE
-        self.action_space = gym.spaces.Discrete(self.env.NUM_STATIONS + 1)
+        self.action_space = gymnasium.spaces.Discrete(self.env.NUM_STATIONS + 1)
         size = self.env.handler.ue_obs_size(self.env)
-        self.observation_space = gym.spaces.Box(
+        self.observation_space = gymnasium.spaces.Box(
             low=-1, high=1, shape=(size,), dtype=np.float32
         )
 
         # track UE IDs of last observation's dictionary, i.e.,
         # what UEs were active in the previous step
         self.prev_step_ues = None
 
@@ -53,14 +53,18 @@
         ), "There is no natural episode termination. terminated should be False."
         terminateds = {ue_id: False for ue_id in self.prev_step_ues}
         terminateds["__all__"] = False
 
         # update keys of previous observation dictionary
         self.prev_step_ues = set(obs.keys())
 
+        # RLlib expects the keys of infos to be a subset of obs + __common__
+        # Put all infos under __common__
+        infos = {"__common__": infos}
+
         return obs, rews, terminateds, truncateds, infos
 
     def render(self) -> None:
         return self.env.render()
 
 
 class PettingZooWrapper:
```

### Comparing `mobile-env-2.0.0/mobile_env.egg-info/PKG-INFO` & `mobile-env-2.0.1/mobile_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobile-env
-Version: 2.0.0
+Version: 2.0.1
 Summary: mobile-env: An Open Environment for Autonomous Coordination in Wireless Mobile Networks
 Home-page: https://github.com/stefanbschneider/mobile-env
 Author: Stefan Schneider, Stefan Werner
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,18 @@
 [![Documentation](https://readthedocs.org/projects/mobile-env/badge/?version=latest)](https://mobile-env.readthedocs.io/en/latest/?badge=latest)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stefanbschneider/mobile-env/blob/master/examples/demo.ipynb)
 
 
 # mobile-env: An Open Environment for Autonomous Coordination in Mobile Networks
 
-mobile-env is an open, minimalist OpenAI Gym environment for training and evaluating coordination algorithms in wireless mobile networks.
+mobile-env is an open, minimalist environment for training and evaluating coordination algorithms in wireless mobile networks.
 The environment allows modeling users moving around an area and can connect to one or multiple base stations.
-Using the Gym interface, the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
+Using the [Gymnasium](https://gymnasium.farama.org/) ([previously Gym](https://www.gymlibrary.dev/)) interface,
+the environment can be used with any reinforcement learning framework (e.g., stable-baselines or Ray RLlib) or any custom (even non-RL) coordination approach.
 The environment is highly configurable and can be easily extended (e.g., regarding users, movement patterns, channel models, etc.).
 
 mobile-env supports multi-agent and centralized reinforcement learning policies. It provides various choices for rewards and observations. mobile-env is also easily extendable, so that anyone may add another channel models (e.g. path loss), movement patterns, utility functions, etc.
 
 As an example, mobile-env can be used to study multi-cell selection in coordinated multipoint.
 Here, it must be decided what connections should be established among user equipments (UEs) and base stations (BSs) in order to maximize Quality of Experience (QoE) globally.
 To maximize the QoE of single UEs, the UE intends to connect to as many BSs as possible, which yields higher (macro) data rates.
@@ -88,18 +89,18 @@
 
 If you want to run tests or examples, also install the requirements in `tests`.
 For dependencies for building docs, install the requirements in `docs`.
 
 ## Example Usage
 
 ```python
-import gymnasium as gym
+import gymnasium
 import mobile_env
 
-env = gym.make("mobile-medium-central-v0")
+env = gymnasium.make("mobile-medium-central-v0")
 obs, info = env.reset()
 done = False
 
 while not done:
     action = ... # Your agent code here
     obs, reward, terminated, truncated, info = env.step(action)
     done = terminated or truncated
@@ -108,15 +109,15 @@
 
 ## Customization
 
 mobile-env supports custom channel models, movement patterns, arrival & departure models, resource multiplexing schemes and utility functions.
 For example, replacing the default [Okumura–Hata](https://en.wikipedia.org/wiki/Hata_model) channel model by a (simplified) path loss model can be as easy as this:
 
 ```python
-import gymnasium as gym
+import gymnasium
 import numpy as np
 from mobile_env.core.base import MComCore
 from mobile_env.core.channel import Channel
 
 
 class PathLoss(Channel):
     def __init__(self, gamma, **kwargs):
@@ -135,15 +136,15 @@
 config = MComCore.default_config()
 config['channel'] = PathLoss
 
 # pass init parameters to custom channel class!
 config['channel_params'].update({'gamma': 2.0})
 
 # create environment with custom channel model
-env = gym.make('mobile-small-central-v0', config=config)
+env = gymnasium.make('mobile-small-central-v0', config=config)
 # ...
 ```
 
 ## Projects Using mobile-env
 
 If you are using `movile-env`, please let us know and we are happy to link to your project from the readme. You can also open a pull request yourself.
```

### Comparing `mobile-env-2.0.0/mobile_env.egg-info/SOURCES.txt` & `mobile-env-2.0.1/mobile_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobile-env-2.0.0/setup.py` & `mobile-env-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "pygame",
     "shapely",
     "svgpath2mpl",
 ]
 
 setup(
     name="mobile-env",
-    version="2.0.0",
+    version="2.0.1",
     author="Stefan Schneider, Stefan Werner",
     description="mobile-env: An Open Environment for Autonomous Coordination in "
     "Wireless Mobile Networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stefanbschneider/mobile-env",
     packages=find_packages(),
```

### Comparing `mobile-env-2.0.0/tests/test_env_stepping.py` & `mobile-env-2.0.1/tests/test_env_stepping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Simple test of small env similar to test notebook."""
-import gymnasium as gym
+import gymnasium
 import pytest
 
 # importing mobile_env automatically registers the predefined scenarios in Gym
-import mobile_env
+import mobile_env  # noqa: F401
 
 
 @pytest.mark.parametrize(
     "env_name",
     ["mobile-small-central-v0", "mobile-medium-central-v0", "mobile-large-central-v0"],
 )
 def test_env_stepping(env_name):
     """Create a mobile-env and run with random actions until done.
 
     Just to ensure that it does not crash.
     """
     # create a small mobile environment for a single, centralized control agent
-    env = gym.make(env_name)
+    env = gymnasium.make(env_name)
     obs, info = env.reset()
     done = False
 
     while not done:
         random_action = env.action_space.sample()
         obs, reward, terminated, truncated, info = env.step(random_action)
         done = terminated or truncated
```

