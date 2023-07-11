# Comparing `tmp/llmreflect-0.0.6.tar.gz` & `tmp/llmreflect-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.0.6.tar", max compression
+gzip compressed data, was "llmreflect-0.0.7.tar", max compression
```

## Comparing `llmreflect-0.0.6.tar` & `llmreflect-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4061 2023-07-10 23:04:49.790592 llmreflect-0.0.6/README.md
--rw-r--r--   0        0        0     3647 2023-07-10 23:04:49.790592 llmreflect-0.0.6/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     2590 2023-07-10 23:04:49.790592 llmreflect-0.0.6/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3038 2023-07-10 23:04:49.790592 llmreflect-0.0.6/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     9650 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Agents/PostgresqlAgent.py
--rw-r--r--   0        0        0     2308 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     2392 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0    21685 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0     1786 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/ModerateChain.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8299 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     2366 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/moderatepostgresql.json
--rw-r--r--   0        0        0     4951 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresql.json
--rw-r--r--   0        0        0     1119 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresqlfix.json
--rw-r--r--   0        0        0     2084 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0     1941 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4219 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0     7579 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      442 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Utils/database.py
--rw-r--r--   0        0        0     1019 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/Utils/log.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:49.794592 llmreflect-0.0.6/llmreflect/__init__.py
--rw-r--r--   0        0        0      478 2023-07-10 23:04:49.794592 llmreflect-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-07-11 18:08:29.939687 llmreflect-0.0.7/README.md
+-rw-r--r--   0        0        0     3771 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     2570 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3092 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     9630 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/PostgresqlAgent.py
+-rw-r--r--   0        0        0     2278 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     2522 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    21670 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     1786 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8381 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/gradingpostgresql.json
+-rw-r--r--   0        0        0     2366 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/moderatepostgresql.json
+-rw-r--r--   0        0        0     4951 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresql.json
+-rw-r--r--   0        0        0     1119 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresqlfix.json
+-rw-r--r--   0        0        0     2084 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/questionpostgresql.json
+-rw-r--r--   0        0        0     1941 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     4219 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0     7612 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      442 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      690 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0     5685 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Utils/log.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-11 18:08:29.939687 llmreflect-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.7/PKG-INFO
```

### Comparing `llmreflect-0.0.6/README.md` & `llmreflect-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Agents/BasicAgent.py` & `llmreflect-0.0.7/llmreflect/Agents/BasicAgent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from langchain.chains import LLMChain
 from llmreflect.Prompt.BasicPrompt import BasicPrompt
 from langchain.base_language import BaseLanguageModel
 from abc import ABC, abstractclassmethod
 from llmreflect.Retriever.BasicRetriever import BasicRetriever
 from dataclasses import dataclass
 from langchain.chat_models import ChatOpenAI
+from llmreflect.Utils.log import get_logger
 
 
 @dataclass
 class LLM_BACKBONE_MODEL:
     gpt_4 = "gpt-4"
     gpt_4_0314 = "gpt-4-0314"
     gpt_4_0613 = "gpt-4-0613"
@@ -45,14 +46,15 @@
     execute the command in the database.
     '''
     def __init__(self, prompt: BasicPrompt, llm: BaseLanguageModel):
         super().__init__(prompt=prompt.get_langchain_prompt_template(),
                          llm=llm)
         # Agent class inherit from the LLM chain class
         object.__setattr__(self, 'retriever', None)
+        object.__setattr__(self, "logger", get_logger(self.__class__.__name__))
 
     @abstractclassmethod
     def equip_retriever(self, retriever: BasicRetriever):
         object.__setattr__(self, 'retriever', retriever)
 
     def get_inputs(self):
         """_summary_
```

### Comparing `llmreflect-0.0.6/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.0.7/llmreflect/Agents/EvaluationAgent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
 
 
 class PostgressqlGradingAgent(OpenAIAgent):
     """
     This is the agent class use for grading postgresql generation.
     Args:
@@ -43,21 +42,21 @@
             retriever.
 
         Returns:
             a dictionary, {'grading': grading, 'explanation': explanation}
         """
         result = {'grading': 0, 'explanation': "Failed, no output from LLM."}
         if self.retriever is None:
-            LOGGER.error("Error: Retriever is not equipped.")
+            self.logger.error("Error: Retriever is not equipped.")
         else:
             try:
                 llm_output = self.predict(
                     request=request,
                     command=sql_cmd,
                     summary=db_summary
                 )
-                LOGGER.debug(llm_output)
+                self.logger.debug(llm_output)
                 result = self.retriever.retrieve(llm_output)
             except Exception as e:
-                LOGGER.error(str(e))
-                LOGGER.error(llm_output)
+                self.logger.error(str(e))
+                self.logger.error(llm_output)
         return result
```

### Comparing `llmreflect-0.0.6/llmreflect/Agents/ModerateAgent.py` & `llmreflect-0.0.7/llmreflect/Agents/ModerateAgent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.BasicRetriever import \
     BasicQuestionModerateRetriever
 
 
 class PostgresqlModerateAgent(OpenAIAgent):
     """
     Agent for filtering out illegal and malicious requests.
@@ -43,38 +42,40 @@
             user_input (str): _description_
 
         Returns:
             bool: boolean answer, true or false
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
-            LOGGER.error("Error: Retriever is not equipped.")
+            self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 topic="patient data",
                 included_tables=self.retriever.include_tables,
                 request=user_input
             )
+            self.logger.debug(llm_output)
             result = self.retriever.retrieve(llm_output)['decision']
         return result
 
     def predict_decision_explained(self, user_input: str) -> dict:
         """
         predict judgement with explanation
         Args:
             user_input (str): _description_
 
         Returns:
             dict: {'decision': bool, 'explanation': str}
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
-            LOGGER.error("Error: Retriever is not equipped.")
+            self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 topic="patient data",
                 included_tables=self.retriever.include_tables,
                 request=user_input
             )
+            self.logger.debug(llm_output)
             result = self.retriever.retrieve(llm_output,
                                              explanation=True)
         return result
```

### Comparing `llmreflect-0.0.6/llmreflect/Agents/PostgresqlAgent.py` & `llmreflect-0.0.7/llmreflect/Agents/PostgresqlAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.DatabaseRetriever import DatabaseRetriever
 from typing import Any
 
 
 class PostgresqlAgent(OpenAIAgent):
     """
     Agent class for executing postgresql command
@@ -49,23 +48,23 @@
             user_input (str): users description for the query.
 
         Returns:
             str: gross output of the llm attempt for generating sql cmd.
         """
         llm_output = "Failed, no output from LLM."
         if self.retriever is None:
-            LOGGER.error("Error: Retriever is not equipped.")
+            self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 dialect=self.retriever.database_dialect,
                 max_present=self.retriever.max_rows_return,
                 table_info=self.retriever.table_info,
                 request=user_input
             )
-            LOGGER.debug(llm_output)
+            self.logger.debug(llm_output)
         return llm_output
 
     def predict_db(self, user_input: str,
                    get_cmd: bool = False,
                    get_summary: bool = False,
                    get_db: bool = False
                    ) -> str:
@@ -146,25 +145,25 @@
             history (str): history command used for query
             his_error (str): the errors raised from executing the history cmd
         Returns:
             str: gross output of the llm attempt for generating sql cmd.
         """
         llm_output = "Failed, no output from LLM."
         if self.retriever is None:
-            LOGGER.error("Error: Retriever is not equipped.")
+            self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 dialect=self.retriever.database_dialect,
                 max_present=self.retriever.max_rows_return,
                 table_info=self.retriever.table_info,
                 request=user_input,
                 history=history,
                 his_error=his_error
             )
-            LOGGER.debug(llm_output)
+            self.logger.debug(llm_output)
         return llm_output
 
     def predict_db(self, user_input: str,
                    history: str,
                    his_error: str,
                    get_cmd: bool = False,
                    get_summary: bool = False,
```

### Comparing `llmreflect-0.0.6/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.0.7/llmreflect/Agents/QuestionAgent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Utils.log import LOGGER
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever
 
 
 class PostgresqlQuestionAgent(OpenAIAgent):
     """
     Agent for creating questions based on a given database
     Args:
@@ -43,16 +42,16 @@
             number of questions to generate in a run. Defaults to 5.
 
         Returns:
             str: a list of questions, I love list.
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
-            LOGGER.error("Error: Retriever is not equipped.")
+            self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 table_info=self.retriever.table_info,
                 n_questions=n_questions
             )
-            LOGGER.debug(llm_output)
+            self.logger.debug(llm_output)
             result = self.retriever.retrieve(llm_output)
         return result
```

### Comparing `llmreflect-0.0.6/llmreflect/Chains/BasicChain.py` & `llmreflect-0.0.7/llmreflect/Chains/BasicChain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from abc import ABC, abstractclassmethod
 from llmreflect.Retriever.BasicRetriever import BasicRetriever
 from llmreflect.Agents.BasicAgent import Agent
 from llmreflect.Prompt.BasicPrompt import BasicPrompt
 from typing import Any, List
 from langchain.llms.openai import OpenAI
 from langchain.callbacks import get_openai_callback
-from llmreflect.Utils.log import LOGGER, openai_cb_2_str
+from llmreflect.Utils.log import get_logger, openai_cb_2_str
 
 
 class BasicChain(ABC):
     '''
     Abstract class for Chain class.
     A chain class should be the atomic unit for completing a job.
     A chain contains at least two components:
     1. an agent 2. a retriever
     A chain object must have the function to perform a job.
     '''
     def __init__(self, agent: Agent, retriever: BasicRetriever):
         self.agent = agent
         self.retriever = retriever
         self.agent.equip_retriever(self.retriever)
+        self.logger = get_logger(self.__class__.__name__)
 
     @abstractclassmethod
     def from_config(cls,
                     open_ai_key: str,
                     prompt_name: str = 'questionpostgresql',
                     temperature: float = 0.0):
         llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
@@ -37,34 +38,35 @@
     def perform(self, **kwargs: Any):
         result = self.agent.predict(kwargs)
         return result
 
     def perform_cost_monitor(self, **kwargs: Any):
         with get_openai_callback() as cb:
             result = self.perform(**kwargs)
-        LOGGER.info(openai_cb_2_str(cb))
+        self.logger.cost(openai_cb_2_str(cb))
         return result, cb
 
 
 class BasicCombinedChain(ABC):
     '''
     Abstract class for combined Chain class.
     A combined chain is a chain with multiple chains
     A chain class should be the atomic unit for completing a job.
     A chain object must have the function to perform a job.
     '''
     def __init__(self, chains: List[BasicChain]):
         self.chains = chains
+        self.logger = get_logger(self.__class__.__name__)
 
     @abstractclassmethod
     def from_config(cls, **kwargs: Any):
         return
 
     @abstractclassmethod
     def perform(self, **kwargs: Any):
         return
 
     def perform_cost_monitor(self, **kwargs: Any):
         with get_openai_callback() as cb:
             result = self.perform(**kwargs)
-        LOGGER.info(openai_cb_2_str(cb))
+        self.logger.cost(openai_cb_2_str(cb))
         return result, cb
```

### Comparing `llmreflect-0.0.6/llmreflect/Chains/DatabaseChain.py` & `llmreflect-0.0.7/llmreflect/Chains/DatabaseChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     PostgresqlSelfFixAgent
 from llmreflect.Agents.EvaluationAgent import PostgressqlGradingAgent
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever, \
     DatabaseRetriever
 from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
 from llmreflect.Chains.ModerateChain import ModerateChain
 from typing import List
-from llmreflect.Utils.log import LOGGER
 
 
 class DatabaseQuestionChain(BasicChain):
     def __init__(self, agent: PostgresqlQuestionAgent,
                  retriever: DatabaseQuestionRetriever):
         """
         A chain for creating questions given by a dataset.
@@ -380,17 +379,17 @@
             db_result = answer_dict['db']
         fix_attempt = 0
 
         error_logs = []
 
         while 'error' in summary.lower() and fix_attempt < self.fix_patience:
             if log_fix:
-                LOGGER.warning(f"Error detected: {summary}")
-                LOGGER.warning(f"Self-fix Attempt: {fix_attempt}")
-                LOGGER.warning("Self-fixing...")
+                self.logger.warning(f"Error detected: {summary}")
+                self.logger.warning(f"Self-fix Attempt: {fix_attempt}")
+                self.logger.warning("Self-fixing...")
                 error_logs.append({
                     'cmd': sql_cmd,
                     'error': summary})
             fixed_answer_dict = self.fix_chain.perform(
                 user_input=user_input,
                 history=sql_cmd,
                 his_error=summary,
@@ -400,19 +399,19 @@
             )
             sql_cmd = fixed_answer_dict['cmd']
             summary = fixed_answer_dict['summary']
             if get_db:
                 db_result = fixed_answer_dict['db']
 
             if 'error' not in summary.lower() and log_fix:
-                LOGGER.info("Self-fix finished.")
+                self.logger.info("Self-fix finished.")
             fix_attempt += 1
 
         if 'error' in summary.lower() and log_fix:
-            LOGGER.error("Self-fix failed!")
+            self.logger.error("Self-fix failed!")
 
         if not get_cmd:
             sql_cmd = ""
         if not get_summary:
             get_summary = ""
 
         return {'cmd': sql_cmd,
```

### Comparing `llmreflect-0.0.6/llmreflect/Chains/ModerateChain.py` & `llmreflect-0.0.7/llmreflect/Chains/ModerateChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.0.7/llmreflect/Prompt/BasicPrompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 2. Soft rule which can be modified by Agents only when necessary.
 3. In-context learning, places for holding in-context learning examples,
 the major part that Agents can tune.
 """
 from typing import Dict, Any
 from langchain.prompts.prompt import PromptTemplate
 import os
-from llmreflect.Utils.log import LOGGER
+from llmreflect.Utils.log import get_logger
 import json
 import re
 
 PROMPT_BASE_DIR = os.path.join(os.path.dirname(__file__), 'promptbase')
 INPUT_KEY_TYPE_CHOICE = ['INPUT', 'OUTPUT', 'CONTEXT']
 
 
-class BasicPrompt:
+class BasicPrompt(object):
     """
     Mighty mother of all prompts (In this repo I mean)
     """
+    logger = get_logger("Default Prompt")
+
     def __init__(self, prompt_dict: Dict[str, Any], promptname: str,
                  customized_input_list: list = []) -> None:
         """
         If you want to start working on a prompt from scratch,
         a dictionary containing the prompts and name of this prompt
         are required.
         Args:
@@ -116,15 +118,15 @@
 
     def get_langchain_prompt_template(self):
         return self.prompt_template
 
     @classmethod
     def load_prompt_from_json_file(cls, promptname: str):
         js = cls._load_json_file(promptname=promptname)
-        LOGGER.info(f"{promptname} prompt loaded successfully!")
+        cls.logger.info(f"{promptname} prompt loaded successfully!")
 
         return cls(prompt_dict=js, promptname=promptname)
 
     @classmethod
     def _load_json_file(cls, promptname: str):
         prompt_dir = os.path.join(PROMPT_BASE_DIR, promptname + '.json')
 
@@ -150,22 +152,23 @@
     def save_prompt(self):
         """
         save prompt into json file.
         """
         try:
             self.__valid_prompt_dict(self.prompt_dict)
         except Exception:
-            LOGGER.error("Prompt dictionary format is illegal!")
+            self.logger.error("Prompt dictionary format is illegal!")
             return
 
         saving_dir = os.path.join(PROMPT_BASE_DIR, f"{self.promptname}.json")
         with open(saving_dir, 'w') as writefile:
             json.dump(self.prompt_dict, writefile)
 
-        LOGGER.info(f"{self.promptname} has been dumped into {saving_dir}")
+        self.logger.info(
+            f"{self.promptname} has been dumped into {saving_dir}")
 
     @classmethod
     def wrap_key_name(cls, key_name):
         return "[" + key_name + "]"
 
     @property
     def hard_rules(self):
```

### Comparing `llmreflect-0.0.6/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.0.7/llmreflect/Prompt/promptbase/gradingpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Prompt/promptbase/moderatepostgresql.json` & `llmreflect-0.0.7/llmreflect/Prompt/promptbase/moderatepostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresql.json` & `llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Prompt/promptbase/postgresqlfix.json` & `llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresqlfix.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.0.7/llmreflect/Prompt/promptbase/questionpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.0.7/llmreflect/Retriever/BasicRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.0.7/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/llmreflect/Tests/test_chains.py` & `llmreflect-0.0.7/llmreflect/Tests/test_chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Have not figured out a way to test current chains without database.
 Future work...
 """
 import os
 import pytest
-from llmreflect.Utils.log import LOGGER
+from llmreflect.Utils.log import get_logger
+
+LOGGER = get_logger("test")
 
 
 def in_workflow():
     return os.getenv("GITHUB_ACTIONS")\
         or os.getenv("TRAVIS") \
         or os.getenv("CIRCLECI") \
         or os.getenv("GITLAB_CI")
```

### Comparing `llmreflect-0.0.6/llmreflect/Utils/database.py` & `llmreflect-0.0.7/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.6/PKG-INFO` & `llmreflect-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.0.6
+Version: 0.0.7
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

