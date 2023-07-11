# Comparing `tmp/pyspark_ai-0.1.8.tar.gz` & `tmp/pyspark_ai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_ai-0.1.8.tar", max compression
+gzip compressed data, was "pyspark_ai-0.1.9.tar", max compression
```

## Comparing `pyspark_ai-0.1.8.tar` & `pyspark_ai-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.8/LICENSE
--rw-r--r--   0        0        0     5215 2023-07-01 05:38:10.252689 pyspark_ai-0.1.8/README.md
--rw-r--r--   0        0        0     1020 2023-07-01 08:08:32.966294 pyspark_ai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.8/pyspark_ai/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.8/pyspark_ai/ai_utils.py
--rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.8/pyspark_ai/cache.py
--rw-r--r--   0        0        0     1954 2023-07-01 04:48:49.616610 pyspark_ai-0.1.8/pyspark_ai/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.8/pyspark_ai/file_cache.py
--rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.8/pyspark_ai/llm_chain_with_cache.py
--rw-r--r--   0        0        0     9288 2023-06-28 23:32:33.674290 pyspark_ai-0.1.8/pyspark_ai/prompt.py
--rw-r--r--   0        0        0    17555 2023-06-29 00:12:04.660577 pyspark_ai-0.1.8/pyspark_ai/pyspark_ai.py
--rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.8/pyspark_ai/search_tool_with_cache.py
--rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 pyspark_ai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5855 2023-07-07 23:19:15.890162 pyspark_ai-0.1.9/README.md
+-rw-r--r--   0        0        0     1020 2023-07-11 07:34:52.275111 pyspark_ai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.9/pyspark_ai/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.9/pyspark_ai/ai_utils.py
+-rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.9/pyspark_ai/cache.py
+-rw-r--r--   0        0        0     1954 2023-07-01 04:48:49.616610 pyspark_ai-0.1.9/pyspark_ai/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.9/pyspark_ai/file_cache.py
+-rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.9/pyspark_ai/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     9288 2023-06-28 23:32:33.674290 pyspark_ai-0.1.9/pyspark_ai/prompt.py
+-rw-r--r--   0        0        0    17849 2023-07-11 07:34:37.651390 pyspark_ai-0.1.9/pyspark_ai/pyspark_ai.py
+-rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.9/pyspark_ai/search_tool_with_cache.py
+-rw-r--r--   0        0        0     7022 1970-01-01 00:00:00.000000 pyspark_ai-0.1.9/PKG-INFO
```

### Comparing `pyspark_ai-0.1.8/LICENSE` & `pyspark_ai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/README.md` & `pyspark_ai-0.1.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 
 ## Introduction
 The English SDK for Apache Spark is an extremely simple yet powerful tool. It takes English instructions and compile them into PySpark objects like DataFrames.
 Its goal is to make Spark more user-friendly and accessible, allowing you to focus your efforts on extracting insights from your data.
 
 For a more comprehensive introduction and background to our project, we have the following resources:
 - [Blog Post](https://www.databricks.com/blog/introducing-english-new-programming-language-apache-spark): A detailed walkthrough of our project.
-- [Demo Video](https://www.youtube.com/watch?v=yj7XlTB1Jvc&t=511s): DATA+AI summit announcement video with demo.
+- [Demo Video](https://www.youtube.com/watch?v=yj7XlTB1Jvc&t=511s): 2023 Data + AI summit announcement video with demo.
+- [Breakout Session](https://www.youtube.com/watch?v=ZunjkL3L62o&t=73s): A deep dive into the story behind the English SDK, its features, and future works at DATA+AI summit 2023.
 
 ## Installation
 
 ```bash
 pip install pyspark-ai
 ```
 
 ## Configuring OpenAI LLMs
-As of June 2023, our extensive testing suggests the most effective utilization with the English SDK and GPT-4.
+As of July 2023, we have found that the GPT-4 works optimally with the English SDK. This superior AI model is readily accessible to all developers through the OpenAI API.
 
 To use OpenAI's Language Learning Models (LLMs), you can set your OpenAI secret key as the `OPENAI_API_KEY` environment variable. This key can be found in your [OpenAI account](https://platform.openai.com/account/api-keys). Example:
 ```bash
 export OPENAI_API_KEY='sk-...'
 ```
 By default, the `SparkAI` instances will use the GPT-4 model. However, you're encouraged to experiment with creating and implementing other LLMs, which can be passed during the initialization of `SparkAI` instances for various use-cases.
 
 ## Usage
 ### Initialization
 
 ```python
-from langchain.chat_models import ChatOpenAI
 from pyspark_ai import SparkAI
 
-# If 'gpt-4' is unavailable, use 'gpt-3.5-turbo' (might lower output quality)
-llm = ChatOpenAI(model_name='gpt-4', temperature=0)
-
-# Initialize SparkAI with the ChatOpenAI model
-spark_ai = SparkAI(llm=llm, verbose=True)
-
-# Activate partial functions for Spark DataFrame
-spark_ai.activate()
+spark_ai = SparkAI()
+spark_ai.activate()  # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 If you have [set up the Google Python client](https://developers.google.com/docs/api/quickstart/python), you can ingest data via search engine:
 ```python
 auto_df = spark_ai.create_df("2022 USA national auto sales by brand")
 ```
@@ -125,11 +119,18 @@
 ```python
 spark_ai.commit()
 ```
 
 Refer to [example.ipynb](https://github.com/databrickslabs/pyspark-ai/blob/master/examples/example.ipynb) for more detailed usage examples.
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+We're delighted that you're considering contributing to the English SDK for Apache Spark project! Whether you're fixing a bug or proposing a new feature, your contribution is highly appreciated.
+
+Before you start, please take a moment to read our [Contribution Guide](./CONTRIBUTING.md). This guide provides an overview of how you can contribute to our project. We're currently in the early stages of development and we're working on introducing more comprehensive test cases and Github Action jobs for enhanced testing of each pull request.
+
+If you have any questions or need assistance, feel free to open a new issue in the GitHub repository.
+
+Thank you for helping us improve the English SDK for Apache Spark. We're excited to see your contributions!
 
 ## License
 Licensed under the Apache License 2.0.
```

### Comparing `pyspark_ai-0.1.8/pyproject.toml` & `pyspark_ai-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyspark-ai"
-version = "0.1.8"
+version = "0.1.9"
 description = "English SDK for Apache Spark"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/databrickslabs/pyspark-ai"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyspark_ai-0.1.8/pyspark_ai/ai_utils.py` & `pyspark_ai-0.1.9/pyspark_ai/ai_utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/pyspark_ai/cache.py` & `pyspark_ai-0.1.9/pyspark_ai/cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/pyspark_ai/code_logger.py` & `pyspark_ai-0.1.9/pyspark_ai/code_logger.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/pyspark_ai/file_cache.py` & `pyspark_ai-0.1.9/pyspark_ai/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/pyspark_ai/llm_chain_with_cache.py` & `pyspark_ai-0.1.9/pyspark_ai/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/pyspark_ai/prompt.py` & `pyspark_ai-0.1.9/pyspark_ai/prompt.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/pyspark_ai/pyspark_ai.py` & `pyspark_ai-0.1.9/pyspark_ai/pyspark_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,30 @@
 from pyspark_ai.search_tool_with_cache import SearchToolWithCache
 from pyspark_ai.ai_utils import AIUtils
 
 
 class SparkAI:
     _HTTP_HEADER = {
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36"
-        " (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
+                      " (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
         "Accept-Language": "en-US,en;q=0.5",
     }
 
     def __init__(
-        self,
-        llm: Optional[BaseLanguageModel] = None,
-        web_search_tool: Optional[Callable[[str], str]] = None,
-        spark_session: Optional[SparkSession] = None,
-        enable_cache: bool = True,
-        cache_file_format: str = "json",
-        cache_file_location: Optional[str] = None,
-        encoding: Optional[Encoding] = None,
-        max_tokens_of_web_content: int = 3000,
-        verbose: bool = False,
+            self,
+            llm: Optional[BaseLanguageModel] = None,
+            web_search_tool: Optional[Callable[[str], str]] = None,
+            spark_session: Optional[SparkSession] = None,
+            enable_cache: bool = True,
+            cache_file_format: str = "json",
+            cache_file_location: Optional[str] = None,
+            encoding: Optional[Encoding] = None,
+            max_tokens_of_web_content: int = 3000,
+            verbose: bool = False,
     ) -> None:
         """
         Initialize the SparkAI object with the provided parameters.
 
         :param llm: LLM instance for selecting web search result
                                  and writing the ingestion SQL query.
         :param web_search_tool: optional function to perform web search,
@@ -184,29 +184,29 @@
         """
         tokens = list(self._encoding.encode(text))
         if len(tokens) > max_tokens:
             tokens = tokens[:max_tokens]
         return self._encoding.decode(tokens)
 
     def _get_url_from_search_tool(
-        self, desc: str, columns: Optional[List[str]], cache: bool
+            self, desc: str, columns: Optional[List[str]], cache: bool
     ) -> str:
         search_result = self._web_search_tool(desc)
         search_columns_hint = self._generate_search_prompt(columns)
         # Run the LLM chain to pick the best search result
         tags = self._get_tags(cache)
         return self._search_llm_chain.run(
             tags=tags,
             query=desc,
             search_results=search_result,
             columns={search_columns_hint},
         )
 
     def _create_dataframe_with_llm(
-        self, text: str, desc: str, columns: Optional[List[str]], cache: bool
+            self, text: str, desc: str, columns: Optional[List[str]], cache: bool
     ) -> DataFrame:
         clean_text = " ".join(text.split())
         web_content = self._trim_text_from_end(
             clean_text, self._max_tokens_of_web_content
         )
 
         sql_columns_hint = self._generate_sql_prompt(columns)
@@ -270,15 +270,15 @@
 
     def _get_tags(self, cache: bool) -> Optional[List[str]]:
         if self._enable_cache and not cache:
             return SKIP_CACHE_TAGS
         return None
 
     def create_df(
-        self, desc: str, columns: Optional[List[str]] = None, cache: bool = True
+            self, desc: str, columns: Optional[List[str]] = None, cache: bool = True
     ) -> DataFrame:
         """
         Create a Spark DataFrame by querying an LLM from web search result.
 
         :param desc: the description of the result DataFrame, which will be used for
                      web searching
         :param columns: the expected column names in the result DataFrame
@@ -317,15 +317,15 @@
         if is_url:
             desc = soup.title.string
         return self._create_dataframe_with_llm(
             page_content, desc, columns, cache
         )
 
     def transform_df(
-        self, df: DataFrame, desc: str, cache: bool = True
+            self, df: DataFrame, desc: str, cache: bool = True
     ) -> DataFrame:
         """
         This method applies a transformation to a provided Spark DataFrame, the specifics of which are determined by the 'desc' parameter.
 
         :param df: The Spark DataFrame that is to be transformed.
         :param desc: A natural language string that outlines the specific transformation to be applied on the DataFrame.
         :param cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
@@ -358,15 +358,15 @@
         if "```" in explain_result:
             summary = explain_result.split("```")[-1]
             return summary.strip()
         else:
             return explain_result
 
     def plot_df(
-        self, df: DataFrame, desc: Optional[str] = None, cache: bool = True
+            self, df: DataFrame, desc: Optional[str] = None, cache: bool = True
     ) -> None:
         instruction = f"The purpose of the plot: {desc}" if desc is not None else ""
         tags = self._get_tags(cache)
         response = self._plot_chain.run(
             tags=tags,
             columns=self._get_df_schema(df),
             explain=self._get_df_explain(df, cache),
@@ -421,16 +421,20 @@
 
     def activate(self):
         """
         Activates AI utility functions for Spark DataFrame.
         """
         DataFrame.ai = AIUtils(self)
         # Patch the Spark Connect DataFrame as well.
-        from pyspark.sql.connect.dataframe import DataFrame as CDataFrame
-        CDataFrame.ai = AIUtils(self)
+        try:
+            from pyspark.sql.connect.dataframe import DataFrame as CDataFrame
+            CDataFrame.ai = AIUtils(self)
+        except ImportError:
+            self.log("The pyspark.sql.connect.dataframe module could not be imported. "
+                     "This might be due to your PySpark version being below 3.4.")
 
     def commit(self):
         """
         Commit the staging in-memory cache into persistent cache, if cache is enabled.
         """
         if self._cache is not None:
             self._cache.commit()
```

### Comparing `pyspark_ai-0.1.8/pyspark_ai/search_tool_with_cache.py` & `pyspark_ai-0.1.9/pyspark_ai/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.8/PKG-INFO` & `pyspark_ai-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-ai
-Version: 0.1.8
+Version: 0.1.9
 Summary: English SDK for Apache Spark
 Home-page: https://github.com/databrickslabs/pyspark-ai
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -35,46 +35,40 @@
 
 ## Introduction
 The English SDK for Apache Spark is an extremely simple yet powerful tool. It takes English instructions and compile them into PySpark objects like DataFrames.
 Its goal is to make Spark more user-friendly and accessible, allowing you to focus your efforts on extracting insights from your data.
 
 For a more comprehensive introduction and background to our project, we have the following resources:
 - [Blog Post](https://www.databricks.com/blog/introducing-english-new-programming-language-apache-spark): A detailed walkthrough of our project.
-- [Demo Video](https://www.youtube.com/watch?v=yj7XlTB1Jvc&t=511s): DATA+AI summit announcement video with demo.
+- [Demo Video](https://www.youtube.com/watch?v=yj7XlTB1Jvc&t=511s): 2023 Data + AI summit announcement video with demo.
+- [Breakout Session](https://www.youtube.com/watch?v=ZunjkL3L62o&t=73s): A deep dive into the story behind the English SDK, its features, and future works at DATA+AI summit 2023.
 
 ## Installation
 
 ```bash
 pip install pyspark-ai
 ```
 
 ## Configuring OpenAI LLMs
-As of June 2023, our extensive testing suggests the most effective utilization with the English SDK and GPT-4.
+As of July 2023, we have found that the GPT-4 works optimally with the English SDK. This superior AI model is readily accessible to all developers through the OpenAI API.
 
 To use OpenAI's Language Learning Models (LLMs), you can set your OpenAI secret key as the `OPENAI_API_KEY` environment variable. This key can be found in your [OpenAI account](https://platform.openai.com/account/api-keys). Example:
 ```bash
 export OPENAI_API_KEY='sk-...'
 ```
 By default, the `SparkAI` instances will use the GPT-4 model. However, you're encouraged to experiment with creating and implementing other LLMs, which can be passed during the initialization of `SparkAI` instances for various use-cases.
 
 ## Usage
 ### Initialization
 
 ```python
-from langchain.chat_models import ChatOpenAI
 from pyspark_ai import SparkAI
 
-# If 'gpt-4' is unavailable, use 'gpt-3.5-turbo' (might lower output quality)
-llm = ChatOpenAI(model_name='gpt-4', temperature=0)
-
-# Initialize SparkAI with the ChatOpenAI model
-spark_ai = SparkAI(llm=llm, verbose=True)
-
-# Activate partial functions for Spark DataFrame
-spark_ai.activate()
+spark_ai = SparkAI()
+spark_ai.activate()  # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 If you have [set up the Google Python client](https://developers.google.com/docs/api/quickstart/python), you can ingest data via search engine:
 ```python
 auto_df = spark_ai.create_df("2022 USA national auto sales by brand")
 ```
@@ -155,12 +149,19 @@
 ```python
 spark_ai.commit()
 ```
 
 Refer to [example.ipynb](https://github.com/databrickslabs/pyspark-ai/blob/master/examples/example.ipynb) for more detailed usage examples.
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+We're delighted that you're considering contributing to the English SDK for Apache Spark project! Whether you're fixing a bug or proposing a new feature, your contribution is highly appreciated.
+
+Before you start, please take a moment to read our [Contribution Guide](./CONTRIBUTING.md). This guide provides an overview of how you can contribute to our project. We're currently in the early stages of development and we're working on introducing more comprehensive test cases and Github Action jobs for enhanced testing of each pull request.
+
+If you have any questions or need assistance, feel free to open a new issue in the GitHub repository.
+
+Thank you for helping us improve the English SDK for Apache Spark. We're excited to see your contributions!
 
 ## License
 Licensed under the Apache License 2.0.
```

