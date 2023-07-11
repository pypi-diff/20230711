# Comparing `tmp/crete-0.0.1.tar.gz` & `tmp/crete-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\_prog\dev\crete\dist\.tmp-juip1ytf\crete-0.0.1.tar", last modified: Sun Jul  9 15:49:59 2023, max compression
+gzip compressed data, was "C:\_prog\dev\crete\dist\.tmp-tfwxyuly\crete-0.2.0.tar", last modified: Tue Jul 11 11:44:17 2023, max compression
```

## Comparing `crete-0.0.1.tar` & `crete-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:49:59.565653 crete-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-05-08 22:10:22.000000 crete-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4306 2023-07-09 15:49:59.565653 crete-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3929 2023-05-10 22:21:41.000000 crete-0.0.1/README.md
--rw-rw-rw-   0        0        0      449 2023-05-10 13:40:45.000000 crete-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      221 2023-07-09 15:49:59.572656 crete-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-09 15:49:59.453657 crete-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 15:49:59.507652 crete-0.0.1/src/crete/
--rw-rw-rw-   0        0        0      272 2023-05-10 22:22:54.000000 crete-0.0.1/src/crete/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-10 22:22:54.000000 crete-0.0.1/src/crete/__main__.py
--rw-rw-rw-   0        0        0     1043 2023-07-09 14:53:58.000000 crete-0.0.1/src/crete/agent.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:49:59.544652 crete-0.0.1/src/crete/cli/
--rw-rw-rw-   0        0        0        0 2023-03-13 11:25:45.000000 crete-0.0.1/src/crete/cli/__init__.py
--rw-rw-rw-   0        0        0      625 2023-04-12 12:07:09.000000 crete-0.0.1/src/crete/cli/cli_utils.py
--rw-rw-rw-   0        0        0    10748 2023-07-09 15:35:24.000000 crete-0.0.1/src/crete/cli/concfile.py
--rw-rw-rw-   0        0        0     1150 2023-05-11 09:47:35.000000 crete-0.0.1/src/crete/cli/list.py
--rw-rw-rw-   0        0        0     7396 2023-07-09 15:19:53.000000 crete-0.0.1/src/crete/cli/main.py
--rw-rw-rw-   0        0        0     1708 2023-07-09 15:30:05.000000 crete-0.0.1/src/crete/cli/module.py
--rw-rw-rw-   0        0        0     8710 2023-07-09 15:08:52.000000 crete-0.0.1/src/crete/core.py
--rw-rw-rw-   0        0        0     1020 2023-05-11 10:12:12.000000 crete-0.0.1/src/crete/error.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:49:59.564652 crete-0.0.1/src/crete/file/
--rw-rw-rw-   0        0        0        0 2023-05-10 14:27:21.000000 crete-0.0.1/src/crete/file/__init__.py
--rw-rw-rw-   0        0        0     3557 2023-07-09 14:04:53.000000 crete-0.0.1/src/crete/file/concrete.py
--rw-rw-rw-   0        0        0      883 2023-05-10 20:58:24.000000 crete-0.0.1/src/crete/file/crete_config.py
--rw-rw-rw-   0        0        0     2859 2023-05-11 10:02:46.000000 crete-0.0.1/src/crete/file/profile.py
--rw-rw-rw-   0        0        0      429 2023-05-10 21:30:41.000000 crete-0.0.1/src/crete/global_state.py
--rw-rw-rw-   0        0        0     4085 2023-05-10 20:38:10.000000 crete-0.0.1/src/crete/registration.py
--rw-rw-rw-   0        0        0      313 2023-05-10 11:10:18.000000 crete-0.0.1/src/crete/types.py
--rw-rw-rw-   0        0        0     1732 2023-05-11 10:02:13.000000 crete-0.0.1/src/crete/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:49:59.530651 crete-0.0.1/src/crete.egg-info/
--rw-rw-rw-   0        0        0     4306 2023-07-09 15:49:59.000000 crete-0.0.1/src/crete.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-07-09 15:49:59.000000 crete-0.0.1/src/crete.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:49:59.000000 crete-0.0.1/src/crete.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-09 15:49:59.000000 crete-0.0.1/src/crete.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 15:49:59.000000 crete-0.0.1/src/crete.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 11:44:17.414749 crete-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-05-08 22:10:22.000000 crete-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6446 2023-07-11 11:44:17.414749 crete-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6067 2023-07-11 11:38:23.000000 crete-0.2.0/README.md
+-rw-rw-rw-   0        0        0      449 2023-07-11 11:40:23.000000 crete-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      221 2023-07-11 11:44:17.416751 crete-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 11:44:17.371750 crete-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 11:44:17.391750 crete-0.2.0/src/crete/
+-rw-rw-rw-   0        0        0      272 2023-05-10 22:22:54.000000 crete-0.2.0/src/crete/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 22:22:54.000000 crete-0.2.0/src/crete/__main__.py
+-rw-rw-rw-   0        0        0     1043 2023-07-09 14:53:58.000000 crete-0.2.0/src/crete/agent.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:44:17.407751 crete-0.2.0/src/crete/cli/
+-rw-rw-rw-   0        0        0        0 2023-03-13 11:25:45.000000 crete-0.2.0/src/crete/cli/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-04-12 12:07:09.000000 crete-0.2.0/src/crete/cli/cli_utils.py
+-rw-rw-rw-   0        0        0    10783 2023-07-11 09:32:34.000000 crete-0.2.0/src/crete/cli/concfile.py
+-rw-rw-rw-   0        0        0     1150 2023-05-11 09:47:35.000000 crete-0.2.0/src/crete/cli/list.py
+-rw-rw-rw-   0        0        0     7412 2023-07-11 09:29:12.000000 crete-0.2.0/src/crete/cli/main.py
+-rw-rw-rw-   0        0        0     1708 2023-07-09 15:30:05.000000 crete-0.2.0/src/crete/cli/module.py
+-rw-rw-rw-   0        0        0     8592 2023-07-11 10:50:34.000000 crete-0.2.0/src/crete/core.py
+-rw-rw-rw-   0        0        0     1020 2023-05-11 10:12:12.000000 crete-0.2.0/src/crete/error.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:44:17.412751 crete-0.2.0/src/crete/file/
+-rw-rw-rw-   0        0        0        0 2023-05-10 14:27:21.000000 crete-0.2.0/src/crete/file/__init__.py
+-rw-rw-rw-   0        0        0     3557 2023-07-09 14:04:53.000000 crete-0.2.0/src/crete/file/concrete.py
+-rw-rw-rw-   0        0        0      883 2023-05-10 20:58:24.000000 crete-0.2.0/src/crete/file/crete_config.py
+-rw-rw-rw-   0        0        0     2859 2023-05-11 10:02:46.000000 crete-0.2.0/src/crete/file/profile.py
+-rw-rw-rw-   0        0        0      429 2023-05-10 21:30:41.000000 crete-0.2.0/src/crete/global_state.py
+-rw-rw-rw-   0        0        0     4085 2023-05-10 20:38:10.000000 crete-0.2.0/src/crete/registration.py
+-rw-rw-rw-   0        0        0      313 2023-05-10 11:10:18.000000 crete-0.2.0/src/crete/types.py
+-rw-rw-rw-   0        0        0     1732 2023-05-11 10:02:13.000000 crete-0.2.0/src/crete/util.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:44:17.398751 crete-0.2.0/src/crete.egg-info/
+-rw-rw-rw-   0        0        0     6446 2023-07-11 11:44:17.000000 crete-0.2.0/src/crete.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-07-11 11:44:17.000000 crete-0.2.0/src/crete.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 11:44:17.000000 crete-0.2.0/src/crete.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-11 11:44:17.000000 crete-0.2.0/src/crete.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 11:44:17.000000 crete-0.2.0/src/crete.egg-info/top_level.txt
```

### Comparing `crete-0.0.1/LICENSE` & `crete-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/PKG-INFO` & `crete-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,99 @@
-Metadata-Version: 2.1
-Name: crete
-Version: 0.0.1
-Summary: An RL agent training assistant
-Author-email: Blair Cross <blair@bxsys.dev>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Crete
 
+[![PyPI version](https://badge.fury.io/py/crete.svg)](https://badge.fury.io/py/crete)
+
 ```
                _       
   ___ _ __ ___| |_ ___ 
  / __| '__/ _ \ __/ _ \
 | (__| | |  __/ ||  __/
  \___|_|  \___|\__\___|
 Reinforcement Learning CLI assistant.
 
 ```
 
 ## Installation
 
-Crete is not released for public use yet, and is not available of PyPI. 
+Crete is now officially on PyPI!
+
+```cmd
+
+pip install crete
+
+```
 
 ## Introduction
 
-Crete is a CLI for RL training. 
+Crete is a CLI for RL training.
 Named after the island that Talos, the first AI in human mythology, walked upon.
 
 It can be used as easily as:
 
 ```
 python -m crete --help
 ```
 
 ## Registering Agents, Environments and Wrappers
 
-To start using Crete, you must register (at least) one agent. 
+To start using Crete, you must register (at least) one agent.
 Crete already comes preloaded with all the OpenAI Gym(nasium) environments.
+You can register your own environments too, as long as they use the OpenAI Gym(nasium) API.
+More information on making enivironment can be found on
+the [Gym(nasium) website](https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/).
 
-Simply create a module containing an agent that inherits `crete.Agent`, for example;
+Agents must inherit the `crete.Agent` class. For example;
 
 ```
  cool_rl_project
- +- crete_profile.yaml
+ +- crete_profile.yaml  <- config file, more on this later.
  +- module_a 
  |  +- agents
  |  |  +- __init__.py
  |  |  +- agent_1.py
  |  +- etc...
 ```
 
 ```python
 # module_a/agent_1.py
 
 from crete import Agent, ExtraState, ProfileConfig
 
+
 class DQNAgent(Agent):
     def __init__(self, obs, n_actions, device='cpu') -> None:
         super().__init__("DQN")
         ...
 
     def get_action(self, obs, extra_state: ExtraState = None) -> Tuple[int, ExtraState]:
         """Request an action."""
         ...
 
-    def save(self) -> Dict:
+    def save(self) -> bytes:
         """Extract all policy data."""
         ...
 
-    def load(self, agent_data: Dict):
+    def load(self, agent_data: bytes):
         """Load policy data."""
         ...
 
+
 def dqn_training_wrapper(
         env_factory: Callable[[int], gym.Env],  # Function that creates the environment.
         agent: DQNAgent,  # The agent itself.
         config: ProfileConfig,  # Object with config values.
         artifacts: Dict,  # Empty map for storing training information.
         save_callback  # Function for saving agents, for instance at peak rewards.
 ):
     """The DQN training procedure."""
+    # Note that this function is outside the agent definition.
     ...
 ```
 
-And then register that agent in the modules initialisation file.
+And then register that agent in the module's initialisation file.
 There is also `register_env` and `register_wrapper` which work the same way.
 Environments and wrappers should use the OpenAI Gym(nasium) API.
 
 ```python
 # module_a/__init__.py
 
 from crete import register_agent
@@ -114,43 +116,84 @@
 
 ```
 python -m crete list agents
 ```
 
 ## Training Agents
 
+Previously we saw the training wrapper for the example DQN agent. It contained 5 parameters;
+
+- `env_factory: Callable[[int], gym.Env]`. This is the function that creates the environment.
+    - A factory is given instead of the environment itself to allow fresh environments to be created for evaluation.
+- `agent: Agent`. The agent itself.
+- `config: ProfileConfig`. The configuration profile containing agent and training parameters.
+- `artifacts: Dict`. An empty dictionary for storing training artifacts.
+    - Training artifacts are things like loss over time. These artifacts are saved in the concrete file.
+- `save_callback: SaveCallback`. Utility function for saving snapshots of the agent.
+    - Used like `save_callback(agent, artifacts, step_iteration, "autosave-name")`
+
 Agents can be trained using the `train` or `batch` command, which trains one or several 'profiles' respectively.
 A 'profile' is contained within a `.yaml` file, and may look like the following;
 
 ```yaml
 ---
 # crete_profile.yaml
 
 defaults: # Contains default `config` values that can be overridden. 
   batch_size: 32
   init_epsilon: 1
   final_epsilon: 0.1
   eval_freq: 1000
   gather_freq: 50
-  
+
 final_dqn_map_0: # Arbitrary profile ID, can be anything.
   agent_id: DQN # The ID of the registered agent to use.
   env_id: CartPole-v1 # The ID of the environment to use.
   env_args: # Arbitrary environment arguments that will be passed to the constructor
     render_mode: human
-  config: # Config values that can be accessed through the Profile object via the training wrapper.
-    total_steps :  40000
-    decay_steps :  38000
+  config: # Config values that can be accessed through the ProfileConfig object via the training wrapper.
+    total_steps: 40000
+    decay_steps: 38000
     replay_buffer_size: 10000
     batch_size: 128
-    refresh_target_network_freq :  1000
+    refresh_target_network_freq: 1000
     hidden_layers:
       - 64
       - 64
 ```
 
 Training is engaged by;
 
 ```
 python -m crete train crete_profile.yaml final_dqn_map_0 ; to train a specific profile or,
 python -m crete batch crete_profile.yaml                 ; to train all profiles within a file.
 ```
+
+## Saving Agents and their Performances
+
+Crete allows the entire training process and outcomes to be saved, for replaying, evaluating and comparing.
+All that is required is for the agent to implement the `save` and `load` methods, which serialise the agents weight data
+to bytes.
+Everything else is handled by Crete. 
+One would usually use `pickle` to achieve this.
+
+For example, with a PyTorch-based agent:
+
+```python
+def save(self) -> bytes:
+    data = {
+        "data": self.net.state_dict(),
+        "layers": self.net.hidden_layers
+    }
+
+    return pickle.dumps(data)
+
+
+def load(self, agent_data: bytes):
+    agent_dict = pickle.loads(agent_data)
+    data, layers = itemgetter("data", "layers")(agent_dict)
+
+    self.net.set_hidden_layers(layers)
+    self.net.load_state_dict(data)
+```
+
+Crete automatically saves the agent on completion of the training wrapper, or on keyboard interrupt.
```

### Comparing `crete-0.0.1/src/crete/agent.py` & `crete-0.2.0/src/crete/agent.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/cli/cli_utils.py` & `crete-0.2.0/src/crete/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/cli/concfile.py` & `crete-0.2.0/src/crete/cli/concfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     graph_agent(concfile.id, concfile.training_artifacts, ProfileConfig(concfile.config, {}))
 
 
 @concfile_app.command()
 def compare(
         paths: List[str] = typer.Argument(
             None,
-            help="Concfiles of agents to compare against each other."
+            help="Concfiles of agents to compare against each other.cnc."
         ),
         opt_env_args: List[str] = typer.Option(
             [],
             "--env-arg",
             help="Arguments to pass to the environment in the form `param=value`."
         ),
         opt_n_episodes: int = typer.Option(
@@ -171,18 +171,20 @@
             None,
             "--save-as",
             "-s",
             help="Prefix to save the graphs and data as."
         )
 ):
     """
-    Compare several agents against each other in an environment.
+    Compare several agents against each other.cnc in an environment.
     Agents must have a common environment, but can have different wrappers.
     """
 
+    load_extra_modules()
+
     opt_env_args = _convert_to_key_value_list(opt_env_args)
 
     loaded_agents = []
     for agent_concfile in paths:
         print(f" > {agent_concfile}... ", end="")
         try:
             # Load concfile.
@@ -200,15 +202,15 @@
                 "env_name": concfile.env_name,
                 "env_factory": agent_env_factory
             })
             extra_info = f"Uses {concfile.env_name}"
             extra_info += f" with wrapper {concfile.used_wrappers}." if concfile.used_wrappers else "."
             print(f"[bold green]success![/] {extra_info}")
         except RuntimeError as ex:
-            print("[bold red]failed![/] Couldn't load .conc file. " + str(ex))
+            print("[bold red]failed![/] Couldn't load .cnc file. " + str(ex))
         except AgentNotFound:
             print("[bold red]failed![/] Couldn't find agent definition. Make sure it's been registered.")
 
     # Check all the environments are the same.
     common_env_id = loaded_agents[0]["env_name"]
     if not all(agent["env_name"] == common_env_id for agent in loaded_agents):
         print("[bold red]Failure![/] Agents don't all use the same environment. Cannot proceed.")
```

### Comparing `crete-0.0.1/src/crete/cli/list.py` & `crete-0.2.0/src/crete/cli/list.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/cli/main.py` & `crete-0.2.0/src/crete/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 ):
 
     if save_path is None:
         save_path = f"{target_profile.name}.cnc"
 
     path = os.path.join(out_dir, save_path)
     if override is False and os.path.exists(path):
-        print(f"Profile {target_profile.name} already exists! To overwrite, set override to true.")
+        print(f"Profile {target_profile.name} already exists! To overwrite, --override, or set an alias with --as")
         return
 
     env_factory = create_env_factory(
         target_profile.env_id,
         target_profile.env_wrapper,
         env_args=target_profile.env_args
     )
```

### Comparing `crete-0.0.1/src/crete/cli/module.py` & `crete-0.2.0/src/crete/cli/module.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/core.py` & `crete-0.2.0/src/crete/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -199,31 +199,29 @@
 
     reward_mean = np.mean(total_ep_rewards).item()
     reward_err = std_err(total_ep_rewards)
     return reward_mean, reward_err, total_infos_mean, total_infos_err
 
 
 def create_save_callback(id: str, config: Dict, used_wrappers: str, env_name: str, env_args: Dict) -> Callable:
-    def callback(agent_data: Any, training_artifacts: Dict, step: int, prefix: str = None):
+    def callback(agent: Agent, training_artifacts: Dict, step: int, prefix: str = None):
         concfile = ConcreteFile(
             id=id,
-            agent_data=agent_data,
+            agent_data=agent.save(),
             training_artifacts=training_artifacts,
             config=config,
             used_wrappers=used_wrappers,
             env_name=env_name,
             env_args=env_args
         )
-        path_meta = "map-" + str(env_args["map_id"]) if "map_id" in env_args else "no-meta"
         filename_parts = [
             id,
             env_name,
-            path_meta,
             str(step),
-            "autosave.tal"
+            "autosave.cnc"
         ]
         if prefix:
             filename_parts.insert(0, prefix)
         concfile.write('-'.join(filename_parts))
 
     return callback
```

### Comparing `crete-0.0.1/src/crete/error.py` & `crete-0.2.0/src/crete/error.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/file/concrete.py` & `crete-0.2.0/src/crete/file/concrete.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/file/crete_config.py` & `crete-0.2.0/src/crete/file/crete_config.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/file/profile.py` & `crete-0.2.0/src/crete/file/profile.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/registration.py` & `crete-0.2.0/src/crete/registration.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete/util.py` & `crete-0.2.0/src/crete/util.py`

 * *Files identical despite different names*

### Comparing `crete-0.0.1/src/crete.egg-info/PKG-INFO` & `crete-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,111 @@
 Metadata-Version: 2.1
 Name: crete
-Version: 0.0.1
+Version: 0.2.0
 Summary: An RL agent training assistant
 Author-email: Blair Cross <blair@bxsys.dev>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Crete
 
+[![PyPI version](https://badge.fury.io/py/crete.svg)](https://badge.fury.io/py/crete)
+
 ```
                _       
   ___ _ __ ___| |_ ___ 
  / __| '__/ _ \ __/ _ \
 | (__| | |  __/ ||  __/
  \___|_|  \___|\__\___|
 Reinforcement Learning CLI assistant.
 
 ```
 
 ## Installation
 
-Crete is not released for public use yet, and is not available of PyPI. 
+Crete is now officially on PyPI!
+
+```cmd
+
+pip install crete
+
+```
 
 ## Introduction
 
-Crete is a CLI for RL training. 
+Crete is a CLI for RL training.
 Named after the island that Talos, the first AI in human mythology, walked upon.
 
 It can be used as easily as:
 
 ```
 python -m crete --help
 ```
 
 ## Registering Agents, Environments and Wrappers
 
-To start using Crete, you must register (at least) one agent. 
+To start using Crete, you must register (at least) one agent.
 Crete already comes preloaded with all the OpenAI Gym(nasium) environments.
+You can register your own environments too, as long as they use the OpenAI Gym(nasium) API.
+More information on making enivironment can be found on
+the [Gym(nasium) website](https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/).
 
-Simply create a module containing an agent that inherits `crete.Agent`, for example;
+Agents must inherit the `crete.Agent` class. For example;
 
 ```
  cool_rl_project
- +- crete_profile.yaml
+ +- crete_profile.yaml  <- config file, more on this later.
  +- module_a 
  |  +- agents
  |  |  +- __init__.py
  |  |  +- agent_1.py
  |  +- etc...
 ```
 
 ```python
 # module_a/agent_1.py
 
 from crete import Agent, ExtraState, ProfileConfig
 
+
 class DQNAgent(Agent):
     def __init__(self, obs, n_actions, device='cpu') -> None:
         super().__init__("DQN")
         ...
 
     def get_action(self, obs, extra_state: ExtraState = None) -> Tuple[int, ExtraState]:
         """Request an action."""
         ...
 
-    def save(self) -> Dict:
+    def save(self) -> bytes:
         """Extract all policy data."""
         ...
 
-    def load(self, agent_data: Dict):
+    def load(self, agent_data: bytes):
         """Load policy data."""
         ...
 
+
 def dqn_training_wrapper(
         env_factory: Callable[[int], gym.Env],  # Function that creates the environment.
         agent: DQNAgent,  # The agent itself.
         config: ProfileConfig,  # Object with config values.
         artifacts: Dict,  # Empty map for storing training information.
         save_callback  # Function for saving agents, for instance at peak rewards.
 ):
     """The DQN training procedure."""
+    # Note that this function is outside the agent definition.
     ...
 ```
 
-And then register that agent in the modules initialisation file.
+And then register that agent in the module's initialisation file.
 There is also `register_env` and `register_wrapper` which work the same way.
 Environments and wrappers should use the OpenAI Gym(nasium) API.
 
 ```python
 # module_a/__init__.py
 
 from crete import register_agent
@@ -114,43 +128,84 @@
 
 ```
 python -m crete list agents
 ```
 
 ## Training Agents
 
+Previously we saw the training wrapper for the example DQN agent. It contained 5 parameters;
+
+- `env_factory: Callable[[int], gym.Env]`. This is the function that creates the environment.
+    - A factory is given instead of the environment itself to allow fresh environments to be created for evaluation.
+- `agent: Agent`. The agent itself.
+- `config: ProfileConfig`. The configuration profile containing agent and training parameters.
+- `artifacts: Dict`. An empty dictionary for storing training artifacts.
+    - Training artifacts are things like loss over time. These artifacts are saved in the concrete file.
+- `save_callback: SaveCallback`. Utility function for saving snapshots of the agent.
+    - Used like `save_callback(agent, artifacts, step_iteration, "autosave-name")`
+
 Agents can be trained using the `train` or `batch` command, which trains one or several 'profiles' respectively.
 A 'profile' is contained within a `.yaml` file, and may look like the following;
 
 ```yaml
 ---
 # crete_profile.yaml
 
 defaults: # Contains default `config` values that can be overridden. 
   batch_size: 32
   init_epsilon: 1
   final_epsilon: 0.1
   eval_freq: 1000
   gather_freq: 50
-  
+
 final_dqn_map_0: # Arbitrary profile ID, can be anything.
   agent_id: DQN # The ID of the registered agent to use.
   env_id: CartPole-v1 # The ID of the environment to use.
   env_args: # Arbitrary environment arguments that will be passed to the constructor
     render_mode: human
-  config: # Config values that can be accessed through the Profile object via the training wrapper.
-    total_steps :  40000
-    decay_steps :  38000
+  config: # Config values that can be accessed through the ProfileConfig object via the training wrapper.
+    total_steps: 40000
+    decay_steps: 38000
     replay_buffer_size: 10000
     batch_size: 128
-    refresh_target_network_freq :  1000
+    refresh_target_network_freq: 1000
     hidden_layers:
       - 64
       - 64
 ```
 
 Training is engaged by;
 
 ```
 python -m crete train crete_profile.yaml final_dqn_map_0 ; to train a specific profile or,
 python -m crete batch crete_profile.yaml                 ; to train all profiles within a file.
 ```
+
+## Saving Agents and their Performances
+
+Crete allows the entire training process and outcomes to be saved, for replaying, evaluating and comparing.
+All that is required is for the agent to implement the `save` and `load` methods, which serialise the agents weight data
+to bytes.
+Everything else is handled by Crete. 
+One would usually use `pickle` to achieve this.
+
+For example, with a PyTorch-based agent:
+
+```python
+def save(self) -> bytes:
+    data = {
+        "data": self.net.state_dict(),
+        "layers": self.net.hidden_layers
+    }
+
+    return pickle.dumps(data)
+
+
+def load(self, agent_data: bytes):
+    agent_dict = pickle.loads(agent_data)
+    data, layers = itemgetter("data", "layers")(agent_dict)
+
+    self.net.set_hidden_layers(layers)
+    self.net.load_state_dict(data)
+```
+
+Crete automatically saves the agent on completion of the training wrapper, or on keyboard interrupt.
```

### Comparing `crete-0.0.1/src/crete.egg-info/SOURCES.txt` & `crete-0.2.0/src/crete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

