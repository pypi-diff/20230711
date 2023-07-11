# Comparing `tmp/agency-1.1.0.tar.gz` & `tmp/agency-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.1.0.tar", max compression
+gzip compressed data, was "agency-1.1.1.tar", max compression
```

## Comparing `agency-1.1.0.tar` & `agency-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35148 2023-07-07 21:43:06.527332 agency-1.1.0/LICENSE
--rw-r--r--   0        0        0     9474 2023-07-07 21:43:06.527332 agency-1.1.0/README.md
--rw-r--r--   0        0        0       40 2023-07-07 21:43:06.527332 agency-1.1.0/agency/__init__.py
--rw-r--r--   0        0        0     9470 2023-07-07 21:43:06.527332 agency-1.1.0/agency/agent.py
--rw-r--r--   0        0        0      802 2023-07-07 21:43:06.527332 agency-1.1.0/agency/schema.py
--rwxr-xr-x   0        0        0     8762 2023-07-07 21:43:06.527332 agency-1.1.0/agency/space.py
--rw-r--r--   0        0        0     3824 2023-07-07 21:43:06.527332 agency-1.1.0/agency/util.py
--rw-r--r--   0        0        0      560 2023-07-07 21:43:07.647329 agency-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10191 1970-01-01 00:00:00.000000 agency-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-11 02:07:16.551773 agency-1.1.1/LICENSE
+-rw-r--r--   0        0        0     9363 2023-07-11 02:07:16.551773 agency-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 02:07:16.551773 agency-1.1.1/agency/__init__.py
+-rw-r--r--   0        0        0     9470 2023-07-11 02:07:16.551773 agency-1.1.1/agency/agent.py
+-rw-r--r--   0        0        0      802 2023-07-11 02:07:16.551773 agency-1.1.1/agency/schema.py
+-rwxr-xr-x   0        0        0     8876 2023-07-11 02:07:16.551773 agency-1.1.1/agency/space.py
+-rw-r--r--   0        0        0     3824 2023-07-11 02:07:16.551773 agency-1.1.1/agency/util.py
+-rw-r--r--   0        0        0      539 2023-07-11 02:07:18.035794 agency-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10037 1970-01-01 00:00:00.000000 agency-1.1.1/PKG-INFO
```

### Comparing `agency-1.1.0/LICENSE` & `agency-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.1.0/README.md` & `agency-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # Summary
 
-`agency` defines a common communication and action framework for creating AI
-agent integrated applications.
+`agency` is a python library that provides a communication and action framework
+for creating AI agent integrated applications.
 
 The library provides a low-level means for connecting agents, systems, and human
 users by defining actions, callbacks, and access policies that you can use to
-monitor, control, and interact with your agents.
+connect, monitor, control, and interact with your agents.
 
 `agency` handles the details of the common messaging system and allows
 discovering and invoking actions across parties, automatically handling things
 such as reporting exceptions, enforcing access restrictions, and more.
 
-`agency`'s purpose is to support agent development and integration by allowing
-you to create dynamic environments for your agents to freely work in a safe and
-controllable way, and to leave all other details up to you.
-
-Set your agents free (or just as much as you want) with `agency`!
-
 
 ## Features
 
 ### Low-Level API Flexibility
   * Straightforward class/method based agent and action definition
   * Supports defining single process applications or networked agent systems
   using AMQP
 
 ### Observability and Control
-  * Before/After action callbacks for observability or other needs
+  * Before/after action and lifecycle callbacks for observability or other needs
   * Access policies and permission callbacks for access control
 
 ### Performance
   * Multithreaded (though python's GIL is a bottleneck for single process apps)
   * AMQP support for multiprocess and networked systems (avoids GIL)
   * [_Python multiprocess support is planned for better scalability on
     single-host systems_](https://github.com/operand/agency/issues/33)
@@ -38,15 +32,15 @@
 ### Multimodal (image/audio) support
   * [_Not yet developed, but is planned_](https://github.com/operand/agency/issues/27)
 
 ### Full demo available at [`examples/demo`](./examples/demo/)
   * Two OpenAI agent examples
   * HuggingFace transformers agent example
   * Simple Flask/React web interface included
-  * Direct host access for agents
+  * Operating system access for agents
   * Docker configuration for reference and development
 
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
@@ -86,31 +80,37 @@
 
 ```python
   @access_policy(ACCESS_PERMITTED) # This allows the action at any time
   def _action__add(a, b):
     ...
 ```
 
-You can also define before/after and permission callbacks for various purposes:
+You can also define callbacks for various purposes:
 
 ```python
 class CalculatorAgent(Agent):
   ...
   def _before_action(self, original_message: dict):
     # Called before any action is attempted
 
   def _after_action(self, original_message: dict, return_value: str, error: str):
     # Called after any action is attempted
 
+  def _after_add(self):
+    # Called after the agent is added to the space and may begin communicating
+
+  def _before_remove(self):
+    # Called before the agent is removed from the space
+
   def _request_permission(self, proposed_message: dict) -> bool:
     # Called before an ACCESS_REQUESTED action is attempted for run-time review
 ```
 
 A `Space` is how you connect your agents together. An agent cannot communicate
-with others until it is added to a common "space".
+with others until it is added to a common `Space`.
 
 There are two included `Space` implementations to choose from:
 * `NativeSpace` - which connects agents within the same python process
 * `AMQPSpace` - which connects agents across processes and systems using an AMQP
   server like RabbitMQ.
 
 Here is an example of creating a `NativeSpace` and adding two agents to it.
@@ -136,20 +136,19 @@
 poetry add agency
 ```
 
 
 # Running the Demo Application
 
 To run the demo, please follow the directions at
-[examples/demo](./examples/demo/).
+[examples/demo](./examples/demo/). After a short boot time you can visit the
+web app at `http://localhost:8080` and you should see a simple chat interface.
 
-After a short boot time you can visit the web app at `http://localhost:8080` and
-you should see a simple chat interface. The following is a screenshot of a
-conversation that demonstrates multiple agents intelligently interacting and
-following orders.
+The following is a screenshot of the web UI that demonstrates the multiple demo
+agents intelligently interacting and following orders.
 
 There are two OpenAI based agents: `"FunctionAI"` and `"CompletionAI"`, named
 for the API's they use, and `"Chatty"` a simple chat agent who uses a small
 local transformers based model for demonstration.
 
 The screenshot also demonstrates the results of rejecting an action and
 directing an agent to use a different approach in real time. After I explained
@@ -165,28 +164,25 @@
 
 # FAQ
 
 ## How does `agency` compare to agent libraries like LangChain?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be a full-fledged agent toolset.
+intended to be a full-fledged agent toolset like other libraries or tools.
 
-Projects like LangChain and others are exploring how to create purpose-built
-agents that solve diverse problems using tools. `agency` is focused on the
-problems surrounding agent/tool integration, such as observability and access
-control.
-
-More likely, you would use LangChain and other libraries for defining agent
-behavior and rely on `agency` to provide the connective layer for bringing
-agents and other systems together.
-
-So in comparison, `agency` is a smaller but more general purpose application
-framework compared to libraries like LangChain that focus on enabling individual
-agent behavior.
+`agency` is focused on the problems surrounding agent/tool/human integration,
+such as communication, observability, and access control. The library strives to
+provide a minimal yet practical foundation for defining and integrating agent
+systems, allowing developers the freedom to experiment with different agent
+solutions as they desire.
+
+More likely, you would use LangChain or other libraries for defining agent
+specific behavior and rely on `agency` to provide the connective layer for
+bringing agents and other systems together.
 
 
 ## What are some known limitations or issues?
 
 * It's a new project, so keep that in mind in terms of
   completeness, but see [the issues
   page](https://github.com/operand/agency/issues) for what is currently planned,
```

### Comparing `agency-1.1.0/agency/agent.py` & `agency-1.1.1/agency/agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.1.0/agency/schema.py` & `agency-1.1.1/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.1.0/agency/space.py` & `agency-1.1.1/agency/space.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC, ABCMeta, abstractmethod
-from agency import util
 from agency.agent import Agent
 from agency.schema import MessageSchema
 from typing import List
 import json
 import os
 import pika
 import queue
@@ -51,16 +50,18 @@
         self.agents.append(agent)
         # add a thread to process messages
 
         def _consume_messages():
             # create queue for agent
             agent._queue = queue.Queue()
             agent._space = self
+            agent._connected = threading.Event()
+            agent._connected.set()
             agent._after_add()
-            while True:
+            while agent._connected.is_set():
                 try:
                     message_dict = agent._queue.get(block=False)
                     message = MessageSchema(
                         **message_dict).dict(by_alias=True)  # validate
                     if 'to' not in message or message['to'] in [None, ""] or message['to'] == agent.id():
                         agent._receive(message)
                 except queue.Empty:
@@ -68,14 +69,15 @@
                 time.sleep(0.01)  # cooperate
 
         threading.Thread(target=_consume_messages).start()
         time.sleep(0.01)  # cooperate
 
     def remove(self, agent: Agent):
         agent._before_remove()
+        agent._connected.clear()
         self.agents.remove(agent)
         agent._space = None
 
     def _route(self, sender: Agent, action: dict) -> None:
         # Define and validate message
         message = MessageSchema(**{
           **action,
```

### Comparing `agency-1.1.0/agency/util.py` & `agency-1.1.1/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.1.0/pyproject.toml` & `agency-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "agency"
-version = "1.1.0"
+version = "1.1.1"
 description = "A fast and minimal actor model framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["agency/**/*"]
 exclude = ["*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncio = "^3.4"
 colorama = "^0.4"
 pydantic = "^1.8"
-eventlet = "^0.33.3"
 pika = "^1.3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
```

### Comparing `agency-1.1.0/PKG-INFO` & `agency-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 Metadata-Version: 2.1
 Name: agency
-Version: 1.1.0
+Version: 1.1.1
 Summary: A fast and minimal actor model framework for building agent-integrated systems
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4,<4.0)
 Requires-Dist: colorama (>=0.4,<0.5)
-Requires-Dist: eventlet (>=0.33.3,<0.34.0)
 Requires-Dist: pika (>=1.3.2,<2.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Description-Content-Type: text/markdown
 
 # Summary
 
-`agency` defines a common communication and action framework for creating AI
-agent integrated applications.
+`agency` is a python library that provides a communication and action framework
+for creating AI agent integrated applications.
 
 The library provides a low-level means for connecting agents, systems, and human
 users by defining actions, callbacks, and access policies that you can use to
-monitor, control, and interact with your agents.
+connect, monitor, control, and interact with your agents.
 
 `agency` handles the details of the common messaging system and allows
 discovering and invoking actions across parties, automatically handling things
 such as reporting exceptions, enforcing access restrictions, and more.
 
-`agency`'s purpose is to support agent development and integration by allowing
-you to create dynamic environments for your agents to freely work in a safe and
-controllable way, and to leave all other details up to you.
-
-Set your agents free (or just as much as you want) with `agency`!
-
 
 ## Features
 
 ### Low-Level API Flexibility
   * Straightforward class/method based agent and action definition
   * Supports defining single process applications or networked agent systems
   using AMQP
 
 ### Observability and Control
-  * Before/After action callbacks for observability or other needs
+  * Before/after action and lifecycle callbacks for observability or other needs
   * Access policies and permission callbacks for access control
 
 ### Performance
   * Multithreaded (though python's GIL is a bottleneck for single process apps)
   * AMQP support for multiprocess and networked systems (avoids GIL)
   * [_Python multiprocess support is planned for better scalability on
     single-host systems_](https://github.com/operand/agency/issues/33)
@@ -57,15 +50,15 @@
 ### Multimodal (image/audio) support
   * [_Not yet developed, but is planned_](https://github.com/operand/agency/issues/27)
 
 ### Full demo available at [`examples/demo`](./examples/demo/)
   * Two OpenAI agent examples
   * HuggingFace transformers agent example
   * Simple Flask/React web interface included
-  * Direct host access for agents
+  * Operating system access for agents
   * Docker configuration for reference and development
 
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
@@ -105,31 +98,37 @@
 
 ```python
   @access_policy(ACCESS_PERMITTED) # This allows the action at any time
   def _action__add(a, b):
     ...
 ```
 
-You can also define before/after and permission callbacks for various purposes:
+You can also define callbacks for various purposes:
 
 ```python
 class CalculatorAgent(Agent):
   ...
   def _before_action(self, original_message: dict):
     # Called before any action is attempted
 
   def _after_action(self, original_message: dict, return_value: str, error: str):
     # Called after any action is attempted
 
+  def _after_add(self):
+    # Called after the agent is added to the space and may begin communicating
+
+  def _before_remove(self):
+    # Called before the agent is removed from the space
+
   def _request_permission(self, proposed_message: dict) -> bool:
     # Called before an ACCESS_REQUESTED action is attempted for run-time review
 ```
 
 A `Space` is how you connect your agents together. An agent cannot communicate
-with others until it is added to a common "space".
+with others until it is added to a common `Space`.
 
 There are two included `Space` implementations to choose from:
 * `NativeSpace` - which connects agents within the same python process
 * `AMQPSpace` - which connects agents across processes and systems using an AMQP
   server like RabbitMQ.
 
 Here is an example of creating a `NativeSpace` and adding two agents to it.
@@ -155,20 +154,19 @@
 poetry add agency
 ```
 
 
 # Running the Demo Application
 
 To run the demo, please follow the directions at
-[examples/demo](./examples/demo/).
+[examples/demo](./examples/demo/). After a short boot time you can visit the
+web app at `http://localhost:8080` and you should see a simple chat interface.
 
-After a short boot time you can visit the web app at `http://localhost:8080` and
-you should see a simple chat interface. The following is a screenshot of a
-conversation that demonstrates multiple agents intelligently interacting and
-following orders.
+The following is a screenshot of the web UI that demonstrates the multiple demo
+agents intelligently interacting and following orders.
 
 There are two OpenAI based agents: `"FunctionAI"` and `"CompletionAI"`, named
 for the API's they use, and `"Chatty"` a simple chat agent who uses a small
 local transformers based model for demonstration.
 
 The screenshot also demonstrates the results of rejecting an action and
 directing an agent to use a different approach in real time. After I explained
@@ -184,28 +182,25 @@
 
 # FAQ
 
 ## How does `agency` compare to agent libraries like LangChain?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be a full-fledged agent toolset.
+intended to be a full-fledged agent toolset like other libraries or tools.
 
-Projects like LangChain and others are exploring how to create purpose-built
-agents that solve diverse problems using tools. `agency` is focused on the
-problems surrounding agent/tool integration, such as observability and access
-control.
-
-More likely, you would use LangChain and other libraries for defining agent
-behavior and rely on `agency` to provide the connective layer for bringing
-agents and other systems together.
-
-So in comparison, `agency` is a smaller but more general purpose application
-framework compared to libraries like LangChain that focus on enabling individual
-agent behavior.
+`agency` is focused on the problems surrounding agent/tool/human integration,
+such as communication, observability, and access control. The library strives to
+provide a minimal yet practical foundation for defining and integrating agent
+systems, allowing developers the freedom to experiment with different agent
+solutions as they desire.
+
+More likely, you would use LangChain or other libraries for defining agent
+specific behavior and rely on `agency` to provide the connective layer for
+bringing agents and other systems together.
 
 
 ## What are some known limitations or issues?
 
 * It's a new project, so keep that in mind in terms of
   completeness, but see [the issues
   page](https://github.com/operand/agency/issues) for what is currently planned,
```

