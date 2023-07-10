# Comparing `tmp/llmreflect-0.0.5.tar.gz` & `tmp/llmreflect-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.0.5.tar", max compression
+gzip compressed data, was "llmreflect-0.0.6.tar", max compression
```

## Comparing `llmreflect-0.0.5.tar` & `llmreflect-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4061 2023-07-10 18:42:44.696518 llmreflect-0.0.5/README.md
--rw-r--r--   0        0        0     3647 2023-07-10 18:42:44.696518 llmreflect-0.0.5/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     2377 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3059 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     9597 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/PostgresqlAgent.py
--rw-r--r--   0        0        0     2284 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     1873 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0    21665 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0     1786 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/ModerateChain.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8378 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     2366 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/moderatepostgresql.json
--rw-r--r--   0        0        0     4951 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresql.json
--rw-r--r--   0        0        0     1119 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresqlfix.json
--rw-r--r--   0        0        0     2011 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0     1933 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4219 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0     7686 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      442 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Utils/database.py
--rw-r--r--   0        0        0      305 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Utils/message.py
--rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/__init__.py
--rw-r--r--   0        0        0      478 2023-07-10 18:42:44.700518 llmreflect-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-07-10 23:04:49.790592 llmreflect-0.0.6/README.md
+-rw-r--r--   0        0        0     3647 2023-07-10 23:04:49.790592 llmreflect-0.0.6/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     2590 2023-07-10 23:04:49.790592 llmreflect-0.0.6/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3038 2023-07-10 23:04:49.790592 llmreflect-0.0.6/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     9650 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Agents/PostgresqlAgent.py
+-rw-r--r--   0        0        0     2308 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     2392 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    21685 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     1786 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8299 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/gradingpostgresql.json
+-rw-r--r--   0        0        0     2366 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/moderatepostgresql.json
+-rw-r--r--   0        0        0     4951 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresql.json
+-rw-r--r--   0        0        0     1119 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresqlfix.json
+-rw-r--r--   0        0        0     2084 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/questionpostgresql.json
+-rw-r--r--   0        0        0     1941 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     4219 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0     7579 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      442 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      690 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0     1019 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Utils/log.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-10 23:04:49.794592 llmreflect-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.6/PKG-INFO
```

### Comparing `llmreflect-0.0.5/README.md` & `llmreflect-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Agents/BasicAgent.py` & `llmreflect-0.0.6/llmreflect/Agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.0.6/llmreflect/Agents/EvaluationAgent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
 
 
 class PostgressqlGradingAgent(OpenAIAgent):
     """
     This is the agent class use for grading postgresql generation.
     Args:
@@ -41,18 +41,23 @@
             sql_cmd (str): sql command generated from LLM
             db_summary (str): a brief report for the query summarized by
             retriever.
 
         Returns:
             a dictionary, {'grading': grading, 'explanation': explanation}
         """
-        result = "Failed, no output from LLM."
+        result = {'grading': 0, 'explanation': "Failed, no output from LLM."}
         if self.retriever is None:
-            message("Error: Retriever is not equipped.", color="red")
+            LOGGER.error("Error: Retriever is not equipped.")
         else:
-            llm_output = self.predict(
-                request=request,
-                command=sql_cmd,
-                summary=db_summary
-            )
-            result = self.retriever.retrieve(llm_output)
+            try:
+                llm_output = self.predict(
+                    request=request,
+                    command=sql_cmd,
+                    summary=db_summary
+                )
+                LOGGER.debug(llm_output)
+                result = self.retriever.retrieve(llm_output)
+            except Exception as e:
+                LOGGER.error(str(e))
+                LOGGER.error(llm_output)
         return result
```

### Comparing `llmreflect-0.0.5/llmreflect/Agents/ModerateAgent.py` & `llmreflect-0.0.6/llmreflect/Agents/ModerateAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.BasicRetriever import \
     BasicQuestionModerateRetriever
 
 
 class PostgresqlModerateAgent(OpenAIAgent):
     """
     Agent for filtering out illegal and malicious requests.
@@ -43,15 +43,15 @@
             user_input (str): _description_
 
         Returns:
             bool: boolean answer, true or false
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
-            message("Error: Retriever is not equipped.", color="red")
+            LOGGER.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 topic="patient data",
                 included_tables=self.retriever.include_tables,
                 request=user_input
             )
             result = self.retriever.retrieve(llm_output)['decision']
@@ -64,15 +64,15 @@
             user_input (str): _description_
 
         Returns:
             dict: {'decision': bool, 'explanation': str}
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
-            message("Error: Retriever is not equipped.", color="red")
+            LOGGER.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 topic="patient data",
                 included_tables=self.retriever.include_tables,
                 request=user_input
             )
             result = self.retriever.retrieve(llm_output,
```

### Comparing `llmreflect-0.0.5/llmreflect/Agents/PostgresqlAgent.py` & `llmreflect-0.0.6/llmreflect/Agents/PostgresqlAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.DatabaseRetriever import DatabaseRetriever
 from typing import Any
 
 
 class PostgresqlAgent(OpenAIAgent):
     """
     Agent class for executing postgresql command
@@ -49,22 +49,23 @@
             user_input (str): users description for the query.
 
         Returns:
             str: gross output of the llm attempt for generating sql cmd.
         """
         llm_output = "Failed, no output from LLM."
         if self.retriever is None:
-            message("Error: Retriever is not equipped.", color="red")
+            LOGGER.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 dialect=self.retriever.database_dialect,
                 max_present=self.retriever.max_rows_return,
                 table_info=self.retriever.table_info,
                 request=user_input
             )
+            LOGGER.debug(llm_output)
         return llm_output
 
     def predict_db(self, user_input: str,
                    get_cmd: bool = False,
                    get_summary: bool = False,
                    get_db: bool = False
                    ) -> str:
@@ -145,24 +146,25 @@
             history (str): history command used for query
             his_error (str): the errors raised from executing the history cmd
         Returns:
             str: gross output of the llm attempt for generating sql cmd.
         """
         llm_output = "Failed, no output from LLM."
         if self.retriever is None:
-            message("Error: Retriever is not equipped.", color="red")
+            LOGGER.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 dialect=self.retriever.database_dialect,
                 max_present=self.retriever.max_rows_return,
                 table_info=self.retriever.table_info,
                 request=user_input,
                 history=history,
                 his_error=his_error
             )
+            LOGGER.debug(llm_output)
         return llm_output
 
     def predict_db(self, user_input: str,
                    history: str,
                    his_error: str,
                    get_cmd: bool = False,
                    get_summary: bool = False,
```

### Comparing `llmreflect-0.0.5/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.0.6/llmreflect/Agents/QuestionAgent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever
 
 
 class PostgresqlQuestionAgent(OpenAIAgent):
     """
     Agent for creating questions based on a given database
     Args:
@@ -43,15 +43,16 @@
             number of questions to generate in a run. Defaults to 5.
 
         Returns:
             str: a list of questions, I love list.
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
-            message("Error: Retriever is not equipped.", color="red")
+            LOGGER.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 table_info=self.retriever.table_info,
                 n_questions=n_questions
             )
+            LOGGER.debug(llm_output)
             result = self.retriever.retrieve(llm_output)
         return result
```

### Comparing `llmreflect-0.0.5/llmreflect/Chains/BasicChain.py` & `llmreflect-0.0.6/llmreflect/Chains/BasicChain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractclassmethod
 from llmreflect.Retriever.BasicRetriever import BasicRetriever
 from llmreflect.Agents.BasicAgent import Agent
 from llmreflect.Prompt.BasicPrompt import BasicPrompt
 from typing import Any, List
 from langchain.llms.openai import OpenAI
+from langchain.callbacks import get_openai_callback
+from llmreflect.Utils.log import LOGGER, openai_cb_2_str
 
 
 class BasicChain(ABC):
     '''
     Abstract class for Chain class.
     A chain class should be the atomic unit for completing a job.
     A chain contains at least two components:
@@ -32,14 +34,20 @@
         return cls(agent=agent, retriever=retriever)
 
     @abstractclassmethod
     def perform(self, **kwargs: Any):
         result = self.agent.predict(kwargs)
         return result
 
+    def perform_cost_monitor(self, **kwargs: Any):
+        with get_openai_callback() as cb:
+            result = self.perform(**kwargs)
+        LOGGER.info(openai_cb_2_str(cb))
+        return result, cb
+
 
 class BasicCombinedChain(ABC):
     '''
     Abstract class for combined Chain class.
     A combined chain is a chain with multiple chains
     A chain class should be the atomic unit for completing a job.
     A chain object must have the function to perform a job.
@@ -50,7 +58,13 @@
     @abstractclassmethod
     def from_config(cls, **kwargs: Any):
         return
 
     @abstractclassmethod
     def perform(self, **kwargs: Any):
         return
+
+    def perform_cost_monitor(self, **kwargs: Any):
+        with get_openai_callback() as cb:
+            result = self.perform(**kwargs)
+        LOGGER.info(openai_cb_2_str(cb))
+        return result, cb
```

### Comparing `llmreflect-0.0.5/llmreflect/Chains/DatabaseChain.py` & `llmreflect-0.0.6/llmreflect/Chains/DatabaseChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     PostgresqlSelfFixAgent
 from llmreflect.Agents.EvaluationAgent import PostgressqlGradingAgent
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever, \
     DatabaseRetriever
 from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
 from llmreflect.Chains.ModerateChain import ModerateChain
 from typing import List
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 
 
 class DatabaseQuestionChain(BasicChain):
     def __init__(self, agent: PostgresqlQuestionAgent,
                  retriever: DatabaseQuestionRetriever):
         """
         A chain for creating questions given by a dataset.
@@ -380,17 +380,17 @@
             db_result = answer_dict['db']
         fix_attempt = 0
 
         error_logs = []
 
         while 'error' in summary.lower() and fix_attempt < self.fix_patience:
             if log_fix:
-                message(f"Error: {summary}", 'red')
-                message(f"Self-fix Attempt: {fix_attempt}", 'yellow')
-                message("Self-fixing...", 'yellow')
+                LOGGER.warning(f"Error detected: {summary}")
+                LOGGER.warning(f"Self-fix Attempt: {fix_attempt}")
+                LOGGER.warning("Self-fixing...")
                 error_logs.append({
                     'cmd': sql_cmd,
                     'error': summary})
             fixed_answer_dict = self.fix_chain.perform(
                 user_input=user_input,
                 history=sql_cmd,
                 his_error=summary,
@@ -400,19 +400,19 @@
             )
             sql_cmd = fixed_answer_dict['cmd']
             summary = fixed_answer_dict['summary']
             if get_db:
                 db_result = fixed_answer_dict['db']
 
             if 'error' not in summary.lower() and log_fix:
-                message("Self-fix finished.", 'green')
+                LOGGER.info("Self-fix finished.")
             fix_attempt += 1
 
         if 'error' in summary.lower() and log_fix:
-            message("Self-fix failed.", 'red')
+            LOGGER.error("Self-fix failed!")
 
         if not get_cmd:
             sql_cmd = ""
         if not get_summary:
             get_summary = ""
 
         return {'cmd': sql_cmd,
@@ -584,15 +584,16 @@
                            }
             return return_dict
 
         answer_dict = self.a_n_f_chain.perform(
             user_input=user_input,
             get_cmd=True,
             get_db=get_db,
-            get_summary=True
+            get_summary=True,
+            log_fix=log_fix
         )
 
         return {'cmd': answer_dict['cmd'],
                 'summary': answer_dict['summary'],
                 'db': answer_dict['db'],
                 'error': answer_dict['error'],
                 'moderate_decision': moderate_decision,
```

### Comparing `llmreflect-0.0.5/llmreflect/Chains/ModerateChain.py` & `llmreflect-0.0.6/llmreflect/Chains/ModerateChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.0.6/llmreflect/Prompt/BasicPrompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 2. Soft rule which can be modified by Agents only when necessary.
 3. In-context learning, places for holding in-context learning examples,
 the major part that Agents can tune.
 """
 from typing import Dict, Any
 from langchain.prompts.prompt import PromptTemplate
 import os
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 import json
 import re
 
 PROMPT_BASE_DIR = os.path.join(os.path.dirname(__file__), 'promptbase')
 INPUT_KEY_TYPE_CHOICE = ['INPUT', 'OUTPUT', 'CONTEXT']
 
 
@@ -116,16 +116,15 @@
 
     def get_langchain_prompt_template(self):
         return self.prompt_template
 
     @classmethod
     def load_prompt_from_json_file(cls, promptname: str):
         js = cls._load_json_file(promptname=promptname)
-        message(msg=f"{promptname} prompt loaded successfully!",
-                color="green")
+        LOGGER.info(f"{promptname} prompt loaded successfully!")
 
         return cls(prompt_dict=js, promptname=promptname)
 
     @classmethod
     def _load_json_file(cls, promptname: str):
         prompt_dir = os.path.join(PROMPT_BASE_DIR, promptname + '.json')
 
@@ -151,23 +150,22 @@
     def save_prompt(self):
         """
         save prompt into json file.
         """
         try:
             self.__valid_prompt_dict(self.prompt_dict)
         except Exception:
-            message(msg="Prompt dictionary format is illegal!", color="red")
+            LOGGER.error("Prompt dictionary format is illegal!")
             return
 
         saving_dir = os.path.join(PROMPT_BASE_DIR, f"{self.promptname}.json")
         with open(saving_dir, 'w') as writefile:
             json.dump(self.prompt_dict, writefile)
 
-        message(msg=f"{self.promptname} has been dumped into {saving_dir}",
-                color="green")
+        LOGGER.info(f"{self.promptname} has been dumped into {saving_dir}")
 
     @classmethod
     def wrap_key_name(cls, key_name):
         return "[" + key_name + "]"
 
     @property
     def hard_rules(self):
```

### Comparing `llmreflect-0.0.5/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.0.6/llmreflect/Prompt/promptbase/gradingpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Prompt/promptbase/moderatepostgresql.json` & `llmreflect-0.0.6/llmreflect/Prompt/promptbase/moderatepostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresql.json` & `llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresqlfix.json` & `llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresqlfix.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.0.6/llmreflect/Prompt/promptbase/questionpostgresql.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'FORMAT'": "{'questions': {'explanation': '\\n[1.] the first question created by you. \\n[2.] "*

 * *             "the second question \\n... \\n[n.] the nth question'}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "FORMAT": {
         "n_questions": {
             "explanation": "number of questions requested",
             "type": "INPUT"
         },
         "questions": {
-            "explanation": "the questions you created",
+            "explanation": "\n[1.] the first question created by you. \n[2.] the second question \n... \n[n.] the nth question",
             "type": "OUTPUT"
         }
     },
     "HARD": "You are a smart assistant designed to help with testing a postgresql AI.\nGiven by information about a database, you must come up with questions in natural language. There are two things that you want to exam. First,it is the comprehensive ability that how well the AI understands the question.Second, it is the postgresql query ability that how well the AI designs complicated queries. Therefore, you must phrase your questions in diverse ways and the questions require sophisticated logic to be solved.\n\nThe information about the database is:\n{table_info}\n",
     "INCONTEXT": [
         {
             "n_questions": "2",
```

### Comparing `llmreflect-0.0.5/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.0.6/llmreflect/Retriever/BasicRetriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         return llm_output.strip('\n').strip(' ')
 
 
 class BasicEvaluationRetriever(BasicRetriever):
     # Class for general postprocessing llm output string
     def retrieve(self, llm_output: str) -> dict:
         llm_output = llm_output.strip('\n').strip(' ')
-        grading = float(llm_output.split("\n")[0].split(']')[-1])
+        grading = float(llm_output.split("\n")[0].split('[grading]')[-1])
         explanation = llm_output.split(']')[-1]
         return {'grading': grading, 'explanation': explanation}
 
 
 class BasicQuestionModerateRetriever(BasicRetriever):
     """_summary_
     Retriever class based on DatabaseQuestionRetriever.
```

### Comparing `llmreflect-0.0.5/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.0.6/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/llmreflect/Tests/test_chains.py` & `llmreflect-0.0.6/llmreflect/Tests/test_chains.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Have not figured out a way to test current chains without database.
 Future work...
 """
 import os
 import pytest
-from llmreflect.Utils.message import message
+from llmreflect.Utils.log import LOGGER
 
 
 def in_workflow():
     return os.getenv("GITHUB_ACTIONS")\
         or os.getenv("TRAVIS") \
         or os.getenv("CIRCLECI") \
         or os.getenv("GITLAB_CI")
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_moderate_answer_fix_chain():
+
     from llmreflect.Chains.DatabaseChain import \
         DatabaseModerateNAnswerNFixChain
     from decouple import config
 
     uri = f"postgresql+psycopg2://{config('DBUSERNAME')}:\
 {config('DBPASSWORD')}@{config('DBHOST')}:{config('DBPORT')}/postgres"
 
@@ -32,24 +33,26 @@
             'tb_patients_allergies',
             'tb_appointment_patients',
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         open_ai_key=config('OPENAI_API_KEY')
     )
-    result = ch.perform(user_input="give me a list of patients",
-                        explain_moderate=True)
-    print(result)
+
+    result, _ = ch.perform_cost_monitor(
+        user_input="give me a list of patients",
+        explain_moderate=True)
+
     assert result['moderate_decision']
 
-    result = ch.perform(user_input="Cats are the true rulers",
-                        explain_moderate=True)
+    result, _ = ch.perform_cost_monitor(
+        user_input="Cats are the true rulers",
+        explain_moderate=True)
     assert not result['moderate_decision']
     assert len(result['moderate_explanation']) > 0
-    print(result)
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_moderate_chain():
     from llmreflect.Chains.ModerateChain import ModerateChain
@@ -60,20 +63,22 @@
             'tb_patient',
             'tb_patients_allergies',
             'tb_appointment_patients',
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ]
     )
-    result = ch.perform(user_input="give me a list of patients",
-                        with_explanation=True)
+    result, _ = ch.perform_cost_monitor(
+        user_input="give me a list of patients",
+        with_explanation=True)
     assert result['decision']
 
-    result = ch.perform(user_input="Cats are the true rulers",
-                        with_explanation=True)
+    result, _ = ch.perform_cost_monitor(
+        user_input="Cats are the true rulers",
+        with_explanation=True)
     assert not result['decision']
     assert len(result['explanation']) > 0
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
@@ -97,31 +102,30 @@
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         a_max_output_tokens=512,
         g_max_output_tokens=256,
         open_ai_key=config('OPENAI_API_KEY')
     )
-    logs = ch.perform(n_question=N_QUESTIONS)
+    logs, _ = ch.perform_cost_monitor(n_question=N_QUESTIONS)
     if SAVE_LOG:
         df = pd.DataFrame.from_records(logs)
         df.to_csv("self_grading.csv")
     else:
         for log in logs:
-            message("Question: " + log["question"], 'blue')
-            message("Query: " + log["cmd"], 'yellow')
-            message("Summary: " + log["summary"], "green")
-            message("Score: %.2f" % log["grading"], 'yellow')
-            message("Explain: " + log["explanation"], "green")
+            LOGGER.info("Question: " + log["question"])
+            LOGGER.info("Query: " + log["cmd"])
+            LOGGER.info("Summary: " + log["summary"])
+            LOGGER.info("Score: %.2f" % log["grading"])
+            LOGGER.info("Explain: " + log["explanation"])
             assert len(log["question"]) > 0
             assert len(log["cmd"]) > 0
             assert len(log["summary"]) > 0
             assert len(log["explanation"]) > 0
-            assert log["grading"] > 0
-            print("=========================\n\n")
+            assert log["grading"] >= 0
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_self_fix_chain():
     from llmreflect.Chains.DatabaseChain import DatabaseQuestionChain,\
@@ -168,37 +172,36 @@
         prompt_name="postgresqlfix",
         max_output_tokens=max_output_tokens,
         temperature=0.1,
         sample_rows=0,
         max_rows_return=500
     )
 
-    questions = q_ch.perform(n_questions=5)
+    questions, _ = q_ch.perform_cost_monitor(n_questions=5)
     for q in questions:
-        cmd_summary = a_ch.perform(user_input=q)
+        cmd_summary, _ = a_ch.perform_cost_monitor(user_input=q)
         cmd = cmd_summary['cmd']
         summary = cmd_summary['summary']
         if "Error" not in summary:
             crooked_cmd = cmd.replace("tb_", "")
             crooked_summary = a_ch.retriever.retrieve_summary(
                 llm_output=crooked_cmd)
-            message("Question: " + q, color='blue')
-            message("Crooked command: " + crooked_cmd, color='yellow')
-            message("Crooked summary: " + crooked_summary, color='red')
-            result_dict = self_fix_ch.perform(
+            LOGGER.info("Question: " + q)
+            LOGGER.info("Crooked command: " + crooked_cmd)
+            LOGGER.info("Crooked summary: " + crooked_summary)
+            result_dict, _ = self_fix_ch.perform_cost_monitor(
                 user_input=q,
                 history=crooked_cmd,
                 his_error=crooked_summary
             )
             fixed_cmd = result_dict['cmd']
             fixed_summary = result_dict['summary']
-            message("Fixed command: " + fixed_cmd, color='yellow')
-            message("Fixed summary: " + fixed_summary, color='green')
+            LOGGER.info("Fixed command: " + fixed_cmd)
+            LOGGER.info("Fixed summary: " + fixed_summary)
             assert "error" not in fixed_summary.lower()
-            print("======================================\n\n")
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_answerNfix_chain():
 
@@ -216,10 +219,11 @@
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         open_ai_key=config('OPENAI_API_KEY'),
         answer_chain_prompt_name="postgresql",
         fix_chain_prompt_name="postgresqlfix"
     )
-    result_dict = ch.perform(user_input="give me a list overweight patients")
+    result_dict, _ = ch.perform_cost_monitor(
+        user_input="give me a list overweight patients")
     assert len(result_dict['summary']) > 0
     assert type(result_dict['error']) is list
```

### Comparing `llmreflect-0.0.5/llmreflect/Utils/database.py` & `llmreflect-0.0.6/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.5/PKG-INFO` & `llmreflect-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.0.5
+Version: 0.0.6
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

