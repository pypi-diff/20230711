# Comparing `tmp/rasa-3.6.2.tar.gz` & `tmp/rasa-3.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-3.6.2.tar", max compression
+gzip compressed data, was "rasa-3.7.0b1.tar", max compression
```

## Comparing `rasa-3.6.2.tar` & `rasa-3.7.0b1.tar`

### file list

```diff
@@ -1,316 +1,317 @@
--rw-r--r--   0        0        0    11352 2023-07-06 11:51:02.973860 rasa-3.6.2/LICENSE.txt
--rw-r--r--   0        0        0    21489 2023-07-06 11:51:02.973860 rasa-3.6.2/README.md
--rw-r--r--   0        0        0     9562 2023-07-06 11:51:03.137874 rasa-3.6.2/pyproject.toml
--rw-r--r--   0        0        0      280 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/__init__.py
--rw-r--r--   0        0        0     5441 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/__main__.py
--rw-r--r--   0        0        0     5314 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/api.py
--rw-r--r--   0        0        0      115 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/__init__.py
--rw-r--r--   0        0        0     2388 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/data.py
--rw-r--r--   0        0        0     5242 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/default_arguments.py
--rw-r--r--   0        0        0     2199 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/evaluate.py
--rw-r--r--   0        0        0     1499 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/export.py
--rw-r--r--   0        0        0     2685 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/interactive.py
--rw-r--r--   0        0        0     5674 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/run.py
--rw-r--r--   0        0        0      367 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/shell.py
--rw-r--r--   0        0        0     6853 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/test.py
--rw-r--r--   0        0        0     8279 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/train.py
--rw-r--r--   0        0        0      861 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/visualize.py
--rw-r--r--   0        0        0     1027 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/arguments/x.py
--rw-r--r--   0        0        0     9722 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/data.py
--rw-r--r--   0        0        0     7948 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/evaluate.py
--rw-r--r--   0        0        0     8204 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/export.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/actions/__init__.py
--rw-r--r--   0        0        0      742 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/actions/actions.py
--rw-r--r--   0        0        0     1505 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/config.yml
--rw-r--r--   0        0        0      998 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/credentials.yml
--rw-r--r--   0        0        0     1433 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/data/nlu.yml
--rw-r--r--   0        0        0      244 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/data/rules.yml
--rw-r--r--   0        0        0      542 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/data/stories.yml
--rw-r--r--   0        0        0      565 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/domain.yml
--rw-r--r--   0        0        0     1411 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/endpoints.yml
--rw-r--r--   0        0        0     1664 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/initial_project/tests/test_stories.yml
--rw-r--r--   0        0        0     5943 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/interactive.py
--rw-r--r--   0        0        0     4196 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/run.py
--rw-r--r--   0        0        0     6846 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/scaffold.py
--rw-r--r--   0        0        0     4264 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/shell.py
--rw-r--r--   0        0        0     3118 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/telemetry.py
--rw-r--r--   0        0        0     8888 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/test.py
--rw-r--r--   0        0        0     7798 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/train.py
--rw-r--r--   0        0        0    12508 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/utils.py
--rw-r--r--   0        0        0     1256 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/visualize.py
--rw-r--r--   0        0        0     6785 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/cli/x.py
--rw-r--r--   0        0        0     1172 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/constants.py
--rw-r--r--   0        0        0      123 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/actions/__init__.py
--rw-r--r--   0        0        0    46526 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/actions/action.py
--rw-r--r--   0        0        0       78 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/actions/constants.py
--rw-r--r--   0        0        0    26651 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/actions/forms.py
--rw-r--r--   0        0        0     3322 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/actions/loops.py
--rw-r--r--   0        0        0     6078 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/actions/two_stage_fallback.py
--rw-r--r--   0        0        0    20445 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/agent.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/brokers/__init__.py
--rw-r--r--   0        0        0     4398 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/brokers/broker.py
--rw-r--r--   0        0        0     1801 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/brokers/file.py
--rw-r--r--   0        0        0    12002 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/brokers/kafka.py
--rw-r--r--   0        0        0    14160 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/brokers/pika.py
--rw-r--r--   0        0        0     2754 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/brokers/sql.py
--rw-r--r--   0        0        0     1656 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/channels/__init__.py
--rw-r--r--   0        0        0    11669 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/channels/botframework.py
--rw-r--r--   0        0        0     2746 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/channels/callback.py
--rw-r--r--   0        0        0    13331 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/channels/channel.py
--rw-r--r--   0        0        0     8073 2023-07-06 11:51:03.137874 rasa-3.6.2/rasa/core/channels/console.py
--rw-r--r--   0        0        0    15812 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/facebook.py
--rw-r--r--   0        0        0    11560 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/hangouts.py
--rw-r--r--   0        0        0     7743 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/mattermost.py
--rw-r--r--   0        0        0     4814 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/rasa_chat.py
--rw-r--r--   0        0        0     6949 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/rest.py
--rw-r--r--   0        0        0     5999 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/rocketchat.py
--rw-r--r--   0        0        0    24405 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/slack.py
--rw-r--r--   0        0        0    10163 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/socketio.py
--rw-r--r--   0        0        0    10630 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/telegram.py
--rw-r--r--   0        0        0     5938 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/twilio.py
--rw-r--r--   0        0        0    13181 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/twilio_voice.py
--rw-r--r--   0        0        0     4845 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/channels/webexteams.py
--rw-r--r--   0        0        0     3047 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/constants.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/evaluation/__init__.py
--rw-r--r--   0        0        0     9154 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/evaluation/marker.py
--rw-r--r--   0        0        0    38043 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/evaluation/marker_base.py
--rw-r--r--   0        0        0    12086 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/evaluation/marker_stats.py
--rw-r--r--   0        0        0     3658 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/evaluation/marker_tracker_loader.py
--rw-r--r--   0        0        0      901 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/exceptions.py
--rw-r--r--   0        0        0    10220 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/exporter.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/featurizers/__init__.py
--rw-r--r--   0        0        0    17964 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/featurizers/precomputation.py
--rw-r--r--   0        0        0    15447 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/featurizers/single_state_featurizer.py
--rw-r--r--   0        0        0    43363 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/featurizers/tracker_featurizers.py
--rw-r--r--   0        0        0     3024 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/http_interpreter.py
--rw-r--r--   0        0        0     2018 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/jobs.py
--rw-r--r--   0        0        0     4719 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/lock.py
--rw-r--r--   0        0        0    11678 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/lock_store.py
--rw-r--r--   0        0        0    14821 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/migrate.py
--rw-r--r--   0        0        0      240 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/nlg/__init__.py
--rw-r--r--   0        0        0     3870 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/nlg/callback.py
--rw-r--r--   0        0        0     3285 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/nlg/generator.py
--rw-r--r--   0        0        0     2635 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/nlg/interpolator.py
--rw-r--r--   0        0        0     7503 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/nlg/response.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/__init__.py
--rw-r--r--   0        0        0    12959 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/ensemble.py
--rw-r--r--   0        0        0    19295 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/memoization.py
--rw-r--r--   0        0        0    25038 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/policy.py
--rw-r--r--   0        0        0    50315 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/rule_policy.py
--rw-r--r--   0        0        0    86521 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/ted_policy.py
--rw-r--r--   0        0        0    39329 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/policies/unexpected_intent_policy.py
--rw-r--r--   0        0        0    40848 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/processor.py
--rw-r--r--   0        0        0     9243 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/run.py
--rw-r--r--   0        0        0    48935 2023-07-06 11:51:03.141874 rasa-3.6.2/rasa/core/test.py
--rw-r--r--   0        0        0    58040 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/tracker_store.py
--rw-r--r--   0        0        0     3543 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/train.py
--rw-r--r--   0        0        0     3218 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/training/converters/__init__.py
--rw-r--r--   0        0        0     3889 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/training/converters/responses_prefix_converter.py
--rw-r--r--   0        0        0    59595 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/training/interactive.py
--rw-r--r--   0        0        0    13604 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/training/story_conflict.py
--rw-r--r--   0        0        0     3067 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/training/training.py
--rw-r--r--   0        0        0    10995 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/utils.py
--rw-r--r--   0        0        0     2125 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/core/visualize.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/__init__.py
--rw-r--r--   0        0        0    16744 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/caching.py
--rw-r--r--   0        0        0      469 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/constants.py
--rw-r--r--   0        0        0      437 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/exceptions.py
--rw-r--r--   0        0        0    22105 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/graph.py
--rw-r--r--   0        0        0     1384 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/loader.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/recipes/__init__.py
--rw-r--r--   0        0        0     1139 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/recipes/config_files/default_config.yml
--rw-r--r--   0        0        0     3244 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/recipes/default_components.py
--rw-r--r--   0        0        0    43587 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/recipes/default_recipe.py
--rw-r--r--   0        0        0     3301 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/recipes/graph_recipe.py
--rw-r--r--   0        0        0     3354 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/recipes/recipe.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/runner/__init__.py
--rw-r--r--   0        0        0     4302 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/runner/dask.py
--rw-r--r--   0        0        0     1672 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/runner/interface.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/storage/__init__.py
--rw-r--r--   0        0        0     9581 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/storage/local_model_storage.py
--rw-r--r--   0        0        0     3931 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/storage/resource.py
--rw-r--r--   0        0        0     6923 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/storage/storage.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/training/__init__.py
--rw-r--r--   0        0        0     6524 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/training/components.py
--rw-r--r--   0        0        0     1848 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/training/fingerprinting.py
--rw-r--r--   0        0        0    10516 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/training/graph_trainer.py
--rw-r--r--   0        0        0     5036 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/training/hooks.py
--rw-r--r--   0        0        0    22697 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/engine/validation.py
--rw-r--r--   0        0        0     2132 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/converters/__init__.py
--rw-r--r--   0        0        0     1576 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/converters/nlu_message_converter.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/__init__.py
--rw-r--r--   0        0        0     3832 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/domain_for_core_training_provider.py
--rw-r--r--   0        0        0     2571 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/domain_provider.py
--rw-r--r--   0        0        0     1294 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/forms_provider.py
--rw-r--r--   0        0        0     2119 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/nlu_training_data_provider.py
--rw-r--r--   0        0        0     1354 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/responses_provider.py
--rw-r--r--   0        0        0     1540 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/rule_only_provider.py
--rw-r--r--   0        0        0     1466 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/story_graph_provider.py
--rw-r--r--   0        0        0     1965 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/providers/training_tracker_provider.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/validators/__init__.py
--rw-r--r--   0        0        0    22668 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/validators/default_recipe_validator.py
--rw-r--r--   0        0        0    12863 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/graph_components/validators/finetuning_validator.py
--rw-r--r--   0        0        0     1782 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/jupyter.py
--rw-r--r--   0        0        0      101 2023-07-06 11:51:20.163318 rasa-3.6.2/rasa/keys
--rw-r--r--   0        0        0     3490 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/model.py
--rw-r--r--   0        0        0    14961 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/model_testing.py
--rw-r--r--   0        0        0    16836 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/model_training.py
--rw-r--r--   0        0        0      123 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/__init__.py
--rw-r--r--   0        0        0      118 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/__init__.py
--rw-r--r--   0        0        0      133 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/classifier.py
--rw-r--r--   0        0        0    71637 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/diet_classifier.py
--rw-r--r--   0        0        0     7150 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/fallback_classifier.py
--rw-r--r--   0        0        0     7581 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/keyword_intent_classifier.py
--rw-r--r--   0        0        0     7568 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/logistic_regression_classifier.py
--rw-r--r--   0        0        0     5559 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/mitie_intent_classifier.py
--rw-r--r--   0        0        0     1989 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/regex_message_handler.py
--rw-r--r--   0        0        0    11915 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/classifiers/sklearn_intent_classifier.py
--rw-r--r--   0        0        0     2757 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/constants.py
--rw-r--r--   0        0        0     1317 2023-07-06 11:51:03.145874 rasa-3.6.2/rasa/nlu/convert.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/emulators/__init__.py
--rw-r--r--   0        0        0     1748 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/emulators/dialogflow.py
--rw-r--r--   0        0        0     1367 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/emulators/emulator.py
--rw-r--r--   0        0        0     3032 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/emulators/luis.py
--rw-r--r--   0        0        0      334 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/emulators/no_emulator.py
--rw-r--r--   0        0        0     1930 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/emulators/wit.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/__init__.py
--rw-r--r--   0        0        0    26499 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/crf_entity_extractor.py
--rw-r--r--   0        0        0     7685 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/duckling_entity_extractor.py
--rw-r--r--   0        0        0     7160 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/entity_synonyms.py
--rw-r--r--   0        0        0    17530 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/extractor.py
--rw-r--r--   0        0        0    10973 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/mitie_entity_extractor.py
--rw-r--r--   0        0        0     8289 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/regex_entity_extractor.py
--rw-r--r--   0        0        0     3366 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/extractors/spacy_entity_extractor.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/__init__.py
--rw-r--r--   0        0        0    17142 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
--rw-r--r--   0        0        0     2433 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
--rw-r--r--   0        0        0    30361 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
--rw-r--r--   0        0        0     5861 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
--rw-r--r--   0        0        0     4888 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
--rw-r--r--   0        0        0     3347 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/featurizer.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/__init__.py
--rw-r--r--   0        0        0    33295 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
--rw-r--r--   0        0        0    21810 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
--rw-r--r--   0        0        0    10289 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
--rw-r--r--   0        0        0      220 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
--rw-r--r--   0        0        0      557 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/model.py
--rw-r--r--   0        0        0     8333 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/persistor.py
--rw-r--r--   0        0        0      803 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/run.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/selectors/__init__.py
--rw-r--r--   0        0        0    39012 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/selectors/response_selector.py
--rw-r--r--   0        0        0    67726 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/test.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/tokenizers/__init__.py
--rw-r--r--   0        0        0     5374 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/tokenizers/jieba_tokenizer.py
--rw-r--r--   0        0        0     2618 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/tokenizers/mitie_tokenizer.py
--rw-r--r--   0        0        0     2378 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/tokenizers/spacy_tokenizer.py
--rw-r--r--   0        0        0     8196 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3750 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      928 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/__init__.py
--rw-r--r--   0        0        0    14703 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/bilou_utils.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/hugging_face/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/hugging_face/registry.py
--rw-r--r--   0        0        0     9143 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
--rw-r--r--   0        0        0     3887 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/mitie_utils.py
--rw-r--r--   0        0        0     5386 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/pattern_utils.py
--rw-r--r--   0        0        0    11795 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/nlu/utils/spacy_utils.py
--rw-r--r--   0        0        0     4921 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/plugin.py
--rw-r--r--   0        0        0    55589 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/server.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/shared/__init__.py
--rw-r--r--   0        0        0     4294 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/shared/constants.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.149875 rasa-3.6.2/rasa/shared/core/__init__.py
--rw-r--r--   0        0        0     4346 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/constants.py
--rw-r--r--   0        0        0     1366 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/conversation.py
--rw-r--r--   0        0        0    77445 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/domain.py
--rw-r--r--   0        0        0    65862 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/events.py
--rw-r--r--   0        0        0    35597 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/generator.py
--rw-r--r--   0        0        0     8286 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/slot_mappings.py
--rw-r--r--   0        0        0    16371 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/slots.py
--rw-r--r--   0        0        0    33790 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/trackers.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/__init__.py
--rw-r--r--   0        0        0     2895 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/loading.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_reader/__init__.py
--rw-r--r--   0        0        0     4449 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_reader/story_reader.py
--rw-r--r--   0        0        0     6671 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_reader/story_step_builder.py
--rw-r--r--   0        0        0    32976 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_writer/__init__.py
--rw-r--r--   0        0        0     2543 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_writer/story_writer.py
--rw-r--r--   0        0        0    14903 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
--rw-r--r--   0        0        0    29313 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/structures.py
--rw-r--r--   0        0        0     3500 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/visualization.html
--rw-r--r--   0        0        0    20341 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/core/training_data/visualization.py
--rw-r--r--   0        0        0     5479 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/data.py
--rw-r--r--   0        0        0     3633 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/importers/__init__.py
--rw-r--r--   0        0        0    21866 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/importers/importer.py
--rw-r--r--   0        0        0     7836 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/importers/multi_project.py
--rw-r--r--   0        0        0     3388 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/importers/rasa.py
--rw-r--r--   0        0        0      861 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/importers/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/constants.py
--rw-r--r--   0        0        0      188 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/interpreter.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/__init__.py
--rw-r--r--   0        0        0     6759 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/entities_parser.py
--rw-r--r--   0        0        0    14835 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/features.py
--rw-r--r--   0        0        0      453 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/__init__.py
--rw-r--r--   0        0        0     6123 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/dialogflow.py
--rw-r--r--   0        0        0     3014 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/luis.py
--rw-r--r--   0        0        0     4495 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/rasa.py
--rw-r--r--   0        0        0    22353 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/rasa_yaml.py
--rw-r--r--   0        0        0     8540 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/readerwriter.py
--rw-r--r--   0        0        0     1820 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/formats/wit.py
--rw-r--r--   0        0        0     4258 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/loading.py
--rw-r--r--   0        0        0     1116 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/lookup_tables_parser.py
--rw-r--r--   0        0        0    16662 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/message.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/schemas/__init__.py
--rw-r--r--   0        0        0     2565 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/schemas/data_schema.py
--rw-r--r--   0        0        0     1179 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/schemas/nlu.yml
--rw-r--r--   0        0        0     1661 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/schemas/responses.yml
--rw-r--r--   0        0        0     1476 2023-07-06 11:51:03.153875 rasa-3.6.2/rasa/shared/nlu/training_data/synonyms_parser.py
--rw-r--r--   0        0        0    28493 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/nlu/training_data/training_data.py
--rw-r--r--   0        0        0     7040 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/nlu/training_data/util.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/cli.py
--rw-r--r--   0        0        0     8731 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/common.py
--rw-r--r--   0        0        0    20533 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/io.py
--rw-r--r--   0        0        0      883 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/pykwalify_extensions.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/schemas/__init__.py
--rw-r--r--   0        0        0       27 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/schemas/config.yml
--rw-r--r--   0        0        0     3267 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/schemas/domain.yml
--rw-r--r--   0        0        0     5569 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/schemas/events.py
--rw-r--r--   0        0        0      998 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/schemas/model_config.yml
--rw-r--r--   0        0        0     4034 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/schemas/stories.yml
--rw-r--r--   0        0        0    10317 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/shared/utils/validation.py
--rw-r--r--   0        0        0    36273 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/telemetry.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/__init__.py
--rw-r--r--   0        0        0    19532 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/common.py
--rw-r--r--   0        0        0     1647 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/converter.py
--rw-r--r--   0        0        0     8796 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/endpoints.py
--rw-r--r--   0        0        0     7831 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/io.py
--rw-r--r--   0        0        0     4482 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/log_utils.py
--rw-r--r--   0        0        0    12246 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/plotting.py
--rw-r--r--   0        0        0        0 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     4036 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/callback.py
--rw-r--r--   0        0        0     3140 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/constants.py
--rw-r--r--   0        0        0    19658 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/crf.py
--rw-r--r--   0        0        0    15526 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/data_generator.py
--rw-r--r--   0        0        0     5576 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/environment.py
--rw-r--r--   0        0        0      168 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/exceptions.py
--rw-r--r--   0        0        0    59263 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/layers.py
--rw-r--r--   0        0        0     3319 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/layers_utils.py
--rw-r--r--   0        0        0    10055 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/metrics.py
--rw-r--r--   0        0        0    34572 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/model_data.py
--rw-r--r--   0        0        0    18667 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/model_data_utils.py
--rw-r--r--   0        0        0    36004 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/models.py
--rw-r--r--   0        0        0    49066 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/rasa_layers.py
--rw-r--r--   0        0        0    25509 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/transformer.py
--rw-r--r--   0        0        0      204 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/tensorflow/types.py
--rw-r--r--   0        0        0    20999 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/utils/train_utils.py
--rw-r--r--   0        0        0    17708 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/validator.py
--rw-r--r--   0        0        0      116 2023-07-06 11:51:03.157875 rasa-3.6.2/rasa/version.py
--rw-r--r--   0        0        0    28124 1970-01-01 00:00:00.000000 rasa-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-07-06 19:05:30.052939 rasa-3.7.0b1/LICENSE.txt
+-rw-r--r--   0        0        0    21489 2023-07-06 19:05:30.052939 rasa-3.7.0b1/README.md
+-rw-r--r--   0        0        0     9566 2023-07-06 19:05:30.284940 rasa-3.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/__init__.py
+-rw-r--r--   0        0        0     5441 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/__main__.py
+-rw-r--r--   0        0        0     5314 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/api.py
+-rw-r--r--   0        0        0      115 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/data.py
+-rw-r--r--   0        0        0     5242 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/default_arguments.py
+-rw-r--r--   0        0        0     2199 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/evaluate.py
+-rw-r--r--   0        0        0     1499 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/export.py
+-rw-r--r--   0        0        0     2685 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/interactive.py
+-rw-r--r--   0        0        0     5674 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/run.py
+-rw-r--r--   0        0        0      367 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/shell.py
+-rw-r--r--   0        0        0     6853 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/test.py
+-rw-r--r--   0        0        0     8279 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/train.py
+-rw-r--r--   0        0        0      861 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/visualize.py
+-rw-r--r--   0        0        0     1027 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/x.py
+-rw-r--r--   0        0        0     9722 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/data.py
+-rw-r--r--   0        0        0     7948 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/evaluate.py
+-rw-r--r--   0        0        0     8204 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/export.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/actions/actions.py
+-rw-r--r--   0        0        0     1505 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/config.yml
+-rw-r--r--   0        0        0      998 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/credentials.yml
+-rw-r--r--   0        0        0     1433 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/data/nlu.yml
+-rw-r--r--   0        0        0      244 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/data/rules.yml
+-rw-r--r--   0        0        0      542 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/data/stories.yml
+-rw-r--r--   0        0        0      565 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/domain.yml
+-rw-r--r--   0        0        0     1411 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/tests/test_stories.yml
+-rw-r--r--   0        0        0     5943 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/interactive.py
+-rw-r--r--   0        0        0     4196 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/run.py
+-rw-r--r--   0        0        0     6846 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/scaffold.py
+-rw-r--r--   0        0        0     4264 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/shell.py
+-rw-r--r--   0        0        0     3118 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/telemetry.py
+-rw-r--r--   0        0        0     8888 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/test.py
+-rw-r--r--   0        0        0     7798 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/train.py
+-rw-r--r--   0        0        0    12508 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/cli/utils.py
+-rw-r--r--   0        0        0     1256 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/cli/visualize.py
+-rw-r--r--   0        0        0     6785 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/cli/x.py
+-rw-r--r--   0        0        0     1172 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/constants.py
+-rw-r--r--   0        0        0      123 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/__init__.py
+-rw-r--r--   0        0        0    48450 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/action.py
+-rw-r--r--   0        0        0       78 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/constants.py
+-rw-r--r--   0        0        0    26651 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/forms.py
+-rw-r--r--   0        0        0     3401 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/loops.py
+-rw-r--r--   0        0        0     6078 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/two_stage_fallback.py
+-rw-r--r--   0        0        0    20445 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/agent.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/broker.py
+-rw-r--r--   0        0        0     1801 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/file.py
+-rw-r--r--   0        0        0    12002 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/kafka.py
+-rw-r--r--   0        0        0    14160 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/pika.py
+-rw-r--r--   0        0        0     2754 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/sql.py
+-rw-r--r--   0        0        0     1656 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/__init__.py
+-rw-r--r--   0        0        0    11669 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/botframework.py
+-rw-r--r--   0        0        0     2746 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/callback.py
+-rw-r--r--   0        0        0    13331 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/channel.py
+-rw-r--r--   0        0        0     8073 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/console.py
+-rw-r--r--   0        0        0    15812 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/facebook.py
+-rw-r--r--   0        0        0    11560 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/hangouts.py
+-rw-r--r--   0        0        0     7743 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/mattermost.py
+-rw-r--r--   0        0        0     4814 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/rasa_chat.py
+-rw-r--r--   0        0        0     6949 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/rest.py
+-rw-r--r--   0        0        0     5999 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/rocketchat.py
+-rw-r--r--   0        0        0    24405 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/slack.py
+-rw-r--r--   0        0        0    10163 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/socketio.py
+-rw-r--r--   0        0        0    10630 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/telegram.py
+-rw-r--r--   0        0        0     5938 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/twilio.py
+-rw-r--r--   0        0        0    13181 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/twilio_voice.py
+-rw-r--r--   0        0        0     4845 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/webexteams.py
+-rw-r--r--   0        0        0     3047 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/constants.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     9154 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker.py
+-rw-r--r--   0        0        0    38043 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker_base.py
+-rw-r--r--   0        0        0    12086 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker_stats.py
+-rw-r--r--   0        0        0     3658 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker_tracker_loader.py
+-rw-r--r--   0        0        0      901 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/exceptions.py
+-rw-r--r--   0        0        0    10220 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/exporter.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/featurizers/__init__.py
+-rw-r--r--   0        0        0    17964 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/featurizers/precomputation.py
+-rw-r--r--   0        0        0    15447 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/featurizers/single_state_featurizer.py
+-rw-r--r--   0        0        0    43363 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/featurizers/tracker_featurizers.py
+-rw-r--r--   0        0        0     3024 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/http_interpreter.py
+-rw-r--r--   0        0        0     2018 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/jobs.py
+-rw-r--r--   0        0        0     4719 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/lock.py
+-rw-r--r--   0        0        0    11678 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/lock_store.py
+-rw-r--r--   0        0        0    14821 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/migrate.py
+-rw-r--r--   0        0        0      240 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/__init__.py
+-rw-r--r--   0        0        0     3870 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/callback.py
+-rw-r--r--   0        0        0     3285 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/generator.py
+-rw-r--r--   0        0        0     2635 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/interpolator.py
+-rw-r--r--   0        0        0     7503 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/response.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/__init__.py
+-rw-r--r--   0        0        0    12959 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/ensemble.py
+-rw-r--r--   0        0        0    19295 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/memoization.py
+-rw-r--r--   0        0        0    25038 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/policy.py
+-rw-r--r--   0        0        0    50315 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/rule_policy.py
+-rw-r--r--   0        0        0    86521 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/ted_policy.py
+-rw-r--r--   0        0        0    39329 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/unexpected_intent_policy.py
+-rw-r--r--   0        0        0    41906 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/processor.py
+-rw-r--r--   0        0        0     9243 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/run.py
+-rw-r--r--   0        0        0    48935 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/test.py
+-rw-r--r--   0        0        0    58040 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/tracker_store.py
+-rw-r--r--   0        0        0     3543 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/train.py
+-rw-r--r--   0        0        0     3218 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/converters/__init__.py
+-rw-r--r--   0        0        0     3889 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/converters/responses_prefix_converter.py
+-rw-r--r--   0        0        0    59595 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/interactive.py
+-rw-r--r--   0        0        0    13604 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/training/story_conflict.py
+-rw-r--r--   0        0        0     3067 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/training/training.py
+-rw-r--r--   0        0        0    10995 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/visualize.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/__init__.py
+-rw-r--r--   0        0        0    16744 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/caching.py
+-rw-r--r--   0        0        0      469 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/constants.py
+-rw-r--r--   0        0        0      437 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/exceptions.py
+-rw-r--r--   0        0        0    22105 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/graph.py
+-rw-r--r--   0        0        0     1384 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/loader.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/__init__.py
+-rw-r--r--   0        0        0     1139 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/config_files/default_config.yml
+-rw-r--r--   0        0        0     3244 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/default_components.py
+-rw-r--r--   0        0        0    43587 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/default_recipe.py
+-rw-r--r--   0        0        0     3301 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/graph_recipe.py
+-rw-r--r--   0        0        0     3354 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/recipe.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/runner/__init__.py
+-rw-r--r--   0        0        0     4302 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/runner/dask.py
+-rw-r--r--   0        0        0     1672 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/runner/interface.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/__init__.py
+-rw-r--r--   0        0        0     9581 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/local_model_storage.py
+-rw-r--r--   0        0        0     3931 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/resource.py
+-rw-r--r--   0        0        0     6923 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/__init__.py
+-rw-r--r--   0        0        0     6524 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/components.py
+-rw-r--r--   0        0        0     1848 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/fingerprinting.py
+-rw-r--r--   0        0        0    10516 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/graph_trainer.py
+-rw-r--r--   0        0        0     5036 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/hooks.py
+-rw-r--r--   0        0        0    22697 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/validation.py
+-rw-r--r--   0        0        0     2132 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/converters/__init__.py
+-rw-r--r--   0        0        0     1576 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/converters/nlu_message_converter.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/domain_for_core_training_provider.py
+-rw-r--r--   0        0        0     2571 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/domain_provider.py
+-rw-r--r--   0        0        0     1294 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/forms_provider.py
+-rw-r--r--   0        0        0     2119 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/nlu_training_data_provider.py
+-rw-r--r--   0        0        0     1354 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/responses_provider.py
+-rw-r--r--   0        0        0     1540 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/rule_only_provider.py
+-rw-r--r--   0        0        0     1466 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/story_graph_provider.py
+-rw-r--r--   0        0        0     1965 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/training_tracker_provider.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/validators/__init__.py
+-rw-r--r--   0        0        0    22668 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/validators/default_recipe_validator.py
+-rw-r--r--   0        0        0    12863 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/validators/finetuning_validator.py
+-rw-r--r--   0        0        0     1782 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/jupyter.py
+-rw-r--r--   0        0        0      101 2023-07-06 19:05:53.169073 rasa-3.7.0b1/rasa/keys
+-rw-r--r--   0        0        0     3490 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/model.py
+-rw-r--r--   0        0        0    14961 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/model_testing.py
+-rw-r--r--   0        0        0    16836 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/model_training.py
+-rw-r--r--   0        0        0      123 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/nlu/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/nlu/classifiers/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/nlu/classifiers/classifier.py
+-rw-r--r--   0        0        0    71637 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/diet_classifier.py
+-rw-r--r--   0        0        0     7150 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/fallback_classifier.py
+-rw-r--r--   0        0        0     7581 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/keyword_intent_classifier.py
+-rw-r--r--   0        0        0     7568 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0        0        0     5559 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/mitie_intent_classifier.py
+-rw-r--r--   0        0        0     1989 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/regex_message_handler.py
+-rw-r--r--   0        0        0    11915 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/sklearn_intent_classifier.py
+-rw-r--r--   0        0        0     2757 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/constants.py
+-rw-r--r--   0        0        0     1317 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/convert.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/__init__.py
+-rw-r--r--   0        0        0     1748 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/dialogflow.py
+-rw-r--r--   0        0        0     1367 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/emulator.py
+-rw-r--r--   0        0        0     3032 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/luis.py
+-rw-r--r--   0        0        0      334 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/no_emulator.py
+-rw-r--r--   0        0        0     1930 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/wit.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/__init__.py
+-rw-r--r--   0        0        0    26499 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/crf_entity_extractor.py
+-rw-r--r--   0        0        0     7685 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/duckling_entity_extractor.py
+-rw-r--r--   0        0        0     7160 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/entity_synonyms.py
+-rw-r--r--   0        0        0    17530 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/extractor.py
+-rw-r--r--   0        0        0    10973 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/mitie_entity_extractor.py
+-rw-r--r--   0        0        0     8289 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/regex_entity_extractor.py
+-rw-r--r--   0        0        0     3366 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/spacy_entity_extractor.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/__init__.py
+-rw-r--r--   0        0        0    17142 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
+-rw-r--r--   0        0        0     2433 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
+-rw-r--r--   0        0        0    30361 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
+-rw-r--r--   0        0        0     5861 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
+-rw-r--r--   0        0        0     4888 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
+-rw-r--r--   0        0        0     3347 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/featurizer.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/__init__.py
+-rw-r--r--   0        0        0    33295 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
+-rw-r--r--   0        0        0    21810 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
+-rw-r--r--   0        0        0    10289 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
+-rw-r--r--   0        0        0      220 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
+-rw-r--r--   0        0        0      557 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/model.py
+-rw-r--r--   0        0        0     8333 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/persistor.py
+-rw-r--r--   0        0        0      803 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/run.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/selectors/__init__.py
+-rw-r--r--   0        0        0    39012 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/selectors/response_selector.py
+-rw-r--r--   0        0        0    67726 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/test.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5374 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/jieba_tokenizer.py
+-rw-r--r--   0        0        0     2618 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/mitie_tokenizer.py
+-rw-r--r--   0        0        0     2378 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0        0        0     8196 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3750 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      928 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/__init__.py
+-rw-r--r--   0        0        0    14703 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/bilou_utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/hugging_face/registry.py
+-rw-r--r--   0        0        0     9143 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
+-rw-r--r--   0        0        0     3887 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/mitie_utils.py
+-rw-r--r--   0        0        0     5386 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/pattern_utils.py
+-rw-r--r--   0        0        0    11795 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/spacy_utils.py
+-rw-r--r--   0        0        0     4921 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/plugin.py
+-rw-r--r--   0        0        0    55589 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/server.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/__init__.py
+-rw-r--r--   0        0        0     4337 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/__init__.py
+-rw-r--r--   0        0        0     4416 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/constants.py
+-rw-r--r--   0        0        0     1366 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/conversation.py
+-rw-r--r--   0        0        0    77445 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/domain.py
+-rw-r--r--   0        0        0    66276 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/events.py
+-rw-r--r--   0        0        0    35597 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/generator.py
+-rw-r--r--   0        0        0     8286 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/slot_mappings.py
+-rw-r--r--   0        0        0    16371 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/slots.py
+-rw-r--r--   0        0        0    34744 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/trackers.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/__init__.py
+-rw-r--r--   0        0        0     2895 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/loading.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/__init__.py
+-rw-r--r--   0        0        0     4449 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_reader.py
+-rw-r--r--   0        0        0     6671 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_step_builder.py
+-rw-r--r--   0        0        0    32976 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/__init__.py
+-rw-r--r--   0        0        0     2543 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/story_writer.py
+-rw-r--r--   0        0        0    14903 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
+-rw-r--r--   0        0        0    29313 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/structures.py
+-rw-r--r--   0        0        0     3500 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/visualization.html
+-rw-r--r--   0        0        0    20341 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/visualization.py
+-rw-r--r--   0        0        0     5479 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/data.py
+-rw-r--r--   0        0        0     3633 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/__init__.py
+-rw-r--r--   0        0        0    21866 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/importer.py
+-rw-r--r--   0        0        0     7836 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/multi_project.py
+-rw-r--r--   0        0        0     3388 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/rasa.py
+-rw-r--r--   0        0        0      861 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/constants.py
+-rw-r--r--   0        0        0      188 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/interpreter.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/__init__.py
+-rw-r--r--   0        0        0     6759 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/entities_parser.py
+-rw-r--r--   0        0        0    14835 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/features.py
+-rw-r--r--   0        0        0      453 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/__init__.py
+-rw-r--r--   0        0        0     6123 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/dialogflow.py
+-rw-r--r--   0        0        0     3014 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/luis.py
+-rw-r--r--   0        0        0     4495 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa.py
+-rw-r--r--   0        0        0    22353 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa_yaml.py
+-rw-r--r--   0        0        0     8540 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/readerwriter.py
+-rw-r--r--   0        0        0     1820 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/wit.py
+-rw-r--r--   0        0        0     4258 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/loading.py
+-rw-r--r--   0        0        0     1116 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/lookup_tables_parser.py
+-rw-r--r--   0        0        0    16662 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/message.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/__init__.py
+-rw-r--r--   0        0        0     2565 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/data_schema.py
+-rw-r--r--   0        0        0     1179 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/nlu.yml
+-rw-r--r--   0        0        0     1661 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/responses.yml
+-rw-r--r--   0        0        0     1476 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/synonyms_parser.py
+-rw-r--r--   0        0        0    28493 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/training_data.py
+-rw-r--r--   0        0        0     7040 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/util.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/cli.py
+-rw-r--r--   0        0        0     8731 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/common.py
+-rw-r--r--   0        0        0    20533 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/io.py
+-rw-r--r--   0        0        0      883 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/pykwalify_extensions.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/config.yml
+-rw-r--r--   0        0        0     3267 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/domain.yml
+-rw-r--r--   0        0        0     5569 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/events.py
+-rw-r--r--   0        0        0      998 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/model_config.yml
+-rw-r--r--   0        0        0     4034 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/stories.yml
+-rw-r--r--   0        0        0    10317 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/validation.py
+-rw-r--r--   0        0        0    36273 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/telemetry.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/__init__.py
+-rw-r--r--   0        0        0    19532 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/common.py
+-rw-r--r--   0        0        0     1647 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/converter.py
+-rw-r--r--   0        0        0     8796 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/endpoints.py
+-rw-r--r--   0        0        0     7831 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/io.py
+-rw-r--r--   0        0        0     2018 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/llm.py
+-rw-r--r--   0        0        0     4482 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/log_utils.py
+-rw-r--r--   0        0        0    12246 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/plotting.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/callback.py
+-rw-r--r--   0        0        0     3140 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/constants.py
+-rw-r--r--   0        0        0    19658 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/crf.py
+-rw-r--r--   0        0        0    15526 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/data_generator.py
+-rw-r--r--   0        0        0     5576 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/environment.py
+-rw-r--r--   0        0        0      168 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/exceptions.py
+-rw-r--r--   0        0        0    59263 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/layers.py
+-rw-r--r--   0        0        0     3319 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/layers_utils.py
+-rw-r--r--   0        0        0    10055 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/metrics.py
+-rw-r--r--   0        0        0    34572 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/model_data.py
+-rw-r--r--   0        0        0    18667 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/model_data_utils.py
+-rw-r--r--   0        0        0    36004 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/models.py
+-rw-r--r--   0        0        0    49066 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/rasa_layers.py
+-rw-r--r--   0        0        0    25509 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/transformer.py
+-rw-r--r--   0        0        0      204 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/types.py
+-rw-r--r--   0        0        0    20999 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/train_utils.py
+-rw-r--r--   0        0        0    17708 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/validator.py
+-rw-r--r--   0        0        0      118 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/version.py
+-rw-r--r--   0        0        0    28128 1970-01-01 00:00:00.000000 rasa-3.7.0b1/PKG-INFO
```

### Comparing `rasa-3.6.2/LICENSE.txt` & `rasa-3.7.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/README.md` & `rasa-3.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/pyproject.toml` & `rasa-3.7.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa"
-version = "3.6.2"
+version = "3.7.0b1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -86,36 +86,36 @@
 line-length = 88
 select = [ "D", "E", "F", "W", "RUF",]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 boto3 = "^1.26.136"
 requests = "^2.23"
-matplotlib = ">=3.1,<3.6"
+matplotlib = ">=3.1,<3.8"
 attrs = ">=19.3,<22.2"
 jsonpickle = ">=1.3,<3.1"
 redis = ">=4.5.3, <5.0"
 absl-py = ">=0.9,<1.5"
 apscheduler = ">=3.6,<3.10"
 tqdm = "^4.31"
 networkx = ">=2.4,<2.7"
 fbmessenger = "~6.0.0"
 pykwalify = ">=1.7,<1.9"
 coloredlogs = ">=10,<16"
 "ruamel.yaml" = ">=0.16.5,<0.17.22"
 pyyaml = ">=5.3.1,<6.0"
-twilio = ">=6.26,<8.3"
+twilio = ">=6.26,<8.4"
 webexteamssdk = ">=1.1.1,<1.7.0"
 mattermostwrapper = "~2.2"
 rocketchat_API = ">=0.6.31,<1.31.0"
 colorhash = ">=1.0.2,<1.3.0"
 jsonschema = ">=3.2,<4.18"
 packaging = ">=20.0,<21.0"
 pytz = ">=2019.1,<2023.0"
-rasa-sdk = "~3.6.0"
+rasa-sdk = "~3.7.0b1"
 colorclass = "~2.2"
 terminaltables = "~3.1.0"
 sanic = "~21.12"
 sanic-cors = "~2.0.0"
 sanic-jwt = "^1.6.0"
 sanic-routing = "^0.7.2"
 websockets = ">=10.0,<11.0"
@@ -137,15 +137,15 @@
 regex = ">=2020.6,<2022.11"
 joblib = ">=0.15.1,<1.3.0"
 sentry-sdk = ">=0.17.0,<1.15.0"
 aio-pika = ">=6.7.1,<8.2.4"
 aiogram = "<2.26"
 typing-extensions = ">=4.1.1,<5.0.0"
 typing-utils = "^0.1.0"
-tarsafe = ">=0.0.3,<0.0.5"
+tarsafe = ">=0.0.3,<0.0.6"
 google-auth = "<3"
 CacheControl = "^0.12.9"
 randomname = "^0.1.5"
 pluggy = "^1.0.0"
 slack-sdk = "^3.19.2"
 confluent-kafka = ">=1.9.2,<3.0.0"
 portalocker = "^2.7.0"
```

### Comparing `rasa-3.6.2/rasa/__main__.py` & `rasa-3.7.0b1/rasa/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/api.py` & `rasa-3.7.0b1/rasa/api.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/data.py` & `rasa-3.7.0b1/rasa/cli/arguments/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/default_arguments.py` & `rasa-3.7.0b1/rasa/cli/arguments/default_arguments.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/evaluate.py` & `rasa-3.7.0b1/rasa/cli/arguments/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/export.py` & `rasa-3.7.0b1/rasa/cli/arguments/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/interactive.py` & `rasa-3.7.0b1/rasa/cli/arguments/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/run.py` & `rasa-3.7.0b1/rasa/cli/arguments/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/test.py` & `rasa-3.7.0b1/rasa/cli/arguments/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/train.py` & `rasa-3.7.0b1/rasa/cli/arguments/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/visualize.py` & `rasa-3.7.0b1/rasa/cli/arguments/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/arguments/x.py` & `rasa-3.7.0b1/rasa/cli/arguments/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/data.py` & `rasa-3.7.0b1/rasa/cli/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/evaluate.py` & `rasa-3.7.0b1/rasa/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/export.py` & `rasa-3.7.0b1/rasa/cli/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/actions/actions.py` & `rasa-3.7.0b1/rasa/cli/initial_project/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/config.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/credentials.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/credentials.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/data/nlu.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/data/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/data/stories.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/data/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/domain.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/endpoints.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/endpoints.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/initial_project/tests/test_stories.yml` & `rasa-3.7.0b1/rasa/cli/initial_project/tests/test_stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/interactive.py` & `rasa-3.7.0b1/rasa/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/run.py` & `rasa-3.7.0b1/rasa/cli/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/scaffold.py` & `rasa-3.7.0b1/rasa/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/shell.py` & `rasa-3.7.0b1/rasa/cli/shell.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/telemetry.py` & `rasa-3.7.0b1/rasa/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/test.py` & `rasa-3.7.0b1/rasa/cli/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/train.py` & `rasa-3.7.0b1/rasa/cli/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/utils.py` & `rasa-3.7.0b1/rasa/cli/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/visualize.py` & `rasa-3.7.0b1/rasa/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/cli/x.py` & `rasa-3.7.0b1/rasa/cli/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/constants.py` & `rasa-3.7.0b1/rasa/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/actions/action.py` & `rasa-3.7.0b1/rasa/core/actions/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     UTTER_PREFIX,
 )
 from rasa.shared.core import events
 from rasa.shared.core.constants import (
     USER_INTENT_OUT_OF_SCOPE,
     ACTION_LISTEN_NAME,
     ACTION_RESTART_NAME,
+    ACTION_SEND_TEXT_NAME,
     ACTION_SESSION_START_NAME,
     ACTION_DEFAULT_FALLBACK_NAME,
     ACTION_DEACTIVATE_LOOP_NAME,
     ACTION_REVERT_FALLBACK_EVENTS_NAME,
     ACTION_DEFAULT_ASK_AFFIRMATION_NAME,
     ACTION_DEFAULT_ASK_REPHRASE_NAME,
     ACTION_UNLIKELY_INTENT_NAME,
@@ -104,14 +105,15 @@
         ActionDefaultFallback(),
         ActionDeactivateLoop(),
         ActionRevertFallbackEvents(),
         ActionDefaultAskAffirmation(),
         ActionDefaultAskRephrase(),
         TwoStageFallbackAction(action_endpoint),
         ActionUnlikelyIntent(),
+        ActionSendText(),
         ActionBack(),
         ActionExtractSlots(action_endpoint),
     ]
 
 
 def action_for_index(
     index: int, domain: Domain, action_endpoint: Optional[EndpointConfig]
@@ -239,14 +241,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Execute the side effects of this action.
 
         Args:
             nlg: which ``nlg`` to use for response generation
             output_channel: ``output_channel`` to which to send the resulting message.
             tracker (DialogueStateTracker): the state tracker for the current
@@ -300,14 +303,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Simple run implementation uttering a (hopefully defined) response."""
         response_ids_for_response = domain.response_ids_per_response.get(
             self.utter_action, set()
         )
 
         response_id_list = list(response_ids_for_response)
@@ -358,14 +362,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action (see parent class for full docstring)."""
         message = {"text": self.action_text}
         return [create_bot_utterance(message)]
 
     def event_for_successful_execution(
         self, prediction: PolicyPrediction
@@ -446,14 +451,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Query the appropriate response and create a bot utterance with that."""
         latest_message = tracker.latest_message
 
         if latest_message is None:
             return []
 
@@ -506,14 +512,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         # only utter the response if it is available
         evts = await super().run(output_channel, nlg, tracker, domain)
 
         return evts + [UserUtteranceReverted(), UserUtteranceReverted()]
 
@@ -531,14 +538,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         return []
 
 
 class ActionRestart(ActionBotResponse):
     """Resets the tracker to its initial state.
@@ -556,14 +564,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         # only utter the response if it is available
         evts = await super().run(output_channel, nlg, tracker, domain)
 
         return evts + [Restarted()]
 
@@ -592,14 +601,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         _events: List[Event] = [SessionStarted()]
 
         if domain.session_config.carry_over_slots:
             _events.extend(self._slot_set_events_from_tracker(tracker))
 
@@ -621,14 +631,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         # only utter the response if it is available
         evts = await super().run(output_channel, nlg, tracker, domain)
 
         return evts + [UserUtteranceReverted()]
 
@@ -641,14 +652,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         return [ActiveLoop(None), SlotSet(REQUESTED_SLOT, None)]
 
 
 class RemoteAction(Action):
     def __init__(self, name: Text, action_endpoint: Optional[EndpointConfig]) -> None:
@@ -755,14 +767,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         json_body = self._action_call_format(tracker, domain)
         if not self.action_endpoint:
             raise RasaException(
                 f"Failed to execute custom action '{self.name()}' "
                 f"because no endpoint is configured to run this "
@@ -881,14 +894,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         from rasa.core.policies.two_stage_fallback import has_user_rephrased
 
         # User rephrased
         if has_user_rephrased(tracker):
             return _revert_successful_rephrasing(tracker)
@@ -911,14 +925,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         return []
 
 
 def has_user_affirmed(tracker: "DialogueStateTracker") -> bool:
     """Indicates if the last executed action is `action_default_ask_affirmation`."""
@@ -991,14 +1006,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         latest_message = tracker.latest_message
         if latest_message is None:
             raise TypeError(
                 "Cannot find last user message for detecting fallback affirmation."
             )
@@ -1039,14 +1055,35 @@
         return ACTION_DEFAULT_ASK_REPHRASE_NAME
 
     def __init__(self) -> None:
         """Initializes action default ask rephrase."""
         super().__init__("utter_ask_rephrase", silent_fail=True)
 
 
+class ActionSendText(Action):
+    """Sends a text message to the output channel."""
+
+    def name(self) -> Text:
+        return ACTION_SEND_TEXT_NAME
+
+    async def run(
+        self,
+        output_channel: "OutputChannel",
+        nlg: "NaturalLanguageGenerator",
+        tracker: "DialogueStateTracker",
+        domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
+    ) -> List[Event]:
+        """Runs action. Please see parent class for the full docstring."""
+
+        fallback = {"text": ""}
+        message = metadata.get("message", fallback) if metadata else fallback
+        return [create_bot_utterance(message)]
+
+
 class ActionExtractSlots(Action):
     """Default action that runs after each user turn.
 
     Action is executed automatically in MessageProcessor.handle_message(...)
     before the next predicted action is run.
 
     Set slots to extracted values from user message
@@ -1238,14 +1275,15 @@
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         """Runs action. Please see parent class for the full docstring."""
         slot_events: List[Event] = []
         executed_custom_actions: Set[Text] = set()
 
         user_slots = [
             slot for slot in domain.slots if slot.name not in DEFAULT_SLOT_NAMES
@@ -1319,14 +1357,24 @@
 
 def extract_slot_value_from_predefined_mapping(
     mapping_type: SlotMappingType,
     mapping: Dict[Text, Any],
     tracker: "DialogueStateTracker",
 ) -> List[Any]:
     """Extracts slot value if slot has an applicable predefined mapping."""
+
+    if tracker.has_bot_message_after_latest_user_message():
+        # TODO: this needs further validation - not sure if this breaks something!!!
+
+        # If the bot sent a message after the user sent a message, we can't
+        # extract any slots from the user message. We assume that the user
+        # message was already processed by the bot and the slot value was
+        # already extracted (e.g. for a prior form slot).
+        return []
+
     should_fill_entity_slot = (
         mapping_type == SlotMappingType.FROM_ENTITY
         and SlotMapping.entity_is_desired(mapping, tracker)
     )
 
     should_fill_intent_slot = mapping_type == SlotMappingType.FROM_INTENT
```

### Comparing `rasa-3.6.2/rasa/core/actions/forms.py` & `rasa-3.7.0b1/rasa/core/actions/forms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/actions/loops.py` & `rasa-3.7.0b1/rasa/core/actions/loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import List, TYPE_CHECKING
+from typing import Any, Dict, List, TYPE_CHECKING, Optional, Text
 
 from rasa.core.actions.action import Action
 from rasa.shared.core.events import Event, ActiveLoop
 
 if TYPE_CHECKING:
     from rasa.core.channels import OutputChannel
     from rasa.shared.core.domain import Domain
@@ -14,14 +14,15 @@
 class LoopAction(Action, ABC):
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
+        metadata: Optional[Dict[Text, Any]] = None,
     ) -> List[Event]:
         events: List[Event] = []
 
         if not await self.is_activated(output_channel, nlg, tracker, domain):
             events += await self._activate_loop(
                 output_channel,
                 nlg,
```

### Comparing `rasa-3.6.2/rasa/core/actions/two_stage_fallback.py` & `rasa-3.7.0b1/rasa/core/actions/two_stage_fallback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/agent.py` & `rasa-3.7.0b1/rasa/core/agent.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/brokers/broker.py` & `rasa-3.7.0b1/rasa/core/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/brokers/file.py` & `rasa-3.7.0b1/rasa/core/brokers/file.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/brokers/kafka.py` & `rasa-3.7.0b1/rasa/core/brokers/kafka.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/brokers/pika.py` & `rasa-3.7.0b1/rasa/core/brokers/pika.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/brokers/sql.py` & `rasa-3.7.0b1/rasa/core/brokers/sql.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/__init__.py` & `rasa-3.7.0b1/rasa/core/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/botframework.py` & `rasa-3.7.0b1/rasa/core/channels/botframework.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/callback.py` & `rasa-3.7.0b1/rasa/core/channels/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/channel.py` & `rasa-3.7.0b1/rasa/core/channels/channel.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/console.py` & `rasa-3.7.0b1/rasa/core/channels/console.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/facebook.py` & `rasa-3.7.0b1/rasa/core/channels/facebook.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/hangouts.py` & `rasa-3.7.0b1/rasa/core/channels/hangouts.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/mattermost.py` & `rasa-3.7.0b1/rasa/core/channels/mattermost.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/rasa_chat.py` & `rasa-3.7.0b1/rasa/core/channels/rasa_chat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/rest.py` & `rasa-3.7.0b1/rasa/core/channels/rest.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/rocketchat.py` & `rasa-3.7.0b1/rasa/core/channels/rocketchat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/slack.py` & `rasa-3.7.0b1/rasa/core/channels/slack.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/socketio.py` & `rasa-3.7.0b1/rasa/core/channels/socketio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/telegram.py` & `rasa-3.7.0b1/rasa/core/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/twilio.py` & `rasa-3.7.0b1/rasa/core/channels/twilio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/twilio_voice.py` & `rasa-3.7.0b1/rasa/core/channels/twilio_voice.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/channels/webexteams.py` & `rasa-3.7.0b1/rasa/core/channels/webexteams.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/constants.py` & `rasa-3.7.0b1/rasa/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/evaluation/marker.py` & `rasa-3.7.0b1/rasa/core/evaluation/marker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/evaluation/marker_base.py` & `rasa-3.7.0b1/rasa/core/evaluation/marker_base.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/evaluation/marker_stats.py` & `rasa-3.7.0b1/rasa/core/evaluation/marker_stats.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/evaluation/marker_tracker_loader.py` & `rasa-3.7.0b1/rasa/core/evaluation/marker_tracker_loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/exceptions.py` & `rasa-3.7.0b1/rasa/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/exporter.py` & `rasa-3.7.0b1/rasa/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/featurizers/precomputation.py` & `rasa-3.7.0b1/rasa/core/featurizers/precomputation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/featurizers/single_state_featurizer.py` & `rasa-3.7.0b1/rasa/core/featurizers/single_state_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/featurizers/tracker_featurizers.py` & `rasa-3.7.0b1/rasa/core/featurizers/tracker_featurizers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/http_interpreter.py` & `rasa-3.7.0b1/rasa/core/http_interpreter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/jobs.py` & `rasa-3.7.0b1/rasa/core/jobs.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/lock.py` & `rasa-3.7.0b1/rasa/core/lock.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/lock_store.py` & `rasa-3.7.0b1/rasa/core/lock_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/migrate.py` & `rasa-3.7.0b1/rasa/core/migrate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/nlg/callback.py` & `rasa-3.7.0b1/rasa/core/nlg/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/nlg/generator.py` & `rasa-3.7.0b1/rasa/core/nlg/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/nlg/interpolator.py` & `rasa-3.7.0b1/rasa/core/nlg/interpolator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/nlg/response.py` & `rasa-3.7.0b1/rasa/core/nlg/response.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/policies/ensemble.py` & `rasa-3.7.0b1/rasa/core/policies/ensemble.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/policies/memoization.py` & `rasa-3.7.0b1/rasa/core/policies/memoization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/policies/policy.py` & `rasa-3.7.0b1/rasa/core/policies/policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/policies/rule_policy.py` & `rasa-3.7.0b1/rasa/core/policies/rule_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/policies/ted_policy.py` & `rasa-3.7.0b1/rasa/core/policies/ted_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/policies/unexpected_intent_policy.py` & `rasa-3.7.0b1/rasa/core/policies/unexpected_intent_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/processor.py` & `rasa-3.7.0b1/rasa/core/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import copy
 import logging
 import structlog
 import os
 from pathlib import Path
 import tarfile
 import time
@@ -58,21 +59,25 @@
 from rasa.core.nlg import NaturalLanguageGenerator
 from rasa.core.lock_store import LockStore
 from rasa.utils.common import TempDirectoryPath, get_temp_dir_name
 import rasa.core.tracker_store
 import rasa.core.actions.action
 import rasa.shared.core.trackers
 from rasa.shared.core.trackers import DialogueStateTracker, EventVerbosity
+from rasa.shared.core.training_data.story_reader.yaml_story_reader import (
+    YAMLStoryReader,
+)
 from rasa.shared.nlu.constants import (
     ENTITIES,
     INTENT,
     INTENT_NAME_KEY,
     PREDICTED_CONFIDENCE_KEY,
     TEXT,
 )
+from rasa.shared.nlu.training_data.message import Message
 from rasa.utils.endpoints import EndpointConfig
 
 logger = logging.getLogger(__name__)
 structlogger = structlog.get_logger()
 
 MAX_NUMBER_OF_PREDICTIONS = int(os.environ.get("MAX_NUMBER_OF_PREDICTIONS", "10"))
 
@@ -711,19 +716,31 @@
 
         Returns:
             Parsed data extracted from the message.
         """
         if self.http_interpreter:
             parse_data = await self.http_interpreter.parse(message)
         else:
-            if tracker is None:
-                tracker = DialogueStateTracker.from_events(message.sender_id, [])
-            parse_data = self._parse_message_with_graph(
-                message, tracker, only_output_properties
+            msg = YAMLStoryReader.unpack_regex_message(
+                message=Message({TEXT: message.text})
             )
+            # Intent is not explicitly present. Pass message to graph.
+            if msg.data.get(INTENT) is None:
+                parse_data = self._parse_message_with_graph(
+                    message, tracker, only_output_properties
+                )
+            else:
+                parse_data = {
+                    TEXT: "",
+                    INTENT: {INTENT_NAME_KEY: None, PREDICTED_CONFIDENCE_KEY: 0.0},
+                    ENTITIES: [],
+                }
+                parse_data.update(
+                    msg.as_dict(only_output_properties=only_output_properties)
+                )
 
         structlogger.debug(
             "processor.message.parse",
             parse_data_text=copy.deepcopy(parse_data["text"]),
             parse_data_intent=parse_data["intent"],
             parse_data_entities=copy.deepcopy(parse_data["entities"]),
         )
@@ -731,15 +748,15 @@
         self._check_for_unseen_features(parse_data)
 
         return parse_data
 
     def _parse_message_with_graph(
         self,
         message: UserMessage,
-        tracker: DialogueStateTracker,
+        tracker: Optional[DialogueStateTracker] = None,
         only_output_properties: bool = True,
     ) -> Dict[Text, Any]:
         """Interprets the passed message.
 
         Arguments:
             message: Message to handle
             tracker: Tracker to use
@@ -953,17 +970,28 @@
         # events and return values are used to update
         # the tracker state after an action has been taken
         try:
             # Use temporary tracker as we might need to discard the policy events in
             # case of a rejection.
             temporary_tracker = tracker.copy()
             temporary_tracker.update_with_events(prediction.events, self.domain)
-            events = await action.run(
-                output_channel, nlg, temporary_tracker, self.domain
-            )
+
+            run_args = inspect.getfullargspec(action.run).args
+            if "metadata" in run_args:
+                events = await action.run(
+                    output_channel,
+                    nlg,
+                    temporary_tracker,
+                    self.domain,
+                    metadata=prediction.action_metadata,
+                )
+            else:
+                events = await action.run(
+                    output_channel, nlg, temporary_tracker, self.domain
+                )
         except rasa.core.actions.action.ActionExecutionRejection:
             events = [
                 ActionExecutionRejected(
                     action.name(), prediction.policy_name, prediction.max_confidence
                 )
             ]
             tracker.update(events[0])
```

### Comparing `rasa-3.6.2/rasa/core/run.py` & `rasa-3.7.0b1/rasa/core/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/test.py` & `rasa-3.7.0b1/rasa/core/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/tracker_store.py` & `rasa-3.7.0b1/rasa/core/tracker_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/train.py` & `rasa-3.7.0b1/rasa/core/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/training/__init__.py` & `rasa-3.7.0b1/rasa/core/training/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/training/converters/responses_prefix_converter.py` & `rasa-3.7.0b1/rasa/core/training/converters/responses_prefix_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/training/interactive.py` & `rasa-3.7.0b1/rasa/core/training/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/training/story_conflict.py` & `rasa-3.7.0b1/rasa/core/training/story_conflict.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/training/training.py` & `rasa-3.7.0b1/rasa/core/training/training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/utils.py` & `rasa-3.7.0b1/rasa/core/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/core/visualize.py` & `rasa-3.7.0b1/rasa/core/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/caching.py` & `rasa-3.7.0b1/rasa/engine/caching.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/graph.py` & `rasa-3.7.0b1/rasa/engine/graph.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/loader.py` & `rasa-3.7.0b1/rasa/engine/loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/recipes/config_files/default_config.yml` & `rasa-3.7.0b1/rasa/engine/recipes/config_files/default_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/recipes/default_components.py` & `rasa-3.7.0b1/rasa/engine/recipes/default_components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/recipes/default_recipe.py` & `rasa-3.7.0b1/rasa/engine/recipes/default_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/recipes/graph_recipe.py` & `rasa-3.7.0b1/rasa/engine/recipes/graph_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/recipes/recipe.py` & `rasa-3.7.0b1/rasa/engine/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/runner/dask.py` & `rasa-3.7.0b1/rasa/engine/runner/dask.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/runner/interface.py` & `rasa-3.7.0b1/rasa/engine/runner/interface.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/storage/local_model_storage.py` & `rasa-3.7.0b1/rasa/engine/storage/local_model_storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/storage/resource.py` & `rasa-3.7.0b1/rasa/engine/storage/resource.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/storage/storage.py` & `rasa-3.7.0b1/rasa/engine/storage/storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/training/components.py` & `rasa-3.7.0b1/rasa/engine/training/components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/training/fingerprinting.py` & `rasa-3.7.0b1/rasa/engine/training/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/training/graph_trainer.py` & `rasa-3.7.0b1/rasa/engine/training/graph_trainer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/training/hooks.py` & `rasa-3.7.0b1/rasa/engine/training/hooks.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/engine/validation.py` & `rasa-3.7.0b1/rasa/engine/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/exceptions.py` & `rasa-3.7.0b1/rasa/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/converters/nlu_message_converter.py` & `rasa-3.7.0b1/rasa/graph_components/converters/nlu_message_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/domain_for_core_training_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/domain_for_core_training_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/domain_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/domain_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/forms_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/forms_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/nlu_training_data_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/nlu_training_data_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/responses_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/responses_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/rule_only_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/rule_only_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/story_graph_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/story_graph_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/providers/training_tracker_provider.py` & `rasa-3.7.0b1/rasa/graph_components/providers/training_tracker_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/validators/default_recipe_validator.py` & `rasa-3.7.0b1/rasa/graph_components/validators/default_recipe_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/graph_components/validators/finetuning_validator.py` & `rasa-3.7.0b1/rasa/graph_components/validators/finetuning_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/jupyter.py` & `rasa-3.7.0b1/rasa/jupyter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/model.py` & `rasa-3.7.0b1/rasa/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/model_testing.py` & `rasa-3.7.0b1/rasa/model_testing.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/model_training.py` & `rasa-3.7.0b1/rasa/model_training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/diet_classifier.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/diet_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/fallback_classifier.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/fallback_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/keyword_intent_classifier.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/keyword_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/logistic_regression_classifier.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/mitie_intent_classifier.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/mitie_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/regex_message_handler.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/regex_message_handler.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/classifiers/sklearn_intent_classifier.py` & `rasa-3.7.0b1/rasa/nlu/classifiers/sklearn_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/constants.py` & `rasa-3.7.0b1/rasa/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/convert.py` & `rasa-3.7.0b1/rasa/nlu/convert.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/emulators/dialogflow.py` & `rasa-3.7.0b1/rasa/nlu/emulators/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/emulators/emulator.py` & `rasa-3.7.0b1/rasa/nlu/emulators/emulator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/emulators/luis.py` & `rasa-3.7.0b1/rasa/nlu/emulators/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/emulators/wit.py` & `rasa-3.7.0b1/rasa/nlu/emulators/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/crf_entity_extractor.py` & `rasa-3.7.0b1/rasa/nlu/extractors/crf_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/duckling_entity_extractor.py` & `rasa-3.7.0b1/rasa/nlu/extractors/duckling_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/entity_synonyms.py` & `rasa-3.7.0b1/rasa/nlu/extractors/entity_synonyms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/extractor.py` & `rasa-3.7.0b1/rasa/nlu/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/mitie_entity_extractor.py` & `rasa-3.7.0b1/rasa/nlu/extractors/mitie_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/regex_entity_extractor.py` & `rasa-3.7.0b1/rasa/nlu/extractors/regex_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/extractors/spacy_entity_extractor.py` & `rasa-3.7.0b1/rasa/nlu/extractors/spacy_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py` & `rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/model.py` & `rasa-3.7.0b1/rasa/nlu/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/persistor.py` & `rasa-3.7.0b1/rasa/nlu/persistor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/run.py` & `rasa-3.7.0b1/rasa/nlu/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/selectors/response_selector.py` & `rasa-3.7.0b1/rasa/nlu/selectors/response_selector.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/test.py` & `rasa-3.7.0b1/rasa/nlu/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/tokenizers/jieba_tokenizer.py` & `rasa-3.7.0b1/rasa/nlu/tokenizers/jieba_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/tokenizers/mitie_tokenizer.py` & `rasa-3.7.0b1/rasa/nlu/tokenizers/mitie_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/tokenizers/spacy_tokenizer.py` & `rasa-3.7.0b1/rasa/nlu/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/tokenizers/tokenizer.py` & `rasa-3.7.0b1/rasa/nlu/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/tokenizers/whitespace_tokenizer.py` & `rasa-3.7.0b1/rasa/nlu/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/__init__.py` & `rasa-3.7.0b1/rasa/nlu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/bilou_utils.py` & `rasa-3.7.0b1/rasa/nlu/utils/bilou_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/hugging_face/registry.py` & `rasa-3.7.0b1/rasa/nlu/utils/hugging_face/registry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py` & `rasa-3.7.0b1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/mitie_utils.py` & `rasa-3.7.0b1/rasa/nlu/utils/mitie_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/pattern_utils.py` & `rasa-3.7.0b1/rasa/nlu/utils/pattern_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/nlu/utils/spacy_utils.py` & `rasa-3.7.0b1/rasa/nlu/utils/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/plugin.py` & `rasa-3.7.0b1/rasa/plugin.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/server.py` & `rasa-3.7.0b1/rasa/server.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/constants.py` & `rasa-3.7.0b1/rasa/shared/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,7 +102,9 @@
 DEFAULT_MARKERS_OUTPUT_PATH = "markers/output"
 DEFAULT_MARKERS_STATS_PATH = "markers/stats"
 
 DIAGNOSTIC_DATA = "diagnostic_data"
 
 RESPONSE_CONDITION = "condition"
 CHANNEL = "channel"
+
+OPENAI_API_KEY_ENV_VAR = "OPENAI_API_KEY"
```

### Comparing `rasa-3.6.2/rasa/shared/core/constants.py` & `rasa-3.7.0b1/rasa/shared/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     constants.DEFAULT_NLU_FALLBACK_INTENT_NAME,
 ]
 
 LOOP_NAME = "name"
 
 ACTION_LISTEN_NAME = "action_listen"
 ACTION_RESTART_NAME = "action_restart"
+ACTION_SEND_TEXT_NAME = "action_send_text"
 ACTION_SESSION_START_NAME = "action_session_start"
 ACTION_DEFAULT_FALLBACK_NAME = "action_default_fallback"
 ACTION_DEACTIVATE_LOOP_NAME = "action_deactivate_loop"
 ACTION_REVERT_FALLBACK_EVENTS_NAME = "action_revert_fallback_events"
 ACTION_DEFAULT_ASK_AFFIRMATION_NAME = "action_default_ask_affirmation"
 ACTION_DEFAULT_ASK_REPHRASE_NAME = "action_default_ask_rephrase"
 ACTION_BACK_NAME = "action_back"
@@ -45,14 +46,15 @@
     ACTION_DEACTIVATE_LOOP_NAME,
     ACTION_REVERT_FALLBACK_EVENTS_NAME,
     ACTION_DEFAULT_ASK_AFFIRMATION_NAME,
     ACTION_DEFAULT_ASK_REPHRASE_NAME,
     ACTION_TWO_STAGE_FALLBACK_NAME,
     ACTION_UNLIKELY_INTENT_NAME,
     ACTION_BACK_NAME,
+    ACTION_SEND_TEXT_NAME,
     RULE_SNIPPET_ACTION_NAME,
     ACTION_EXTRACT_SLOTS,
 ]
 
 ACTION_SHOULD_SEND_DOMAIN = "send_domain"
 
 # rules allow setting a value of slots or active_loops to None;
```

### Comparing `rasa-3.6.2/rasa/shared/core/conversation.py` & `rasa-3.7.0b1/rasa/shared/core/conversation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/domain.py` & `rasa-3.7.0b1/rasa/shared/core/domain.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/events.py` & `rasa-3.7.0b1/rasa/shared/core/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,14 +545,22 @@
 
         return (
             f"UserUttered(text: {self.text}, intent: {self.intent_name}"
             f"{entities}"
             f", use_text_for_featurization: {self.use_text_for_featurization})"
         )
 
+    def __repr__(self) -> Text:
+        """Returns text representation of event for debugging."""
+        return (
+            f"UserUttered('{self.text}', "
+            f"'{self.intent_name}', "
+            f"{json.dumps(self.entities)})"
+        )
+
     @staticmethod
     def empty() -> "UserUttered":
         return UserUttered(None)
 
     def is_empty(self) -> bool:
         return not self.text and not self.intent_name and not self.entities
 
@@ -1731,14 +1739,18 @@
         self.name = name
         super().__init__(timestamp, metadata)
 
     def __str__(self) -> Text:
         """Returns text representation of event."""
         return f"Loop({self.name})"
 
+    def __repr__(self) -> Text:
+        """Returns event as string for debugging."""
+        return f"ActiveLoop({self.name}, {self.timestamp}, {self.metadata})"
+
     def __hash__(self) -> int:
         """Returns unique hash for event."""
         return hash(self.name)
 
     def __eq__(self, other: Any) -> bool:
         """Compares object with other object."""
         if not isinstance(other, ActiveLoop):
```

### Comparing `rasa-3.6.2/rasa/shared/core/generator.py` & `rasa-3.7.0b1/rasa/shared/core/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/slot_mappings.py` & `rasa-3.7.0b1/rasa/shared/core/slot_mappings.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/slots.py` & `rasa-3.7.0b1/rasa/shared/core/slots.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/trackers.py` & `rasa-3.7.0b1/rasa/shared/core/trackers.py`

 * *Files 5% similar despite different names*

```diff
@@ -383,14 +383,40 @@
         """Retrieves the value of a slot."""
         if key in self.slots:
             return self.slots[key].value
         else:
             logger.info(f"Tried to access non existent slot '{key}'")
             return None
 
+    def has_bot_message_after_latest_user_message(self) -> bool:
+        """Checks if there is a bot message after the most recent user message.
+
+        Returns:
+            `True` if there is an action after the most recent user message.
+        """
+        for event in reversed(self.applied_events()):
+            if isinstance(event, BotUttered):
+                return True
+            elif isinstance(event, UserUttered):
+                return False
+        return False
+
+    def has_action_after_latest_user_message(self) -> bool:
+        """Check if there is an action after the most recent user message.
+
+        Returns:
+            `True` if there is an action after the most recent user message.
+        """
+        for event in reversed(self.applied_events()):
+            if isinstance(event, ActionExecuted):
+                return True
+            elif isinstance(event, UserUttered):
+                return False
+        return False
+
     def get_latest_entity_values(
         self,
         entity_type: Text,
         entity_role: Optional[Text] = None,
         entity_group: Optional[Text] = None,
     ) -> Iterator[Text]:
         """Get entity values found for the passed entity type and optional role and
```

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/loading.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/story_reader/story_reader.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/story_reader/story_step_builder.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_step_builder.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/story_reader/yaml_story_reader.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/story_writer/story_writer.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/story_writer/yaml_story_writer.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/structures.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/structures.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/visualization.html` & `rasa-3.7.0b1/rasa/shared/core/training_data/visualization.html`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/core/training_data/visualization.py` & `rasa-3.7.0b1/rasa/shared/core/training_data/visualization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/data.py` & `rasa-3.7.0b1/rasa/shared/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/exceptions.py` & `rasa-3.7.0b1/rasa/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/importers/importer.py` & `rasa-3.7.0b1/rasa/shared/importers/importer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/importers/multi_project.py` & `rasa-3.7.0b1/rasa/shared/importers/multi_project.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/importers/rasa.py` & `rasa-3.7.0b1/rasa/shared/importers/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/importers/utils.py` & `rasa-3.7.0b1/rasa/shared/importers/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/constants.py` & `rasa-3.7.0b1/rasa/shared/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/entities_parser.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/entities_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/features.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/features.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/formats/dialogflow.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/formats/luis.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/formats/rasa.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/formats/rasa_yaml.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa_yaml.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/formats/readerwriter.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/readerwriter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/formats/wit.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/loading.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/lookup_tables_parser.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/lookup_tables_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/message.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/message.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/schemas/data_schema.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/data_schema.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/schemas/nlu.yml` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/schemas/responses.yml` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/responses.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/synonyms_parser.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/synonyms_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/training_data.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/training_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/nlu/training_data/util.py` & `rasa-3.7.0b1/rasa/shared/nlu/training_data/util.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/cli.py` & `rasa-3.7.0b1/rasa/shared/utils/cli.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/common.py` & `rasa-3.7.0b1/rasa/shared/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/io.py` & `rasa-3.7.0b1/rasa/shared/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/pykwalify_extensions.py` & `rasa-3.7.0b1/rasa/shared/utils/pykwalify_extensions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/schemas/domain.yml` & `rasa-3.7.0b1/rasa/shared/utils/schemas/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/schemas/events.py` & `rasa-3.7.0b1/rasa/shared/utils/schemas/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/schemas/model_config.yml` & `rasa-3.7.0b1/rasa/shared/utils/schemas/model_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/schemas/stories.yml` & `rasa-3.7.0b1/rasa/shared/utils/schemas/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/shared/utils/validation.py` & `rasa-3.7.0b1/rasa/shared/utils/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/telemetry.py` & `rasa-3.7.0b1/rasa/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/common.py` & `rasa-3.7.0b1/rasa/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/converter.py` & `rasa-3.7.0b1/rasa/utils/converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/endpoints.py` & `rasa-3.7.0b1/rasa/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/io.py` & `rasa-3.7.0b1/rasa/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/log_utils.py` & `rasa-3.7.0b1/rasa/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/plotting.py` & `rasa-3.7.0b1/rasa/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/callback.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/constants.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/crf.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/crf.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/data_generator.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/data_generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/environment.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/environment.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/layers.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/layers_utils.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/layers_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/metrics.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/metrics.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/model_data.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/model_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/model_data_utils.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/model_data_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/models.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/rasa_layers.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/rasa_layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/tensorflow/transformer.py` & `rasa-3.7.0b1/rasa/utils/tensorflow/transformer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/utils/train_utils.py` & `rasa-3.7.0b1/rasa/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/rasa/validator.py` & `rasa-3.7.0b1/rasa/validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.2/PKG-INFO` & `rasa-3.7.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa
-Version: 3.6.2
+Version: 3.7.0b1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
@@ -45,15 +45,15 @@
 Requires-Dist: fbmessenger (>=6.0.0,<6.1.0)
 Requires-Dist: github3.py (>=3.2.0,<3.3.0) ; extra == "gh-release-notes"
 Requires-Dist: google-auth (<3)
 Requires-Dist: jieba (>=0.39,<0.43) ; extra == "jieba" or extra == "full"
 Requires-Dist: joblib (>=0.15.1,<1.3.0)
 Requires-Dist: jsonpickle (>=1.3,<3.1)
 Requires-Dist: jsonschema (>=3.2,<4.18)
-Requires-Dist: matplotlib (>=3.1,<3.6)
+Requires-Dist: matplotlib (>=3.1,<3.8)
 Requires-Dist: mattermostwrapper (>=2.2,<2.3)
 Requires-Dist: networkx (>=2.4,<2.7)
 Requires-Dist: numpy (==1.22.3) ; sys_platform == "Windows" and platform_python_implementation != "PyPy" and python_version == "3.10"
 Requires-Dist: numpy (>=1.19.2,<1.22.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: numpy (>=1.19.2,<1.25.0) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: packaging (>=20.0,<21.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
@@ -68,15 +68,15 @@
 Requires-Dist: python-dateutil (>=2.8,<2.9)
 Requires-Dist: python-engineio (>=4,<6,!=5.0.0)
 Requires-Dist: python-socketio (>=4.4,<6)
 Requires-Dist: pytz (>=2019.1,<2023.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0)
 Requires-Dist: questionary (>=1.5.1,<1.11.0)
 Requires-Dist: randomname (>=0.1.5,<0.2.0)
-Requires-Dist: rasa-sdk (>=3.6.0,<3.7.0)
+Requires-Dist: rasa-sdk (>=3.7.0b1,<3.8.0)
 Requires-Dist: redis (>=4.5.3,<5.0)
 Requires-Dist: regex (>=2020.6,<2022.11)
 Requires-Dist: requests (>=2.23,<3.0)
 Requires-Dist: rocketchat_API (>=0.6.31,<1.31.0)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.17.22)
 Requires-Dist: sanic (>=21.12,<21.13)
 Requires-Dist: sanic-cors (>=2.0.0,<2.1.0)
@@ -91,29 +91,29 @@
 Requires-Dist: setuptools (>=41.0.0)
 Requires-Dist: sklearn-crfsuite (>=0.3,<0.4)
 Requires-Dist: slack-sdk (>=3.19.2,<4.0.0)
 Requires-Dist: spacy (>=3.1,<3.5) ; (sys_platform != "darwin" or platform_machine != "arm64") and (extra == "spacy" or extra == "full")
 Requires-Dist: spacy (>=3.4,<4.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "spacy" or extra == "full")
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: structlog-sentry (>=2.0.2,<3.0.0)
-Requires-Dist: tarsafe (>=0.0.3,<0.0.5)
+Requires-Dist: tarsafe (>=0.0.3,<0.0.6)
 Requires-Dist: tensorflow (==2.12.0) ; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: tensorflow-cpu-aws (==2.12.0) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
 Requires-Dist: tensorflow-intel (==2.12.0) ; sys_platform == "win32"
 Requires-Dist: tensorflow-io-gcs-filesystem (==0.31) ; sys_platform == "win32"
 Requires-Dist: tensorflow-io-gcs-filesystem (==0.32) ; sys_platform == "darwin" and platform_machine != "arm64"
 Requires-Dist: tensorflow-io-gcs-filesystem (==0.32) ; sys_platform == "linux"
 Requires-Dist: tensorflow-macos (==2.12.0) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: tensorflow-metal (==0.8.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "metal")
 Requires-Dist: tensorflow-text (==2.12.0) ; sys_platform != "win32" and platform_machine != "arm64" and platform_machine != "aarch64"
 Requires-Dist: tensorflow_hub (>=0.13.0,<0.14.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tqdm (>=4.31,<5.0)
 Requires-Dist: transformers (>=4.13.0,<=4.26.0) ; extra == "transformers" or extra == "full"
-Requires-Dist: twilio (>=6.26,<8.3)
+Requires-Dist: twilio (>=6.26,<8.4)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Requires-Dist: typing-utils (>=0.1.0,<0.2.0)
 Requires-Dist: ujson (>=1.35,<6.0)
 Requires-Dist: webexteamssdk (>=1.1.1,<1.7.0)
 Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Documentation, https://rasa.com/docs
 Project-URL: Repository, https://github.com/rasahq/rasa
```

