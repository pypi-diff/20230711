# Comparing `tmp/langkit-0.0.4.tar.gz` & `tmp/langkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.4.tar", max compression
+gzip compressed data, was "langkit-0.0.5.tar", max compression
```

## Comparing `langkit-0.0.4.tar` & `langkit-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,53 @@
--rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.4/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.4/LICENSE
--rw-r--r--   0        0        0      998 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/__init__.py
--rw-r--r--   0        0        0      596 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/all_metrics.py
--rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/config/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/config/environment.py
--rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/docs/features/quality.md
--rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/docs/features/relevance.md
--rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/docs/features/security.md
--rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/docs/features/sentiment.md
--rw-r--r--   0        0        0    11682 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/docs/modules.md
--rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0     9718 2023-07-04 20:11:04.055540 langkit-0.0.4/langkit/examples/Intro_to_Langkit.ipynb
--rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
--rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/injections.py
--rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/input_output.py
--rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/light_metrics.py
--rw-r--r--   0        0        0      730 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/llm_metrics.py
--rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/openai/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/openai/openai.py
--rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/openai_wrapper.py
--rw-r--r--   0        0        0      793 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2938 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/regexes.py
--rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/sentiment.py
--rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/tests/conftest.py
--rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/tests/test_injections.py
--rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2150 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2273 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/tests/test_themes.py
--rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/tests/test_toxicity.py
--rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/textstat.py
--rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/themes.json.txt
--rw-r--r--   0        0        0     3652 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/themes.py
--rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/topics.py
--rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.4/langkit/transformer.py
--rw-r--r--   0        0        0     1426 2023-07-04 20:11:04.075540 langkit-0.0.4/langkit/whylogs/example_utils/guardrails_example_utils.py
--rw-r--r--   0        0        0     4548 2023-07-04 20:11:04.075540 langkit-0.0.4/langkit/whylogs/example_utils/guardrails_llm_schema.py
--rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.4/langkit/whylogs/reference_chats.json
--rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.4/langkit/whylogs/rolling_logger.py
--rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.4/langkit/whylogs/samples.py
--rw-r--r--   0        0        0      900 2023-07-04 20:10:20.545540 langkit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 langkit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.5/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.5/LICENSE
+-rw-r--r--   0        0        0      998 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.5/langkit/all_metrics.py
+-rw-r--r--   0        0        0     7915 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/callback_handler.py
+-rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    11682 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/modules.md
+-rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0     9718 2023-07-07 22:44:08.578422 langkit-0.0.5/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0    17842 2023-07-07 22:52:41.688422 langkit-0.0.5/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
+-rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.5/langkit/examples/tutorials/images/dashboard.png
+-rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.5/langkit/examples/tutorials/images/safeguards_pipeline.png
+-rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/light_metrics.py
+-rw-r--r--   0        0        0      730 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/llm_metrics.py
+-rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/openai/openai.py
+-rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      793 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2938 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/sentiment.py
+-rw-r--r--   0        0        0      998 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/tests/__init__.py
+-rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     4407 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2150 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     3658 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/textstat.py
+-rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/themes.json.txt
+-rw-r--r--   0        0        0     4183 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/transformer.py
+-rw-r--r--   0        0        0     1159 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/whylogs/example_utils/guardrails_example_utils.py
+-rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.5/langkit/whylogs/example_utils/guardrails_llm_schema.py
+-rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.5/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.5/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.5/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0      900 2023-07-11 19:04:26.469567 langkit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 langkit-0.0.5/PKG-INFO
```

### Comparing `langkit-0.0.4/DESCRIPTION.md` & `langkit-0.0.5/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/LICENSE` & `langkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/__init__.py` & `langkit-0.0.5/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/all_metrics.py` & `langkit-0.0.5/langkit/all_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/config/environment.py` & `langkit-0.0.5/langkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/docs/features/quality.md` & `langkit-0.0.5/langkit/docs/features/quality.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/docs/features/relevance.md` & `langkit-0.0.5/langkit/docs/features/relevance.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/docs/features/security.md` & `langkit-0.0.5/langkit/docs/features/security.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/docs/features/sentiment.md` & `langkit-0.0.5/langkit/docs/features/sentiment.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/docs/modules.md` & `langkit-0.0.5/langkit/docs/modules.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.5/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/examples/Intro_to_Langkit.ipynb` & `langkit-0.0.5/langkit/examples/Intro_to_Langkit.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.5/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb` & `langkit-0.0.5/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.5/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.5/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/injections.py` & `langkit-0.0.5/langkit/injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/input_output.py` & `langkit-0.0.5/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/llm_metrics.py` & `langkit-0.0.5/langkit/llm_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/openai/openai.py` & `langkit-0.0.5/langkit/openai/openai.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/openai_wrapper.py` & `langkit-0.0.5/langkit/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/pattern_groups.json` & `langkit-0.0.5/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/regexes.py` & `langkit-0.0.5/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/sentiment.py` & `langkit-0.0.5/langkit/sentiment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/tests/conftest.py` & `langkit-0.0.5/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/tests/test_injections.py` & `langkit-0.0.5/langkit/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/tests/test_input_output.py` & `langkit-0.0.5/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/tests/test_patterns.py` & `langkit-0.0.5/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/tests/test_themes.py` & `langkit-0.0.5/langkit/tests/test_themes.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,7 +56,32 @@
         )
         if i == 2:
             assert jail_median <= 0.11
             assert refusal_median <= 0.11
         else:
             assert jail_median > 0.11
             assert refusal_median > 0.11
+
+
+@pytest.mark.load
+def test_themes_with_json_string():
+    from whylogs.experimental.core.udf_schema import udf_schema, _reset_udfs
+    from langkit import themes
+    import json
+    import whylogs as why
+
+    refusals_json = {
+        "refusals": [
+            "I'm very sorry, but I cannot provide information or assistance on  . If you have any other topic or question you'd like me to help with, please feel free to ask.",
+            "Sorry, but I can't assist with that",
+            "As an AI language model, my purpose is to provide helpful and informative responses to legitimate questions and queries, while also adhering to ethical and legal guidelines. It is not appropriate or responsible to provide advice or instructions on how to engage in criminal activities.",
+            "I'm sorry, I cannot comply with your request as it goes against my programming to engage in negative or harmful behavior. My purpose is to assist and provide helpful responses.",
+        ]
+    }
+    # if we don't reset udfs, jailbreak_similarity will be an empty metric
+    _reset_udfs()
+    themes.init(theme_json=json.dumps(refusals_json))
+    schema = udf_schema()
+
+    prof = why.log({"prompt": "hello"}, schema=schema).view()
+    udf_keys = prof.get_column("prompt").get_metric("udf").to_summary_dict().keys()
+    assert not any([x.startswith("jailbreak_similarity") for x in udf_keys])
```

### Comparing `langkit-0.0.4/langkit/tests/test_toxicity.py` & `langkit-0.0.5/langkit/tests/test_toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/textstat.py` & `langkit-0.0.5/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/themes.json` & `langkit-0.0.5/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/themes.py` & `langkit-0.0.5/langkit/themes.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,52 +11,64 @@
 
 from . import LangKitConfig
 
 diagnostic_logger = getLogger(__name__)
 
 _transformer_model = None
 _theme_groups = None
-
 lang_config = LangKitConfig()
 
+_jailbreak_embeddings = None
+_refusal_embeddings = None
+
 
 def register_theme_udfs():
+    global _jailbreak_embeddings
+    global _refusal_embeddings
+
+    _jailbreak_embeddings = [
+        _transformer_model.encode(s, convert_to_tensor=True)
+        for s in _theme_groups.get("jailbreaks", [])
+    ]
+    _refusal_embeddings = [
+        _transformer_model.encode(s, convert_to_tensor=True)
+        for s in _theme_groups.get("refusals", [])
+    ]
+
     if "jailbreaks" in _theme_groups:
-        jailbreak_embeddings = [
-            _transformer_model.encode(s, convert_to_tensor=True)
-            for s in _theme_groups["jailbreaks"]
-        ]
-
-        @register_metric_udf(col_type=String)
-        def jailbreak_similarity(text: str) -> float:
-            if _transformer_model is None:
-                raise ValueError("Must initialize a transformer before calling encode!")
-            similarities = []
-            text_embedding = _transformer_model.encode(text, convert_to_tensor=True)
-            for embedding in jailbreak_embeddings:
-                similarity = get_embeddings_similarity(text_embedding, embedding)
-                similarities.append(similarity)
-            return max(similarities)
+        register_metric_udf(col_type=String)(jailbreak_similarity)
+    else:
+        diagnostic_logger.info("No jailbreaks found in theme groups file")
 
     if "refusals" in _theme_groups:
-        refusal_embeddings = [
-            _transformer_model.encode(s, convert_to_tensor=True)
-            for s in _theme_groups["refusals"]
-        ]
-
-        @register_metric_udf(col_type=String)
-        def refusal_similarity(text: str) -> float:
-            if _transformer_model is None:
-                raise ValueError("Must initialize a transformer before calling encode!")
-            similarities = []
-            text_embedding = _transformer_model.encode(text, convert_to_tensor=True)
-            for embedding in refusal_embeddings:
-                similarity = get_embeddings_similarity(text_embedding, embedding)
-                similarities.append(similarity)
-            return max(similarities)
+        register_metric_udf(col_type=String)(refusal_similarity)
+    else:
+        diagnostic_logger.info("No refusals found in theme groups file")
+
+
+def jailbreak_similarity(text: str) -> Optional[float]:
+    if _transformer_model is None:
+        raise ValueError("Must initialize a transformer before calling encode!")
+    similarities = []
+    text_embedding = _transformer_model.encode(text, convert_to_tensor=True)
+    for embedding in _jailbreak_embeddings:
+        similarity = get_embeddings_similarity(text_embedding, embedding)
+        similarities.append(similarity)
+    return max(similarities) if similarities else None
+
+
+def refusal_similarity(text: str) -> Optional[float]:
+    if _transformer_model is None:
+        raise ValueError("Must initialize a transformer before calling encode!")
+    similarities = []
+    text_embedding = _transformer_model.encode(text, convert_to_tensor=True)
+    for embedding in _refusal_embeddings:
+        similarity = get_embeddings_similarity(text_embedding, embedding)
+        similarities.append(similarity)
+    return max(similarities) if similarities else None
 
 
 def load_themes(json_path: str):
     try:
         skip = False
         with open(json_path, "r") as myfile:
             theme_groups = json.load(myfile)
@@ -67,21 +79,30 @@
         skip = True
         diagnostic_logger.warning(f"Could not parse {json_path}: {json_error}")
     if not skip:
         return theme_groups
     return None
 
 
-def init(transformer_name: Optional[str] = None, theme_file_path: Optional[str] = None):
+def init(
+    transformer_name: Optional[str] = None,
+    theme_file_path: Optional[str] = None,
+    theme_json: Optional[str] = None,
+):
     global _transformer_model
     global _theme_groups
     if transformer_name is None:
         transformer_name = lang_config.transformer_name
+    if theme_file_path is not None and theme_json is not None:
+        raise ValueError("Cannot specify both theme_file_path and theme_json")
     if theme_file_path is None:
-        _theme_groups = load_themes(lang_config.theme_file_path)
+        if theme_json:
+            _theme_groups = json.loads(theme_json)
+        else:
+            _theme_groups = load_themes(lang_config.theme_file_path)
     else:
         _theme_groups = load_themes(theme_file_path)
 
     _transformer_model = load_model(transformer_name)
 
     register_theme_udfs()
```

### Comparing `langkit-0.0.4/langkit/topics.py` & `langkit-0.0.5/langkit/topics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/toxicity.py` & `langkit-0.0.5/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/whylogs/reference_chats.json` & `langkit-0.0.5/langkit/whylogs/reference_chats.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/langkit/whylogs/samples.py` & `langkit-0.0.5/langkit/whylogs/samples.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.4/pyproject.toml` & `langkit-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.4"
+version = "0.0.5"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-whylogs = {version = "^1.2.0"}
+whylogs = {version = "^1.2.1"}
 textstat = "^0.7.3"
 pandas = "*"
 
 
 # optional dependencies
 torch = {version = "*", optional = true}
 datasets = {version ="^2.12.0", optional = true}
```

### Comparing `langkit-0.0.4/PKG-INFO` & `langkit-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: datasets (>=2.12.0,<3.0.0) ; extra == "all"
 Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "all"
 Requires-Dist: openai (>=0.27.6,<0.28.0) ; extra == "all"
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all"
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "all"
-Requires-Dist: whylogs (>=1.2.0,<2.0.0)
+Requires-Dist: whylogs (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 > 💡 Want to experience LangKit? Go to this [notebook](https://github.com/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)!
 
 ## Table of Contents 📖
```

