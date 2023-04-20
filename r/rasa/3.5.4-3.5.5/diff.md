# Comparing `tmp/rasa-3.5.4.tar.gz` & `tmp/rasa-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-3.5.4.tar", max compression
+gzip compressed data, was "rasa-3.5.5.tar", max compression
```

## Comparing `rasa-3.5.4.tar` & `rasa-3.5.5.tar`

### file list

```diff
@@ -1,315 +1,314 @@
--rw-r--r--   0        0        0    11352 2023-04-05 14:19:12.706149 rasa-3.5.4/LICENSE.txt
--rw-r--r--   0        0        0    20292 2023-04-05 14:19:12.706149 rasa-3.5.4/README.md
--rw-r--r--   0        0        0     8910 2023-04-05 14:19:12.886150 rasa-3.5.4/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/__init__.py
--rw-r--r--   0        0        0     5188 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/__main__.py
--rw-r--r--   0        0        0     5314 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/api.py
--rw-r--r--   0        0        0      115 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/__init__.py
--rw-r--r--   0        0        0     2388 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/data.py
--rw-r--r--   0        0        0     5242 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/default_arguments.py
--rw-r--r--   0        0        0     2199 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/evaluate.py
--rw-r--r--   0        0        0     1499 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/export.py
--rw-r--r--   0        0        0     2685 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/interactive.py
--rw-r--r--   0        0        0     5674 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/run.py
--rw-r--r--   0        0        0      367 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/shell.py
--rw-r--r--   0        0        0     6853 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/test.py
--rw-r--r--   0        0        0     7355 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/train.py
--rw-r--r--   0        0        0      861 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/visualize.py
--rw-r--r--   0        0        0     1027 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/arguments/x.py
--rw-r--r--   0        0        0     8906 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/data.py
--rw-r--r--   0        0        0     7948 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/evaluate.py
--rw-r--r--   0        0        0     8204 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/export.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/actions/__init__.py
--rw-r--r--   0        0        0      742 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/actions/actions.py
--rw-r--r--   0        0        0     1505 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/config.yml
--rw-r--r--   0        0        0      998 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/credentials.yml
--rw-r--r--   0        0        0     1433 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/data/nlu.yml
--rw-r--r--   0        0        0      244 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/data/rules.yml
--rw-r--r--   0        0        0      542 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/data/stories.yml
--rw-r--r--   0        0        0      565 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/domain.yml
--rw-r--r--   0        0        0     1411 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/endpoints.yml
--rw-r--r--   0        0        0     1664 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/initial_project/tests/test_stories.yml
--rw-r--r--   0        0        0     5827 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/interactive.py
--rw-r--r--   0        0        0     4196 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/run.py
--rw-r--r--   0        0        0     6846 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/scaffold.py
--rw-r--r--   0        0        0     4264 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/shell.py
--rw-r--r--   0        0        0     3118 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/telemetry.py
--rw-r--r--   0        0        0     8888 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/test.py
--rw-r--r--   0        0        0     6871 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/train.py
--rw-r--r--   0        0        0     9628 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/utils.py
--rw-r--r--   0        0        0     1256 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/visualize.py
--rw-r--r--   0        0        0     6785 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/cli/x.py
--rw-r--r--   0        0        0     1172 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/constants.py
--rw-r--r--   0        0        0      123 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/actions/__init__.py
--rw-r--r--   0        0        0    45583 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/actions/action.py
--rw-r--r--   0        0        0       78 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/actions/constants.py
--rw-r--r--   0        0        0    25982 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/actions/forms.py
--rw-r--r--   0        0        0     3322 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/actions/loops.py
--rw-r--r--   0        0        0     6078 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/actions/two_stage_fallback.py
--rw-r--r--   0        0        0    20361 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/agent.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/brokers/__init__.py
--rw-r--r--   0        0        0     4398 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/brokers/broker.py
--rw-r--r--   0        0        0     1801 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/brokers/file.py
--rw-r--r--   0        0        0    11397 2023-04-05 14:19:12.886150 rasa-3.5.4/rasa/core/brokers/kafka.py
--rw-r--r--   0        0        0    13495 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/brokers/pika.py
--rw-r--r--   0        0        0     2754 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/brokers/sql.py
--rw-r--r--   0        0        0     1656 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/__init__.py
--rw-r--r--   0        0        0    11686 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/botframework.py
--rw-r--r--   0        0        0     2746 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/callback.py
--rw-r--r--   0        0        0    13331 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/channel.py
--rw-r--r--   0        0        0     8073 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/console.py
--rw-r--r--   0        0        0    15789 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/facebook.py
--rw-r--r--   0        0        0    11532 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/hangouts.py
--rw-r--r--   0        0        0     7743 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/mattermost.py
--rw-r--r--   0        0        0     4814 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/rasa_chat.py
--rw-r--r--   0        0        0     6937 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/rest.py
--rw-r--r--   0        0        0     5999 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/rocketchat.py
--rw-r--r--   0        0        0    24359 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/slack.py
--rw-r--r--   0        0        0    10163 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/socketio.py
--rw-r--r--   0        0        0    10630 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/telegram.py
--rw-r--r--   0        0        0     5389 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/twilio.py
--rw-r--r--   0        0        0    13181 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/twilio_voice.py
--rw-r--r--   0        0        0     4845 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/channels/webexteams.py
--rw-r--r--   0        0        0     3047 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/constants.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/evaluation/__init__.py
--rw-r--r--   0        0        0     9154 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/evaluation/marker.py
--rw-r--r--   0        0        0    36811 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/evaluation/marker_base.py
--rw-r--r--   0        0        0    12086 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/evaluation/marker_stats.py
--rw-r--r--   0        0        0     3658 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/evaluation/marker_tracker_loader.py
--rw-r--r--   0        0        0      901 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/exceptions.py
--rw-r--r--   0        0        0    10220 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/exporter.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/featurizers/__init__.py
--rw-r--r--   0        0        0    17964 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/featurizers/precomputation.py
--rw-r--r--   0        0        0    15447 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/featurizers/single_state_featurizer.py
--rw-r--r--   0        0        0    43363 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/featurizers/tracker_featurizers.py
--rw-r--r--   0        0        0     2906 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/http_interpreter.py
--rw-r--r--   0        0        0     2018 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/jobs.py
--rw-r--r--   0        0        0     4719 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/lock.py
--rw-r--r--   0        0        0    11678 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/lock_store.py
--rw-r--r--   0        0        0    14821 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/migrate.py
--rw-r--r--   0        0        0      240 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/nlg/__init__.py
--rw-r--r--   0        0        0     3745 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/nlg/callback.py
--rw-r--r--   0        0        0     3285 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/nlg/generator.py
--rw-r--r--   0        0        0     2794 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/nlg/interpolator.py
--rw-r--r--   0        0        0     7503 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/nlg/response.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/policies/__init__.py
--rw-r--r--   0        0        0    12959 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/policies/ensemble.py
--rw-r--r--   0        0        0    19062 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/policies/memoization.py
--rw-r--r--   0        0        0    25038 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/policies/policy.py
--rw-r--r--   0        0        0    50189 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/policies/rule_policy.py
--rw-r--r--   0        0        0    86521 2023-04-05 14:19:12.890149 rasa-3.5.4/rasa/core/policies/ted_policy.py
--rw-r--r--   0        0        0    39329 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/policies/unexpected_intent_policy.py
--rw-r--r--   0        0        0    39091 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/processor.py
--rw-r--r--   0        0        0     9150 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/run.py
--rw-r--r--   0        0        0    48935 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/test.py
--rw-r--r--   0        0        0    58298 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/tracker_store.py
--rw-r--r--   0        0        0     3543 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/train.py
--rw-r--r--   0        0        0     3218 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/training/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/training/converters/__init__.py
--rw-r--r--   0        0        0     3889 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/training/converters/responses_prefix_converter.py
--rw-r--r--   0        0        0    59595 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/training/interactive.py
--rw-r--r--   0        0        0    13604 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/training/story_conflict.py
--rw-r--r--   0        0        0     3067 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/training/training.py
--rw-r--r--   0        0        0    10782 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/utils.py
--rw-r--r--   0        0        0     2125 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/core/visualize.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/__init__.py
--rw-r--r--   0        0        0    16744 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/caching.py
--rw-r--r--   0        0        0      469 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/constants.py
--rw-r--r--   0        0        0      437 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/exceptions.py
--rw-r--r--   0        0        0    22059 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/graph.py
--rw-r--r--   0        0        0     1384 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/loader.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/recipes/__init__.py
--rw-r--r--   0        0        0     1139 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/recipes/config_files/default_config.yml
--rw-r--r--   0        0        0     3244 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/recipes/default_components.py
--rw-r--r--   0        0        0    42860 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/recipes/default_recipe.py
--rw-r--r--   0        0        0     3260 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/recipes/graph_recipe.py
--rw-r--r--   0        0        0     3354 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/recipes/recipe.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/runner/__init__.py
--rw-r--r--   0        0        0     4302 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/runner/dask.py
--rw-r--r--   0        0        0     1672 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/runner/interface.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/storage/__init__.py
--rw-r--r--   0        0        0     9534 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/storage/local_model_storage.py
--rw-r--r--   0        0        0     3931 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/storage/resource.py
--rw-r--r--   0        0        0     6739 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/storage/storage.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/training/__init__.py
--rw-r--r--   0        0        0     6524 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/training/components.py
--rw-r--r--   0        0        0     1848 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/training/fingerprinting.py
--rw-r--r--   0        0        0    10516 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/training/graph_trainer.py
--rw-r--r--   0        0        0     5036 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/training/hooks.py
--rw-r--r--   0        0        0    22639 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/engine/validation.py
--rw-r--r--   0        0        0     2132 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/converters/__init__.py
--rw-r--r--   0        0        0     1576 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/converters/nlu_message_converter.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/__init__.py
--rw-r--r--   0        0        0     3832 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/domain_for_core_training_provider.py
--rw-r--r--   0        0        0     2571 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/domain_provider.py
--rw-r--r--   0        0        0     1294 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/forms_provider.py
--rw-r--r--   0        0        0     2119 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/nlu_training_data_provider.py
--rw-r--r--   0        0        0     1354 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/responses_provider.py
--rw-r--r--   0        0        0     1540 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/rule_only_provider.py
--rw-r--r--   0        0        0     1466 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/story_graph_provider.py
--rw-r--r--   0        0        0     1965 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/providers/training_tracker_provider.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/validators/__init__.py
--rw-r--r--   0        0        0    22668 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/validators/default_recipe_validator.py
--rw-r--r--   0        0        0    12863 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/graph_components/validators/finetuning_validator.py
--rw-r--r--   0        0        0     1782 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/jupyter.py
--rw-r--r--   0        0        0      101 2023-04-05 14:19:30.754159 rasa-3.5.4/rasa/keys
--rw-r--r--   0        0        0     3490 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/model.py
--rw-r--r--   0        0        0    14961 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/model_testing.py
--rw-r--r--   0        0        0    16760 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/model_training.py
--rw-r--r--   0        0        0      123 2023-04-05 14:19:12.894149 rasa-3.5.4/rasa/nlu/__init__.py
--rw-r--r--   0        0        0      118 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/__init__.py
--rw-r--r--   0        0        0      133 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/classifier.py
--rw-r--r--   0        0        0    71640 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/diet_classifier.py
--rw-r--r--   0        0        0     7150 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/fallback_classifier.py
--rw-r--r--   0        0        0     7581 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/keyword_intent_classifier.py
--rw-r--r--   0        0        0     7568 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/logistic_regression_classifier.py
--rw-r--r--   0        0        0     5559 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/mitie_intent_classifier.py
--rw-r--r--   0        0        0     1989 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/regex_message_handler.py
--rw-r--r--   0        0        0    11915 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/classifiers/sklearn_intent_classifier.py
--rw-r--r--   0        0        0     2757 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/constants.py
--rw-r--r--   0        0        0     1317 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/convert.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/emulators/__init__.py
--rw-r--r--   0        0        0     1748 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/emulators/dialogflow.py
--rw-r--r--   0        0        0     1367 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/emulators/emulator.py
--rw-r--r--   0        0        0     3032 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/emulators/luis.py
--rw-r--r--   0        0        0      334 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/emulators/no_emulator.py
--rw-r--r--   0        0        0     1930 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/emulators/wit.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/__init__.py
--rw-r--r--   0        0        0    26499 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/crf_entity_extractor.py
--rw-r--r--   0        0        0     7685 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/duckling_entity_extractor.py
--rw-r--r--   0        0        0     7160 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/entity_synonyms.py
--rw-r--r--   0        0        0    17530 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/extractor.py
--rw-r--r--   0        0        0    10973 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/mitie_entity_extractor.py
--rw-r--r--   0        0        0     8289 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/regex_entity_extractor.py
--rw-r--r--   0        0        0     3366 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/extractors/spacy_entity_extractor.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/__init__.py
--rw-r--r--   0        0        0    17142 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
--rw-r--r--   0        0        0     2433 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
--rw-r--r--   0        0        0    30361 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
--rw-r--r--   0        0        0     5861 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
--rw-r--r--   0        0        0     4888 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
--rw-r--r--   0        0        0     3347 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/featurizer.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/__init__.py
--rw-r--r--   0        0        0    33295 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
--rw-r--r--   0        0        0    21810 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
--rw-r--r--   0        0        0    10289 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
--rw-r--r--   0        0        0      220 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
--rw-r--r--   0        0        0      557 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/model.py
--rw-r--r--   0        0        0     8333 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/persistor.py
--rw-r--r--   0        0        0      803 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/run.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/selectors/__init__.py
--rw-r--r--   0        0        0    39012 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/selectors/response_selector.py
--rw-r--r--   0        0        0    66681 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/test.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/tokenizers/__init__.py
--rw-r--r--   0        0        0     5276 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/tokenizers/jieba_tokenizer.py
--rw-r--r--   0        0        0     2520 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/tokenizers/mitie_tokenizer.py
--rw-r--r--   0        0        0     2280 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/tokenizers/spacy_tokenizer.py
--rw-r--r--   0        0        0     7655 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3652 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      928 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/utils/__init__.py
--rw-r--r--   0        0        0    14703 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/utils/bilou_utils.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.898149 rasa-3.5.4/rasa/nlu/utils/hugging_face/__init__.py
--rw-r--r--   0        0        0     3380 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/nlu/utils/hugging_face/registry.py
--rw-r--r--   0        0        0     9143 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
--rw-r--r--   0        0        0     3887 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/nlu/utils/mitie_utils.py
--rw-r--r--   0        0        0     5386 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/nlu/utils/pattern_utils.py
--rw-r--r--   0        0        0    11795 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/nlu/utils/spacy_utils.py
--rw-r--r--   0        0        0     2241 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/plugin.py
--rw-r--r--   0        0        0    55474 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/server.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/__init__.py
--rw-r--r--   0        0        0     4294 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/constants.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/__init__.py
--rw-r--r--   0        0        0     4346 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/constants.py
--rw-r--r--   0        0        0     1366 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/conversation.py
--rw-r--r--   0        0        0    75018 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/domain.py
--rw-r--r--   0        0        0    65833 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/events.py
--rw-r--r--   0        0        0    35597 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/generator.py
--rw-r--r--   0        0        0     8130 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/slot_mappings.py
--rw-r--r--   0        0        0    16371 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/slots.py
--rw-r--r--   0        0        0    33176 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/trackers.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/__init__.py
--rw-r--r--   0        0        0     2895 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/loading.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_reader/__init__.py
--rw-r--r--   0        0        0     4449 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_reader/story_reader.py
--rw-r--r--   0        0        0     6671 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_reader/story_step_builder.py
--rw-r--r--   0        0        0    32873 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_writer/__init__.py
--rw-r--r--   0        0        0     2543 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_writer/story_writer.py
--rw-r--r--   0        0        0    14903 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
--rw-r--r--   0        0        0    29313 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/structures.py
--rw-r--r--   0        0        0     3500 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/visualization.html
--rw-r--r--   0        0        0    20341 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/core/training_data/visualization.py
--rw-r--r--   0        0        0     5479 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/data.py
--rw-r--r--   0        0        0     3633 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/importers/__init__.py
--rw-r--r--   0        0        0    21555 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/importers/importer.py
--rw-r--r--   0        0        0     7836 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/importers/multi_project.py
--rw-r--r--   0        0        0     3388 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/importers/rasa.py
--rw-r--r--   0        0        0      861 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/importers/utils.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/__init__.py
--rw-r--r--   0        0        0     1388 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/constants.py
--rw-r--r--   0        0        0      188 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/interpreter.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/__init__.py
--rw-r--r--   0        0        0     6759 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/entities_parser.py
--rw-r--r--   0        0        0    14835 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/features.py
--rw-r--r--   0        0        0      453 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/__init__.py
--rw-r--r--   0        0        0     6123 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/dialogflow.py
--rw-r--r--   0        0        0     3014 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/luis.py
--rw-r--r--   0        0        0     4495 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/rasa.py
--rw-r--r--   0        0        0    22353 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/rasa_yaml.py
--rw-r--r--   0        0        0     8540 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/readerwriter.py
--rw-r--r--   0        0        0     1820 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/formats/wit.py
--rw-r--r--   0        0        0     4258 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/loading.py
--rw-r--r--   0        0        0     1116 2023-04-05 14:19:12.902150 rasa-3.5.4/rasa/shared/nlu/training_data/lookup_tables_parser.py
--rw-r--r--   0        0        0    16662 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/message.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/schemas/__init__.py
--rw-r--r--   0        0        0     2565 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/schemas/data_schema.py
--rw-r--r--   0        0        0     1179 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/schemas/nlu.yml
--rw-r--r--   0        0        0     1595 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/schemas/responses.yml
--rw-r--r--   0        0        0     1476 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/synonyms_parser.py
--rw-r--r--   0        0        0    28493 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/training_data.py
--rw-r--r--   0        0        0     7040 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/nlu/training_data/util.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/__init__.py
--rw-r--r--   0        0        0     1129 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/cli.py
--rw-r--r--   0        0        0     8731 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/common.py
--rw-r--r--   0        0        0    19456 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/io.py
--rw-r--r--   0        0        0      883 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/pykwalify_extensions.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/schemas/__init__.py
--rw-r--r--   0        0        0       27 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/schemas/config.yml
--rw-r--r--   0        0        0     3267 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/schemas/domain.yml
--rw-r--r--   0        0        0     5569 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/schemas/events.py
--rw-r--r--   0        0        0      779 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/schemas/model_config.yml
--rw-r--r--   0        0        0     4034 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/schemas/stories.yml
--rw-r--r--   0        0        0    10178 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/shared/utils/validation.py
--rw-r--r--   0        0        0    36084 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/telemetry.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/__init__.py
--rw-r--r--   0        0        0    19852 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/common.py
--rw-r--r--   0        0        0     1647 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/converter.py
--rw-r--r--   0        0        0     8796 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/endpoints.py
--rw-r--r--   0        0        0     7831 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/io.py
--rw-r--r--   0        0        0    12246 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/plotting.py
--rw-r--r--   0        0        0        0 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     4036 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/callback.py
--rw-r--r--   0        0        0     3140 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/constants.py
--rw-r--r--   0        0        0     9020 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/crf.py
--rw-r--r--   0        0        0    15526 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/data_generator.py
--rw-r--r--   0        0        0     5576 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/environment.py
--rw-r--r--   0        0        0      168 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/exceptions.py
--rw-r--r--   0        0        0    59313 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/layers.py
--rw-r--r--   0        0        0     3319 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/layers_utils.py
--rw-r--r--   0        0        0    34572 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/model_data.py
--rw-r--r--   0        0        0    18667 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/model_data_utils.py
--rw-r--r--   0        0        0    36004 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/models.py
--rw-r--r--   0        0        0    49066 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/rasa_layers.py
--rw-r--r--   0        0        0    25509 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/transformer.py
--rw-r--r--   0        0        0      204 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/tensorflow/types.py
--rw-r--r--   0        0        0    20984 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/utils/train_utils.py
--rw-r--r--   0        0        0    17708 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/validator.py
--rw-r--r--   0        0        0      116 2023-04-05 14:19:12.906149 rasa-3.5.4/rasa/version.py
--rw-r--r--   0        0        0    27169 1970-01-01 00:00:00.000000 rasa-3.5.4/setup.py
--rw-r--r--   0        0        0    26357 1970-01-01 00:00:00.000000 rasa-3.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-04-20 12:25:45.652852 rasa-3.5.5/LICENSE.txt
+-rw-r--r--   0        0        0    20451 2023-04-20 12:25:45.656852 rasa-3.5.5/README.md
+-rw-r--r--   0        0        0     8933 2023-04-20 12:25:45.816854 rasa-3.5.5/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/__main__.py
+-rw-r--r--   0        0        0     5314 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/api.py
+-rw-r--r--   0        0        0      115 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/__init__.py
+-rw-r--r--   0        0        0     2388 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/data.py
+-rw-r--r--   0        0        0     5242 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/default_arguments.py
+-rw-r--r--   0        0        0     2199 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/evaluate.py
+-rw-r--r--   0        0        0     1499 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/export.py
+-rw-r--r--   0        0        0     2685 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/interactive.py
+-rw-r--r--   0        0        0     5674 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/run.py
+-rw-r--r--   0        0        0      367 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/shell.py
+-rw-r--r--   0        0        0     6853 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/test.py
+-rw-r--r--   0        0        0     7355 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/train.py
+-rw-r--r--   0        0        0      861 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/visualize.py
+-rw-r--r--   0        0        0     1027 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/arguments/x.py
+-rw-r--r--   0        0        0     8906 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/data.py
+-rw-r--r--   0        0        0     7948 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/evaluate.py
+-rw-r--r--   0        0        0     8204 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/export.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/actions/actions.py
+-rw-r--r--   0        0        0     1505 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/config.yml
+-rw-r--r--   0        0        0      998 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/credentials.yml
+-rw-r--r--   0        0        0     1433 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/data/nlu.yml
+-rw-r--r--   0        0        0      244 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/data/rules.yml
+-rw-r--r--   0        0        0      542 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/data/stories.yml
+-rw-r--r--   0        0        0      565 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/domain.yml
+-rw-r--r--   0        0        0     1411 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/initial_project/tests/test_stories.yml
+-rw-r--r--   0        0        0     5827 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/interactive.py
+-rw-r--r--   0        0        0     4196 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/run.py
+-rw-r--r--   0        0        0     6846 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/scaffold.py
+-rw-r--r--   0        0        0     4264 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/shell.py
+-rw-r--r--   0        0        0     3118 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/telemetry.py
+-rw-r--r--   0        0        0     8888 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/test.py
+-rw-r--r--   0        0        0     6871 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/train.py
+-rw-r--r--   0        0        0     9670 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/utils.py
+-rw-r--r--   0        0        0     1256 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/visualize.py
+-rw-r--r--   0        0        0     6785 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/cli/x.py
+-rw-r--r--   0        0        0     1172 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/constants.py
+-rw-r--r--   0        0        0      123 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/core/actions/__init__.py
+-rw-r--r--   0        0        0    45583 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/core/actions/action.py
+-rw-r--r--   0        0        0       78 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/core/actions/constants.py
+-rw-r--r--   0        0        0    25982 2023-04-20 12:25:45.816854 rasa-3.5.5/rasa/core/actions/forms.py
+-rw-r--r--   0        0        0     3322 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/actions/loops.py
+-rw-r--r--   0        0        0     6078 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/actions/two_stage_fallback.py
+-rw-r--r--   0        0        0    20361 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/agent.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/brokers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/brokers/broker.py
+-rw-r--r--   0        0        0     1801 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/brokers/file.py
+-rw-r--r--   0        0        0    11397 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/brokers/kafka.py
+-rw-r--r--   0        0        0    13495 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/brokers/pika.py
+-rw-r--r--   0        0        0     2754 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/brokers/sql.py
+-rw-r--r--   0        0        0     1656 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/__init__.py
+-rw-r--r--   0        0        0    11686 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/botframework.py
+-rw-r--r--   0        0        0     2746 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/callback.py
+-rw-r--r--   0        0        0    13331 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/channel.py
+-rw-r--r--   0        0        0     8073 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/console.py
+-rw-r--r--   0        0        0    15789 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/facebook.py
+-rw-r--r--   0        0        0    11532 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/hangouts.py
+-rw-r--r--   0        0        0     7743 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/mattermost.py
+-rw-r--r--   0        0        0     4814 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/rasa_chat.py
+-rw-r--r--   0        0        0     6937 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/rest.py
+-rw-r--r--   0        0        0     5999 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/rocketchat.py
+-rw-r--r--   0        0        0    24359 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/slack.py
+-rw-r--r--   0        0        0    10163 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/socketio.py
+-rw-r--r--   0        0        0    10630 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/telegram.py
+-rw-r--r--   0        0        0     5389 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/twilio.py
+-rw-r--r--   0        0        0    13181 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/twilio_voice.py
+-rw-r--r--   0        0        0     4845 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/channels/webexteams.py
+-rw-r--r--   0        0        0     3047 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/constants.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     9154 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/evaluation/marker.py
+-rw-r--r--   0        0        0    36811 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/evaluation/marker_base.py
+-rw-r--r--   0        0        0    12086 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/evaluation/marker_stats.py
+-rw-r--r--   0        0        0     3658 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/evaluation/marker_tracker_loader.py
+-rw-r--r--   0        0        0      901 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/exceptions.py
+-rw-r--r--   0        0        0    10220 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/exporter.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/featurizers/__init__.py
+-rw-r--r--   0        0        0    17964 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/featurizers/precomputation.py
+-rw-r--r--   0        0        0    15447 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/featurizers/single_state_featurizer.py
+-rw-r--r--   0        0        0    43363 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/featurizers/tracker_featurizers.py
+-rw-r--r--   0        0        0     2906 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/http_interpreter.py
+-rw-r--r--   0        0        0     2018 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/jobs.py
+-rw-r--r--   0        0        0     4719 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/lock.py
+-rw-r--r--   0        0        0    11678 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/lock_store.py
+-rw-r--r--   0        0        0    14821 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/migrate.py
+-rw-r--r--   0        0        0      240 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/nlg/__init__.py
+-rw-r--r--   0        0        0     3745 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/nlg/callback.py
+-rw-r--r--   0        0        0     3285 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/nlg/generator.py
+-rw-r--r--   0        0        0     2794 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/nlg/interpolator.py
+-rw-r--r--   0        0        0     7503 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/nlg/response.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/policies/__init__.py
+-rw-r--r--   0        0        0    12959 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/policies/ensemble.py
+-rw-r--r--   0        0        0    19062 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/policies/memoization.py
+-rw-r--r--   0        0        0    25038 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/policies/policy.py
+-rw-r--r--   0        0        0    50189 2023-04-20 12:25:45.820854 rasa-3.5.5/rasa/core/policies/rule_policy.py
+-rw-r--r--   0        0        0    86521 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/policies/ted_policy.py
+-rw-r--r--   0        0        0    39329 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/policies/unexpected_intent_policy.py
+-rw-r--r--   0        0        0    39091 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/processor.py
+-rw-r--r--   0        0        0     9150 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/run.py
+-rw-r--r--   0        0        0    48935 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/test.py
+-rw-r--r--   0        0        0    58298 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/tracker_store.py
+-rw-r--r--   0        0        0     3543 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/train.py
+-rw-r--r--   0        0        0     3218 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/training/converters/__init__.py
+-rw-r--r--   0        0        0     3889 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/training/converters/responses_prefix_converter.py
+-rw-r--r--   0        0        0    59595 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/training/interactive.py
+-rw-r--r--   0        0        0    13604 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/training/story_conflict.py
+-rw-r--r--   0        0        0     3067 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/training/training.py
+-rw-r--r--   0        0        0    10782 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/utils.py
+-rw-r--r--   0        0        0     2125 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/core/visualize.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/__init__.py
+-rw-r--r--   0        0        0    16744 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/caching.py
+-rw-r--r--   0        0        0      469 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/constants.py
+-rw-r--r--   0        0        0      437 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/exceptions.py
+-rw-r--r--   0        0        0    22059 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/graph.py
+-rw-r--r--   0        0        0     1384 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/loader.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/recipes/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/recipes/config_files/default_config.yml
+-rw-r--r--   0        0        0     3244 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/recipes/default_components.py
+-rw-r--r--   0        0        0    42860 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/recipes/default_recipe.py
+-rw-r--r--   0        0        0     3260 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/recipes/graph_recipe.py
+-rw-r--r--   0        0        0     3354 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/recipes/recipe.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/runner/__init__.py
+-rw-r--r--   0        0        0     4302 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/runner/dask.py
+-rw-r--r--   0        0        0     1672 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/runner/interface.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/storage/__init__.py
+-rw-r--r--   0        0        0     9534 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/storage/local_model_storage.py
+-rw-r--r--   0        0        0     3931 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/storage/resource.py
+-rw-r--r--   0        0        0     6739 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/training/__init__.py
+-rw-r--r--   0        0        0     6524 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/training/components.py
+-rw-r--r--   0        0        0     1848 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/training/fingerprinting.py
+-rw-r--r--   0        0        0    10516 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/training/graph_trainer.py
+-rw-r--r--   0        0        0     5036 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/training/hooks.py
+-rw-r--r--   0        0        0    22639 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/engine/validation.py
+-rw-r--r--   0        0        0     2132 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/converters/__init__.py
+-rw-r--r--   0        0        0     1576 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/converters/nlu_message_converter.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/domain_for_core_training_provider.py
+-rw-r--r--   0        0        0     2571 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/domain_provider.py
+-rw-r--r--   0        0        0     1294 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/forms_provider.py
+-rw-r--r--   0        0        0     2119 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/nlu_training_data_provider.py
+-rw-r--r--   0        0        0     1354 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/responses_provider.py
+-rw-r--r--   0        0        0     1540 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/rule_only_provider.py
+-rw-r--r--   0        0        0     1466 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/story_graph_provider.py
+-rw-r--r--   0        0        0     1965 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/providers/training_tracker_provider.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/validators/__init__.py
+-rw-r--r--   0        0        0    22668 2023-04-20 12:25:45.824854 rasa-3.5.5/rasa/graph_components/validators/default_recipe_validator.py
+-rw-r--r--   0        0        0    12863 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/graph_components/validators/finetuning_validator.py
+-rw-r--r--   0        0        0     1782 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/jupyter.py
+-rw-r--r--   0        0        0      101 2023-04-20 12:26:03.297006 rasa-3.5.5/rasa/keys
+-rw-r--r--   0        0        0     3490 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/model.py
+-rw-r--r--   0        0        0    14961 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/model_testing.py
+-rw-r--r--   0        0        0    16760 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/model_training.py
+-rw-r--r--   0        0        0      123 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/classifier.py
+-rw-r--r--   0        0        0    71640 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/diet_classifier.py
+-rw-r--r--   0        0        0     7150 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/fallback_classifier.py
+-rw-r--r--   0        0        0     7581 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/keyword_intent_classifier.py
+-rw-r--r--   0        0        0     7568 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0        0        0     5559 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/mitie_intent_classifier.py
+-rw-r--r--   0        0        0     1989 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/regex_message_handler.py
+-rw-r--r--   0        0        0    11915 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/classifiers/sklearn_intent_classifier.py
+-rw-r--r--   0        0        0     2757 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/constants.py
+-rw-r--r--   0        0        0     1317 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/convert.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/emulators/__init__.py
+-rw-r--r--   0        0        0     1748 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/emulators/dialogflow.py
+-rw-r--r--   0        0        0     1367 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/emulators/emulator.py
+-rw-r--r--   0        0        0     3032 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/emulators/luis.py
+-rw-r--r--   0        0        0      334 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/emulators/no_emulator.py
+-rw-r--r--   0        0        0     1930 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/emulators/wit.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/__init__.py
+-rw-r--r--   0        0        0    26499 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/crf_entity_extractor.py
+-rw-r--r--   0        0        0     7685 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/duckling_entity_extractor.py
+-rw-r--r--   0        0        0     7160 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/entity_synonyms.py
+-rw-r--r--   0        0        0    17530 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/extractor.py
+-rw-r--r--   0        0        0    10973 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/mitie_entity_extractor.py
+-rw-r--r--   0        0        0     8289 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/regex_entity_extractor.py
+-rw-r--r--   0        0        0     3366 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/extractors/spacy_entity_extractor.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/__init__.py
+-rw-r--r--   0        0        0    17142 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
+-rw-r--r--   0        0        0     2433 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
+-rw-r--r--   0        0        0    30361 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
+-rw-r--r--   0        0        0     5861 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
+-rw-r--r--   0        0        0     4888 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
+-rw-r--r--   0        0        0     3347 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/featurizer.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/__init__.py
+-rw-r--r--   0        0        0    33295 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
+-rw-r--r--   0        0        0    21810 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
+-rw-r--r--   0        0        0    10289 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
+-rw-r--r--   0        0        0      220 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
+-rw-r--r--   0        0        0      557 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/model.py
+-rw-r--r--   0        0        0     8333 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/persistor.py
+-rw-r--r--   0        0        0      803 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/run.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/selectors/__init__.py
+-rw-r--r--   0        0        0    39012 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/selectors/response_selector.py
+-rw-r--r--   0        0        0    66681 2023-04-20 12:25:45.828854 rasa-3.5.5/rasa/nlu/test.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5276 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/tokenizers/jieba_tokenizer.py
+-rw-r--r--   0        0        0     2520 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/tokenizers/mitie_tokenizer.py
+-rw-r--r--   0        0        0     2280 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0        0        0     7655 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3652 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      928 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/__init__.py
+-rw-r--r--   0        0        0    14703 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/bilou_utils.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3380 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/hugging_face/registry.py
+-rw-r--r--   0        0        0     9143 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
+-rw-r--r--   0        0        0     3887 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/mitie_utils.py
+-rw-r--r--   0        0        0     5386 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/pattern_utils.py
+-rw-r--r--   0        0        0    11795 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/nlu/utils/spacy_utils.py
+-rw-r--r--   0        0        0     2241 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/plugin.py
+-rw-r--r--   0        0        0    55529 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/server.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/__init__.py
+-rw-r--r--   0        0        0     4294 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/__init__.py
+-rw-r--r--   0        0        0     4346 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/constants.py
+-rw-r--r--   0        0        0     1366 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/conversation.py
+-rw-r--r--   0        0        0    75018 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/domain.py
+-rw-r--r--   0        0        0    65833 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/events.py
+-rw-r--r--   0        0        0    35597 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/generator.py
+-rw-r--r--   0        0        0     8286 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/slot_mappings.py
+-rw-r--r--   0        0        0    16371 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/slots.py
+-rw-r--r--   0        0        0    33176 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/trackers.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/__init__.py
+-rw-r--r--   0        0        0     2895 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/loading.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_reader/__init__.py
+-rw-r--r--   0        0        0     4449 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_reader/story_reader.py
+-rw-r--r--   0        0        0     6671 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_reader/story_step_builder.py
+-rw-r--r--   0        0        0    32873 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_writer/__init__.py
+-rw-r--r--   0        0        0     2543 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_writer/story_writer.py
+-rw-r--r--   0        0        0    14903 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
+-rw-r--r--   0        0        0    29313 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/structures.py
+-rw-r--r--   0        0        0     3500 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/visualization.html
+-rw-r--r--   0        0        0    20341 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/core/training_data/visualization.py
+-rw-r--r--   0        0        0     5479 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/data.py
+-rw-r--r--   0        0        0     3633 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/importers/__init__.py
+-rw-r--r--   0        0        0    21555 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/importers/importer.py
+-rw-r--r--   0        0        0     7836 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/importers/multi_project.py
+-rw-r--r--   0        0        0     3388 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/importers/rasa.py
+-rw-r--r--   0        0        0      861 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/importers/utils.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/__init__.py
+-rw-r--r--   0        0        0     1388 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/constants.py
+-rw-r--r--   0        0        0      188 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/interpreter.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/training_data/__init__.py
+-rw-r--r--   0        0        0     6759 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/training_data/entities_parser.py
+-rw-r--r--   0        0        0    14835 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/training_data/features.py
+-rw-r--r--   0        0        0      453 2023-04-20 12:25:45.832854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/dialogflow.py
+-rw-r--r--   0        0        0     3014 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/luis.py
+-rw-r--r--   0        0        0     4495 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/rasa.py
+-rw-r--r--   0        0        0    22353 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/rasa_yaml.py
+-rw-r--r--   0        0        0     8540 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/readerwriter.py
+-rw-r--r--   0        0        0     1820 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/formats/wit.py
+-rw-r--r--   0        0        0     4258 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/loading.py
+-rw-r--r--   0        0        0     1116 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/lookup_tables_parser.py
+-rw-r--r--   0        0        0    16662 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/message.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/schemas/__init__.py
+-rw-r--r--   0        0        0     2565 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/schemas/data_schema.py
+-rw-r--r--   0        0        0     1179 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/schemas/nlu.yml
+-rw-r--r--   0        0        0     1595 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/schemas/responses.yml
+-rw-r--r--   0        0        0     1476 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/synonyms_parser.py
+-rw-r--r--   0        0        0    28493 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/training_data.py
+-rw-r--r--   0        0        0     7040 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/nlu/training_data/util.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/cli.py
+-rw-r--r--   0        0        0     8731 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/common.py
+-rw-r--r--   0        0        0    20533 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/io.py
+-rw-r--r--   0        0        0      883 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/pykwalify_extensions.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/schemas/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/schemas/config.yml
+-rw-r--r--   0        0        0     3267 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/schemas/domain.yml
+-rw-r--r--   0        0        0     5569 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/schemas/events.py
+-rw-r--r--   0        0        0      779 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/schemas/model_config.yml
+-rw-r--r--   0        0        0     4034 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/schemas/stories.yml
+-rw-r--r--   0        0        0    10178 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/shared/utils/validation.py
+-rw-r--r--   0        0        0    36084 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/telemetry.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/__init__.py
+-rw-r--r--   0        0        0    19852 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/common.py
+-rw-r--r--   0        0        0     1647 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/converter.py
+-rw-r--r--   0        0        0     8796 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/endpoints.py
+-rw-r--r--   0        0        0     7831 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/io.py
+-rw-r--r--   0        0        0    12246 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/plotting.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     4036 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/callback.py
+-rw-r--r--   0        0        0     3140 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/constants.py
+-rw-r--r--   0        0        0     9020 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/crf.py
+-rw-r--r--   0        0        0    15526 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/data_generator.py
+-rw-r--r--   0        0        0     5576 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/environment.py
+-rw-r--r--   0        0        0      168 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/exceptions.py
+-rw-r--r--   0        0        0    59313 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/layers.py
+-rw-r--r--   0        0        0     3319 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/layers_utils.py
+-rw-r--r--   0        0        0    34572 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/model_data.py
+-rw-r--r--   0        0        0    18667 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/model_data_utils.py
+-rw-r--r--   0        0        0    36004 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/models.py
+-rw-r--r--   0        0        0    49066 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/rasa_layers.py
+-rw-r--r--   0        0        0    25509 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/transformer.py
+-rw-r--r--   0        0        0      204 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/tensorflow/types.py
+-rw-r--r--   0        0        0    20984 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/utils/train_utils.py
+-rw-r--r--   0        0        0    17708 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/validator.py
+-rw-r--r--   0        0        0      116 2023-04-20 12:25:45.836854 rasa-3.5.5/rasa/version.py
+-rw-r--r--   0        0        0    26607 1970-01-01 00:00:00.000000 rasa-3.5.5/PKG-INFO
```

### Comparing `rasa-3.5.4/LICENSE.txt` & `rasa-3.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/README.md` & `rasa-3.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
 
 ### Installing Poetry
 
 Rasa uses Poetry for packaging and dependency management. If you want to build it from source,
 you have to install Poetry first. Please follow
 [the official guide](https://python-poetry.org/docs/#installation) to see all possible options.
 
+To update an existing poetry version to the [version](.github/poetry_version.txt), currently used in rasa, run:
+```shell
+    poetry self update <version>
+```
+
 ### Managing environments
 
 The official [Poetry guide](https://python-poetry.org/docs/managing-environments/) suggests to use
 [pyenv](https://github.com/pyenv/pyenv) or any other similar tool to easily switch between Python versions.
 This is how it can be done:
 
 ```bash
```

### Comparing `rasa-3.5.4/pyproject.toml` & `rasa-3.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa"
-version = "3.5.4"
+version = "3.5.5"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -144,14 +144,15 @@
 tarsafe = "^0.0.3"
 google-auth = "<3"
 CacheControl = "^0.12.9"
 randomname = "^0.1.5"
 pluggy = "^1.0.0"
 slack-sdk = "^3.19.2"
 confluent-kafka = "^1.9.2"
+portalocker = "^2.7.0"
 [[tool.poetry.dependencies.dask]]
 version = "2022.2.0"
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.dask]]
 version = "2022.10.2"
 python = ">=3.8,<3.11"
```

### Comparing `rasa-3.5.4/rasa/__main__.py` & `rasa-3.5.5/rasa/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/api.py` & `rasa-3.5.5/rasa/api.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/data.py` & `rasa-3.5.5/rasa/cli/arguments/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/default_arguments.py` & `rasa-3.5.5/rasa/cli/arguments/default_arguments.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/evaluate.py` & `rasa-3.5.5/rasa/cli/arguments/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/export.py` & `rasa-3.5.5/rasa/cli/arguments/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/interactive.py` & `rasa-3.5.5/rasa/cli/arguments/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/run.py` & `rasa-3.5.5/rasa/cli/arguments/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/test.py` & `rasa-3.5.5/rasa/cli/arguments/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/train.py` & `rasa-3.5.5/rasa/cli/arguments/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/visualize.py` & `rasa-3.5.5/rasa/cli/arguments/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/arguments/x.py` & `rasa-3.5.5/rasa/cli/arguments/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/data.py` & `rasa-3.5.5/rasa/cli/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/evaluate.py` & `rasa-3.5.5/rasa/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/export.py` & `rasa-3.5.5/rasa/cli/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/actions/actions.py` & `rasa-3.5.5/rasa/cli/initial_project/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/config.yml` & `rasa-3.5.5/rasa/cli/initial_project/config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/credentials.yml` & `rasa-3.5.5/rasa/cli/initial_project/credentials.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/data/nlu.yml` & `rasa-3.5.5/rasa/cli/initial_project/data/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/data/stories.yml` & `rasa-3.5.5/rasa/cli/initial_project/data/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/domain.yml` & `rasa-3.5.5/rasa/cli/initial_project/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/endpoints.yml` & `rasa-3.5.5/rasa/cli/initial_project/endpoints.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/initial_project/tests/test_stories.yml` & `rasa-3.5.5/rasa/cli/initial_project/tests/test_stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/interactive.py` & `rasa-3.5.5/rasa/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/run.py` & `rasa-3.5.5/rasa/cli/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/scaffold.py` & `rasa-3.5.5/rasa/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/shell.py` & `rasa-3.5.5/rasa/cli/shell.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/telemetry.py` & `rasa-3.5.5/rasa/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/test.py` & `rasa-3.5.5/rasa/cli/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/train.py` & `rasa-3.5.5/rasa/cli/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/utils.py` & `rasa-3.5.5/rasa/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,17 @@
 
 def validate_assistant_id_in_config(config_file: Union["Path", Text]) -> None:
     """Verifies that the assistant_id key exists and has a unique value in config.
 
     Issues a warning if the key does not exist or has the default value and replaces it
     with a pseudo-random string value.
     """
-    config_data = rasa.shared.utils.io.read_config_file(config_file)
+    config_data = rasa.shared.utils.io.read_config_file(
+        config_file, reader_type=["safe", "rt"]
+    )
     assistant_id = config_data.get(ASSISTANT_ID_KEY)
 
     if assistant_id is None or assistant_id == ASSISTANT_ID_DEFAULT_VALUE:
         rasa.shared.utils.io.raise_warning(
             f"The config file '{str(config_file)}' is missing a unique value for the "
             f"'{ASSISTANT_ID_KEY}' mandatory key. Proceeding with generating a random "
             f"value and overwriting the '{ASSISTANT_ID_KEY}' in the config file."
```

### Comparing `rasa-3.5.4/rasa/cli/visualize.py` & `rasa-3.5.5/rasa/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/cli/x.py` & `rasa-3.5.5/rasa/cli/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/constants.py` & `rasa-3.5.5/rasa/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/actions/action.py` & `rasa-3.5.5/rasa/core/actions/action.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/actions/forms.py` & `rasa-3.5.5/rasa/core/actions/forms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/actions/loops.py` & `rasa-3.5.5/rasa/core/actions/loops.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/actions/two_stage_fallback.py` & `rasa-3.5.5/rasa/core/actions/two_stage_fallback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/agent.py` & `rasa-3.5.5/rasa/core/agent.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/brokers/broker.py` & `rasa-3.5.5/rasa/core/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/brokers/file.py` & `rasa-3.5.5/rasa/core/brokers/file.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/brokers/kafka.py` & `rasa-3.5.5/rasa/core/brokers/kafka.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/brokers/pika.py` & `rasa-3.5.5/rasa/core/brokers/pika.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/brokers/sql.py` & `rasa-3.5.5/rasa/core/brokers/sql.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/__init__.py` & `rasa-3.5.5/rasa/core/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/botframework.py` & `rasa-3.5.5/rasa/core/channels/botframework.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/callback.py` & `rasa-3.5.5/rasa/core/channels/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/channel.py` & `rasa-3.5.5/rasa/core/channels/channel.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/console.py` & `rasa-3.5.5/rasa/core/channels/console.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/facebook.py` & `rasa-3.5.5/rasa/core/channels/facebook.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/hangouts.py` & `rasa-3.5.5/rasa/core/channels/hangouts.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/mattermost.py` & `rasa-3.5.5/rasa/core/channels/mattermost.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/rasa_chat.py` & `rasa-3.5.5/rasa/core/channels/rasa_chat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/rest.py` & `rasa-3.5.5/rasa/core/channels/rest.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/rocketchat.py` & `rasa-3.5.5/rasa/core/channels/rocketchat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/slack.py` & `rasa-3.5.5/rasa/core/channels/slack.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/socketio.py` & `rasa-3.5.5/rasa/core/channels/socketio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/telegram.py` & `rasa-3.5.5/rasa/core/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/twilio.py` & `rasa-3.5.5/rasa/core/channels/twilio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/twilio_voice.py` & `rasa-3.5.5/rasa/core/channels/twilio_voice.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/channels/webexteams.py` & `rasa-3.5.5/rasa/core/channels/webexteams.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/constants.py` & `rasa-3.5.5/rasa/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/evaluation/marker.py` & `rasa-3.5.5/rasa/core/evaluation/marker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/evaluation/marker_base.py` & `rasa-3.5.5/rasa/core/evaluation/marker_base.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/evaluation/marker_stats.py` & `rasa-3.5.5/rasa/core/evaluation/marker_stats.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/evaluation/marker_tracker_loader.py` & `rasa-3.5.5/rasa/core/evaluation/marker_tracker_loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/exceptions.py` & `rasa-3.5.5/rasa/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/exporter.py` & `rasa-3.5.5/rasa/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/featurizers/precomputation.py` & `rasa-3.5.5/rasa/core/featurizers/precomputation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/featurizers/single_state_featurizer.py` & `rasa-3.5.5/rasa/core/featurizers/single_state_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/featurizers/tracker_featurizers.py` & `rasa-3.5.5/rasa/core/featurizers/tracker_featurizers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/http_interpreter.py` & `rasa-3.5.5/rasa/core/http_interpreter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/jobs.py` & `rasa-3.5.5/rasa/core/jobs.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/lock.py` & `rasa-3.5.5/rasa/core/lock.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/lock_store.py` & `rasa-3.5.5/rasa/core/lock_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/migrate.py` & `rasa-3.5.5/rasa/core/migrate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/nlg/callback.py` & `rasa-3.5.5/rasa/core/nlg/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/nlg/generator.py` & `rasa-3.5.5/rasa/core/nlg/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/nlg/interpolator.py` & `rasa-3.5.5/rasa/core/nlg/interpolator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/nlg/response.py` & `rasa-3.5.5/rasa/core/nlg/response.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/policies/ensemble.py` & `rasa-3.5.5/rasa/core/policies/ensemble.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/policies/memoization.py` & `rasa-3.5.5/rasa/core/policies/memoization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/policies/policy.py` & `rasa-3.5.5/rasa/core/policies/policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/policies/rule_policy.py` & `rasa-3.5.5/rasa/core/policies/rule_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/policies/ted_policy.py` & `rasa-3.5.5/rasa/core/policies/ted_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/policies/unexpected_intent_policy.py` & `rasa-3.5.5/rasa/core/policies/unexpected_intent_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/processor.py` & `rasa-3.5.5/rasa/core/processor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/run.py` & `rasa-3.5.5/rasa/core/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/test.py` & `rasa-3.5.5/rasa/core/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/tracker_store.py` & `rasa-3.5.5/rasa/core/tracker_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/train.py` & `rasa-3.5.5/rasa/core/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/training/__init__.py` & `rasa-3.5.5/rasa/core/training/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/training/converters/responses_prefix_converter.py` & `rasa-3.5.5/rasa/core/training/converters/responses_prefix_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/training/interactive.py` & `rasa-3.5.5/rasa/core/training/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/training/story_conflict.py` & `rasa-3.5.5/rasa/core/training/story_conflict.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/training/training.py` & `rasa-3.5.5/rasa/core/training/training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/utils.py` & `rasa-3.5.5/rasa/core/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/core/visualize.py` & `rasa-3.5.5/rasa/core/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/caching.py` & `rasa-3.5.5/rasa/engine/caching.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/graph.py` & `rasa-3.5.5/rasa/engine/graph.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/loader.py` & `rasa-3.5.5/rasa/engine/loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/recipes/config_files/default_config.yml` & `rasa-3.5.5/rasa/engine/recipes/config_files/default_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/recipes/default_components.py` & `rasa-3.5.5/rasa/engine/recipes/default_components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/recipes/default_recipe.py` & `rasa-3.5.5/rasa/engine/recipes/default_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/recipes/graph_recipe.py` & `rasa-3.5.5/rasa/engine/recipes/graph_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/recipes/recipe.py` & `rasa-3.5.5/rasa/engine/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/runner/dask.py` & `rasa-3.5.5/rasa/engine/runner/dask.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/runner/interface.py` & `rasa-3.5.5/rasa/engine/runner/interface.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/storage/local_model_storage.py` & `rasa-3.5.5/rasa/engine/storage/local_model_storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/storage/resource.py` & `rasa-3.5.5/rasa/engine/storage/resource.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/storage/storage.py` & `rasa-3.5.5/rasa/engine/storage/storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/training/components.py` & `rasa-3.5.5/rasa/engine/training/components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/training/fingerprinting.py` & `rasa-3.5.5/rasa/engine/training/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/training/graph_trainer.py` & `rasa-3.5.5/rasa/engine/training/graph_trainer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/training/hooks.py` & `rasa-3.5.5/rasa/engine/training/hooks.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/engine/validation.py` & `rasa-3.5.5/rasa/engine/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/exceptions.py` & `rasa-3.5.5/rasa/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/converters/nlu_message_converter.py` & `rasa-3.5.5/rasa/graph_components/converters/nlu_message_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/domain_for_core_training_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/domain_for_core_training_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/domain_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/domain_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/forms_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/forms_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/nlu_training_data_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/nlu_training_data_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/responses_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/responses_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/rule_only_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/rule_only_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/story_graph_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/story_graph_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/providers/training_tracker_provider.py` & `rasa-3.5.5/rasa/graph_components/providers/training_tracker_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/validators/default_recipe_validator.py` & `rasa-3.5.5/rasa/graph_components/validators/default_recipe_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/graph_components/validators/finetuning_validator.py` & `rasa-3.5.5/rasa/graph_components/validators/finetuning_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/jupyter.py` & `rasa-3.5.5/rasa/jupyter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/model.py` & `rasa-3.5.5/rasa/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/model_testing.py` & `rasa-3.5.5/rasa/model_testing.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/model_training.py` & `rasa-3.5.5/rasa/model_training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/diet_classifier.py` & `rasa-3.5.5/rasa/nlu/classifiers/diet_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/fallback_classifier.py` & `rasa-3.5.5/rasa/nlu/classifiers/fallback_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/keyword_intent_classifier.py` & `rasa-3.5.5/rasa/nlu/classifiers/keyword_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/logistic_regression_classifier.py` & `rasa-3.5.5/rasa/nlu/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/mitie_intent_classifier.py` & `rasa-3.5.5/rasa/nlu/classifiers/mitie_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/regex_message_handler.py` & `rasa-3.5.5/rasa/nlu/classifiers/regex_message_handler.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/classifiers/sklearn_intent_classifier.py` & `rasa-3.5.5/rasa/nlu/classifiers/sklearn_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/constants.py` & `rasa-3.5.5/rasa/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/convert.py` & `rasa-3.5.5/rasa/nlu/convert.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/emulators/dialogflow.py` & `rasa-3.5.5/rasa/nlu/emulators/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/emulators/emulator.py` & `rasa-3.5.5/rasa/nlu/emulators/emulator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/emulators/luis.py` & `rasa-3.5.5/rasa/nlu/emulators/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/emulators/wit.py` & `rasa-3.5.5/rasa/nlu/emulators/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/crf_entity_extractor.py` & `rasa-3.5.5/rasa/nlu/extractors/crf_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/duckling_entity_extractor.py` & `rasa-3.5.5/rasa/nlu/extractors/duckling_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/entity_synonyms.py` & `rasa-3.5.5/rasa/nlu/extractors/entity_synonyms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/extractor.py` & `rasa-3.5.5/rasa/nlu/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/mitie_entity_extractor.py` & `rasa-3.5.5/rasa/nlu/extractors/mitie_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/regex_entity_extractor.py` & `rasa-3.5.5/rasa/nlu/extractors/regex_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/extractors/spacy_entity_extractor.py` & `rasa-3.5.5/rasa/nlu/extractors/spacy_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py` & `rasa-3.5.5/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/model.py` & `rasa-3.5.5/rasa/nlu/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/persistor.py` & `rasa-3.5.5/rasa/nlu/persistor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/run.py` & `rasa-3.5.5/rasa/nlu/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/selectors/response_selector.py` & `rasa-3.5.5/rasa/nlu/selectors/response_selector.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/test.py` & `rasa-3.5.5/rasa/nlu/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/tokenizers/jieba_tokenizer.py` & `rasa-3.5.5/rasa/nlu/tokenizers/jieba_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/tokenizers/mitie_tokenizer.py` & `rasa-3.5.5/rasa/nlu/tokenizers/mitie_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/tokenizers/spacy_tokenizer.py` & `rasa-3.5.5/rasa/nlu/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/tokenizers/tokenizer.py` & `rasa-3.5.5/rasa/nlu/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/tokenizers/whitespace_tokenizer.py` & `rasa-3.5.5/rasa/nlu/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/__init__.py` & `rasa-3.5.5/rasa/nlu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/bilou_utils.py` & `rasa-3.5.5/rasa/nlu/utils/bilou_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/hugging_face/registry.py` & `rasa-3.5.5/rasa/nlu/utils/hugging_face/registry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py` & `rasa-3.5.5/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/mitie_utils.py` & `rasa-3.5.5/rasa/nlu/utils/mitie_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/pattern_utils.py` & `rasa-3.5.5/rasa/nlu/utils/pattern_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/nlu/utils/spacy_utils.py` & `rasa-3.5.5/rasa/nlu/utils/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/plugin.py` & `rasa-3.5.5/rasa/plugin.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/server.py` & `rasa-3.5.5/rasa/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,15 +717,16 @@
     @ensure_loaded_agent(app)
     async def retrieve_tracker(request: Request, conversation_id: Text) -> HTTPResponse:
         """Get a dump of a conversation's tracker including its events."""
         verbosity = event_verbosity_parameter(request, EventVerbosity.AFTER_RESTART)
         until_time = rasa.utils.endpoints.float_arg(request, "until")
 
         tracker = await app.ctx.agent.processor.fetch_full_tracker_with_initial_session(
-            conversation_id
+            conversation_id,
+            output_channel=CollectingOutputChannel(),
         )
 
         try:
             if until_time is not None:
                 tracker = tracker.travel_back_in_time(until_time)
 
             state = tracker.current_state(verbosity)
```

### Comparing `rasa-3.5.4/rasa/shared/constants.py` & `rasa-3.5.5/rasa/shared/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/constants.py` & `rasa-3.5.5/rasa/shared/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/conversation.py` & `rasa-3.5.5/rasa/shared/core/conversation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/domain.py` & `rasa-3.5.5/rasa/shared/core/domain.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/events.py` & `rasa-3.5.5/rasa/shared/core/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/generator.py` & `rasa-3.5.5/rasa/shared/core/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/slot_mappings.py` & `rasa-3.5.5/rasa/shared/core/slot_mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,22 +201,24 @@
                 f"Skipping slot extraction because of invalid mapping."
             )
             return False
 
         if (
             mapping_type == SlotMappingType.FROM_INTENT
             and mapping.get(INTENT) is not None
-            and mapping.get(INTENT) not in domain.intents
         ):
-            rasa.shared.utils.io.raise_warning(
-                f"Slot '{slot_name}' uses a 'from_intent' mapping for "
-                f"a non-existent intent '{mapping.get('intent')}'. "
-                f"Skipping slot extraction because of invalid mapping."
-            )
-            return False
+            intent_list = SlotMapping.to_list(mapping.get(INTENT))
+            for intent in intent_list:
+                if intent and intent not in domain.intents:
+                    rasa.shared.utils.io.raise_warning(
+                        f"Slot '{slot_name}' uses a 'from_intent' mapping for "
+                        f"a non-existent intent '{mapping.get('intent')}'. "
+                        f"Skipping slot extraction because of invalid mapping."
+                    )
+                    return False
 
         return True
 
 
 def validate_slot_mappings(domain_slots: Dict[Text, Any]) -> None:
     """Raises InvalidDomain exception if slot mappings are invalid."""
     rasa.shared.utils.io.raise_warning(
```

### Comparing `rasa-3.5.4/rasa/shared/core/slots.py` & `rasa-3.5.5/rasa/shared/core/slots.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/trackers.py` & `rasa-3.5.5/rasa/shared/core/trackers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/loading.py` & `rasa-3.5.5/rasa/shared/core/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/story_reader/story_reader.py` & `rasa-3.5.5/rasa/shared/core/training_data/story_reader/story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/story_reader/story_step_builder.py` & `rasa-3.5.5/rasa/shared/core/training_data/story_reader/story_step_builder.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/story_reader/yaml_story_reader.py` & `rasa-3.5.5/rasa/shared/core/training_data/story_reader/yaml_story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/story_writer/story_writer.py` & `rasa-3.5.5/rasa/shared/core/training_data/story_writer/story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/story_writer/yaml_story_writer.py` & `rasa-3.5.5/rasa/shared/core/training_data/story_writer/yaml_story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/structures.py` & `rasa-3.5.5/rasa/shared/core/training_data/structures.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/visualization.html` & `rasa-3.5.5/rasa/shared/core/training_data/visualization.html`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/core/training_data/visualization.py` & `rasa-3.5.5/rasa/shared/core/training_data/visualization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/data.py` & `rasa-3.5.5/rasa/shared/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/exceptions.py` & `rasa-3.5.5/rasa/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/importers/importer.py` & `rasa-3.5.5/rasa/shared/importers/importer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/importers/multi_project.py` & `rasa-3.5.5/rasa/shared/importers/multi_project.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/importers/rasa.py` & `rasa-3.5.5/rasa/shared/importers/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/importers/utils.py` & `rasa-3.5.5/rasa/shared/importers/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/constants.py` & `rasa-3.5.5/rasa/shared/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/entities_parser.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/entities_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/features.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/features.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/formats/dialogflow.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/formats/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/formats/luis.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/formats/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/formats/rasa.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/formats/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/formats/rasa_yaml.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/formats/rasa_yaml.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/formats/readerwriter.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/formats/readerwriter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/formats/wit.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/formats/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/loading.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/lookup_tables_parser.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/lookup_tables_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/message.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/message.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/schemas/data_schema.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/schemas/data_schema.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/schemas/nlu.yml` & `rasa-3.5.5/rasa/shared/nlu/training_data/schemas/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/schemas/responses.yml` & `rasa-3.5.5/rasa/shared/nlu/training_data/schemas/responses.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/synonyms_parser.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/synonyms_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/training_data.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/training_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/nlu/training_data/util.py` & `rasa-3.5.5/rasa/shared/nlu/training_data/util.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/cli.py` & `rasa-3.5.5/rasa/shared/utils/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from typing import Any, Text, NoReturn
 
 import rasa.shared.utils.io
 
 
 def print_color(*args: Any, color: Text) -> None:
     output = rasa.shared.utils.io.wrap_with_color(*args, color=color)
-    try:
+    stream = sys.stdout
+    if sys.platform == "win32":
         # colorama is used to fix a regression where colors can not be printed on
         # windows. https://github.com/RasaHQ/rasa/issues/7053
         from colorama import AnsiToWin32
 
         stream = AnsiToWin32(sys.stdout).stream
+    try:
         print(output, file=stream)
-    except ImportError:
-        print(output)
+    except BlockingIOError:
+        rasa.shared.utils.io.handle_print_blocking(output)
 
 
 def print_success(*args: Any) -> None:
     print_color(*args, color=rasa.shared.utils.io.bcolors.OKGREEN)
 
 
 def print_info(*args: Any) -> None:
@@ -31,10 +33,9 @@
 
 def print_error(*args: Any) -> None:
     print_color(*args, color=rasa.shared.utils.io.bcolors.FAIL)
 
 
 def print_error_and_exit(message: Text, exit_code: int = 1) -> NoReturn:
     """Print error message and exit the application."""
-
     print_error(message)
     sys.exit(exit_code)
```

### Comparing `rasa-3.5.4/rasa/shared/utils/common.py` & `rasa-3.5.5/rasa/shared/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/io.py` & `rasa-3.5.5/rasa/shared/utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from collections import OrderedDict
 import errno
 import glob
 from hashlib import md5
 from io import StringIO
 import json
 import os
+import sys
 from pathlib import Path
 import re
 from typing import Any, Dict, List, Optional, Text, Type, Union
 import warnings
 import random
 import string
+import portalocker
 
 from ruamel import yaml as yaml
 from ruamel.yaml import RoundTripRepresenter, YAMLError
 from ruamel.yaml.constructor import DuplicateKeyError, BaseConstructor, ScalarNode
 
 from rasa.shared.constants import (
     DEFAULT_LOG_LEVEL,
@@ -53,15 +55,14 @@
 def raise_warning(
     message: Text,
     category: Optional[Type[Warning]] = None,
     docs: Optional[Text] = None,
     **kwargs: Any,
 ) -> None:
     """Emit a `warnings.warn` with sensible defaults and a colored warning msg."""
-
     original_formatter = warnings.formatwarning
 
     def should_show_source_line() -> bool:
         if "stacklevel" not in kwargs:
             if category == UserWarning or category is None:
                 return False
             if category == FutureWarning:
@@ -117,15 +118,14 @@
     mode = "a" if append else "w"
     with open(file_path, mode, encoding=encoding) as file:
         file.write(content)
 
 
 def read_file(filename: Union[Text, Path], encoding: Text = DEFAULT_ENCODING) -> Any:
     """Read text from a file."""
-
     try:
         with open(filename, encoding=encoding) as f:
             return f.read()
     except FileNotFoundError:
         raise FileNotFoundException(
             f"Failed to read file, " f"'{os.path.abspath(filename)}' does not exist."
         )
@@ -149,16 +149,16 @@
         )
 
 
 def list_directory(path: Text) -> List[Text]:
     """Returns all files and folders excluding hidden files.
 
     If the path points to a file, returns the file. This is a recursive
-    implementation returning files in any depth of the path."""
-
+    implementation returning files in any depth of the path.
+    """
     if not isinstance(path, str):
         raise ValueError(
             f"`resource_name` must be a string type. " f"Got `{type(path)}` instead"
         )
 
     if os.path.isfile(path):
         return [path]
@@ -177,29 +177,29 @@
     else:
         raise ValueError(f"Could not locate the resource '{os.path.abspath(path)}'.")
 
 
 def list_files(path: Text) -> List[Text]:
     """Returns all files excluding hidden files.
 
-    If the path points to a file, returns the file."""
-
+    If the path points to a file, returns the file.
+    """
     return [fn for fn in list_directory(path) if os.path.isfile(fn)]
 
 
 def _filename_without_prefix(file: Text) -> Text:
     """Splits of a filenames prefix until after the first ``_``."""
     return "_".join(file.split("_")[1:])
 
 
 def list_subdirectories(path: Text) -> List[Text]:
     """Returns all folders excluding hidden files.
 
-    If the path points to a file, returns an empty list."""
-
+    If the path points to a file, returns an empty list.
+    """
     return [fn for fn in glob.glob(os.path.join(path, "*")) if os.path.isdir(fn)]
 
 
 def deep_container_fingerprint(
     obj: Union[List[Any], Dict[Any, Any], Any], encoding: Text = DEFAULT_ENCODING
 ) -> Text:
     """Calculate a hash which is stable.
@@ -359,37 +359,40 @@
     return yaml_parser.load(content) or {}
 
 
 def _is_ascii(text: Text) -> bool:
     return all(ord(character) < 128 for character in text)
 
 
-def read_yaml_file(filename: Union[Text, Path]) -> Union[List[Any], Dict[Text, Any]]:
+def read_yaml_file(
+    filename: Union[Text, Path], reader_type: Union[Text, List[Text]] = "safe"
+) -> Union[List[Any], Dict[Text, Any]]:
     """Parses a yaml file.
 
     Raises an exception if the content of the file can not be parsed as YAML.
 
     Args:
         filename: The path to the file which should be read.
+        reader_type: Reader type to use. By default "safe" will be used.
 
     Returns:
         Parsed content of the file.
     """
     try:
-        return read_yaml(read_file(filename, DEFAULT_ENCODING))
+        return read_yaml(read_file(filename, DEFAULT_ENCODING), reader_type)
     except (YAMLError, DuplicateKeyError) as e:
         raise YamlSyntaxException(filename, e)
 
 
 def write_yaml(
     data: Any,
     target: Union[Text, Path, StringIO],
     should_preserve_key_order: bool = False,
 ) -> None:
-    """Writes a yaml to the file or to the stream
+    """Writes a yaml to the file or to the stream.
 
     Args:
         data: The data to write.
         target: The path to the file which should be written or a stream object
         should_preserve_key_order: Whether to force preserve key order in `data`.
     """
     _enable_ordered_dict_yaml_dumping()
@@ -485,15 +488,14 @@
     log_level = os.environ.get(ENV_LOG_LEVEL, DEFAULT_LOG_LEVEL)
 
     return log_level in ("ERROR", "WARNING")
 
 
 def create_directory_for_file(file_path: Union[Text, Path]) -> None:
     """Creates any missing parent directories of this file path."""
-
     create_directory(os.path.dirname(file_path))
 
 
 def dump_obj_as_json_to_file(filename: Union[Text, Path], obj: Any) -> None:
     """Dump an object as a json string to a file."""
     write_text_file(json.dumps(obj, ensure_ascii=False, indent=2), filename)
 
@@ -516,80 +518,87 @@
 
     return buffer.getvalue()
 
 
 def create_directory(directory_path: Text) -> None:
     """Creates a directory and its super paths.
 
-    Succeeds even if the path already exists."""
-
+    Succeeds even if the path already exists.
+    """
     try:
         os.makedirs(directory_path)
     except OSError as e:
         # be happy if someone already created the path
         if e.errno != errno.EEXIST:
             raise
 
 
 def raise_deprecation_warning(
     message: Text,
     warn_until_version: Text = NEXT_MAJOR_VERSION_FOR_DEPRECATIONS,
     docs: Optional[Text] = None,
     **kwargs: Any,
 ) -> None:
-    """
-    Thin wrapper around `raise_warning()` to raise a deprecation warning. It requires
+    """Thin wrapper around `raise_warning()` to raise a deprecation warning. It requires
     a version until which we'll warn, and after which the support for the feature will
     be removed.
     """
     if warn_until_version not in message:
         message = f"{message} (will be removed in {warn_until_version})"
 
     # need the correct stacklevel now
     kwargs.setdefault("stacklevel", 3)
     # we're raising a `FutureWarning` instead of a `DeprecationWarning` because
     # we want these warnings to be visible in the terminal of our users
     # https://docs.python.org/3/library/warnings.html#warning-categories
     raise_warning(message, FutureWarning, docs, **kwargs)
 
 
-def read_validated_yaml(filename: Union[Text, Path], schema: Text) -> Any:
+def read_validated_yaml(
+    filename: Union[Text, Path],
+    schema: Text,
+    reader_type: Union[Text, List[Text]] = "safe",
+) -> Any:
     """Validates YAML file content and returns parsed content.
 
     Args:
         filename: The path to the file which should be read.
         schema: The path to the schema file which should be used for validating the
             file content.
+        reader_type: Reader type to use. By default "safe" will be used.
 
     Returns:
         The parsed file content.
 
     Raises:
         YamlValidationException: In case the model configuration doesn't match the
             expected schema.
     """
     content = read_file(filename)
 
     rasa.shared.utils.validation.validate_yaml_schema(content, schema)
-    return read_yaml(content)
+    return read_yaml(content, reader_type)
 
 
-def read_config_file(filename: Union[Path, Text]) -> Dict[Text, Any]:
+def read_config_file(
+    filename: Union[Path, Text], reader_type: Union[Text, List[Text]] = "safe"
+) -> Dict[Text, Any]:
     """Parses a yaml configuration file. Content needs to be a dictionary.
 
     Args:
         filename: The path to the file which should be read.
+        reader_type: Reader type to use. By default "safe" will be used.
 
     Raises:
         YamlValidationException: In case file content is not a `Dict`.
 
     Returns:
         Parsed config file.
     """
-    return read_validated_yaml(filename, CONFIG_SCHEMA_FILE)
+    return read_validated_yaml(filename, CONFIG_SCHEMA_FILE, reader_type)
 
 
 def read_model_configuration(filename: Union[Path, Text]) -> Dict[Text, Any]:
     """Parses a model configuration file.
 
     Args:
         filename: The path to the file which should be read.
@@ -622,7 +631,25 @@
 
     return potential_parent_directory in path
 
 
 def random_string(length: int) -> Text:
     """Returns a random string of given length."""
     return "".join(random.choices(string.ascii_uppercase + string.digits, k=length))
+
+
+def handle_print_blocking(output: Text) -> None:
+    """Handle print blocking (BlockingIOError) by getting the STDOUT lock.
+
+    Args:
+        output: Text to be printed to STDOUT.
+    """
+    # Locking again to obtain STDOUT with a lock.
+    with portalocker.Lock(sys.stdout) as lock:
+        if sys.platform == "win32":
+            # colorama is used to fix a regression where colors can not be printed on
+            # windows. https://github.com/RasaHQ/rasa/issues/7053
+            from colorama import AnsiToWin32
+
+            lock = AnsiToWin32(lock).stream
+
+        print(output, file=lock, flush=True)
```

### Comparing `rasa-3.5.4/rasa/shared/utils/pykwalify_extensions.py` & `rasa-3.5.5/rasa/shared/utils/pykwalify_extensions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/schemas/domain.yml` & `rasa-3.5.5/rasa/shared/utils/schemas/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/schemas/events.py` & `rasa-3.5.5/rasa/shared/utils/schemas/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/schemas/model_config.yml` & `rasa-3.5.5/rasa/shared/utils/schemas/model_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/schemas/stories.yml` & `rasa-3.5.5/rasa/shared/utils/schemas/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/shared/utils/validation.py` & `rasa-3.5.5/rasa/shared/utils/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/telemetry.py` & `rasa-3.5.5/rasa/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/common.py` & `rasa-3.5.5/rasa/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/converter.py` & `rasa-3.5.5/rasa/utils/converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/endpoints.py` & `rasa-3.5.5/rasa/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/io.py` & `rasa-3.5.5/rasa/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/plotting.py` & `rasa-3.5.5/rasa/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/callback.py` & `rasa-3.5.5/rasa/utils/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/constants.py` & `rasa-3.5.5/rasa/utils/tensorflow/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/crf.py` & `rasa-3.5.5/rasa/utils/tensorflow/crf.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/data_generator.py` & `rasa-3.5.5/rasa/utils/tensorflow/data_generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/environment.py` & `rasa-3.5.5/rasa/utils/tensorflow/environment.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/layers.py` & `rasa-3.5.5/rasa/utils/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/layers_utils.py` & `rasa-3.5.5/rasa/utils/tensorflow/layers_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/model_data.py` & `rasa-3.5.5/rasa/utils/tensorflow/model_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/model_data_utils.py` & `rasa-3.5.5/rasa/utils/tensorflow/model_data_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/models.py` & `rasa-3.5.5/rasa/utils/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/rasa_layers.py` & `rasa-3.5.5/rasa/utils/tensorflow/rasa_layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/tensorflow/transformer.py` & `rasa-3.5.5/rasa/utils/tensorflow/transformer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/utils/train_utils.py` & `rasa-3.5.5/rasa/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/rasa/validator.py` & `rasa-3.5.5/rasa/validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.4/PKG-INFO` & `rasa-3.5.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa
-Version: 3.5.4
+Version: 3.5.5
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
@@ -32,35 +32,36 @@
 Requires-Dist: aio-pika (>=6.7.1,<8.2.4)
 Requires-Dist: aiogram (<2.26)
 Requires-Dist: aiohttp (>=3.6,!=3.7.4.post0,<3.9)
 Requires-Dist: apscheduler (>=3.6,<3.10)
 Requires-Dist: attrs (>=19.3,<22.2)
 Requires-Dist: boto3 (>=1.12,<2.0)
 Requires-Dist: cloudpickle (>=1.2,<2.3)
-Requires-Dist: colorama (>=0.4.4,<0.5.0); sys_platform == "win32"
+Requires-Dist: colorama (>=0.4.4,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: colorclass (>=2.2,<2.3)
 Requires-Dist: coloredlogs (>=10,<16)
 Requires-Dist: colorhash (>=1.0.2,<1.3.0)
 Requires-Dist: confluent-kafka (>=1.9.2,<2.0.0)
-Requires-Dist: dask (==2022.10.2); python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: dask (==2022.2.0); python_full_version >= "3.7.0" and python_full_version < "3.8.0"
+Requires-Dist: dask (==2022.10.2) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: dask (==2022.2.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: fbmessenger (>=6.0.0,<6.1.0)
-Requires-Dist: github3.py (>=3.2.0,<3.3.0); extra == "gh-release-notes"
+Requires-Dist: github3.py (>=3.2.0,<3.3.0) ; extra == "gh-release-notes"
 Requires-Dist: google-auth (<3)
-Requires-Dist: jieba (>=0.39,<0.43); extra == "jieba" or extra == "full"
+Requires-Dist: jieba (>=0.39,<0.43) ; extra == "jieba" or extra == "full"
 Requires-Dist: joblib (>=0.15.1,<1.3.0)
 Requires-Dist: jsonpickle (>=1.3,<3.1)
 Requires-Dist: jsonschema (>=3.2,<4.18)
 Requires-Dist: matplotlib (>=3.1,<3.6)
 Requires-Dist: mattermostwrapper (>=2.2,<2.3)
 Requires-Dist: networkx (>=2.4,<2.7)
-Requires-Dist: numpy (>=1.19.2,<1.22.0); python_full_version >= "3.7.0" and python_full_version < "3.8.0"
-Requires-Dist: numpy (>=1.19.2,<1.25.0); python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: numpy (>=1.19.2,<1.22.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
+Requires-Dist: numpy (>=1.19.2,<1.25.0) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: packaging (>=20.0,<21.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
+Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
 Requires-Dist: protobuf (>=3.9.2,<3.20)
 Requires-Dist: psycopg2-binary (>=2.8.2,<2.10.0)
 Requires-Dist: pydantic (<1.10.3)
 Requires-Dist: pydot (>=1.4,<1.5)
 Requires-Dist: pykwalify (>=1.7,<1.9)
 Requires-Dist: pymongo[srv,tls] (>=3.8,<3.11)
@@ -76,37 +77,37 @@
 Requires-Dist: requests (>=2.23,<3.0)
 Requires-Dist: rocketchat_API (>=0.6.31,<1.29.0)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.18.0)
 Requires-Dist: sanic (>=21.12,<21.13)
 Requires-Dist: sanic-cors (>=2.0.0,<2.1.0)
 Requires-Dist: sanic-jwt (>=1.6.0,<2.0.0)
 Requires-Dist: sanic-routing (>=0.7.2,<0.8.0)
-Requires-Dist: scikit-learn (>=0.22,<1.1); python_full_version >= "3.7.0" and python_full_version < "3.8.0"
-Requires-Dist: scikit-learn (>=0.22,<1.2); python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: scipy (>=1.4.1,<1.8.0); python_full_version >= "3.7.0" and python_full_version < "3.8.0"
-Requires-Dist: scipy (>=1.4.1,<1.9.0); python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: sentencepiece[sentencepiece] (>=0.1.96,<0.2.0); extra == "transformers" or extra == "full"
+Requires-Dist: scikit-learn (>=0.22,<1.1) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
+Requires-Dist: scikit-learn (>=0.22,<1.2) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: scipy (>=1.4.1,<1.8.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
+Requires-Dist: scipy (>=1.4.1,<1.9.0) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: sentencepiece[sentencepiece] (>=0.1.96,<0.2.0) ; extra == "transformers" or extra == "full"
 Requires-Dist: sentry-sdk (>=0.17.0,<1.15.0)
 Requires-Dist: setuptools (>=41.0.0)
 Requires-Dist: sklearn-crfsuite (>=0.3,<0.4)
 Requires-Dist: slack-sdk (>=3.19.2,<4.0.0)
-Requires-Dist: spacy (>=3.1,<3.5); (sys_platform != "darwin" or platform_machine != "arm64") and (extra == "spacy" or extra == "full")
-Requires-Dist: spacy (>=3.4,<4.0); (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "spacy" or extra == "full")
+Requires-Dist: spacy (>=3.1,<3.5) ; (sys_platform != "darwin" or platform_machine != "arm64") and (extra == "spacy" or extra == "full")
+Requires-Dist: spacy (>=3.4,<4.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "spacy" or extra == "full")
 Requires-Dist: tarsafe (>=0.0.3,<0.0.4)
-Requires-Dist: tensorflow (==2.11.0); sys_platform != "darwin" or platform_machine != "arm64"
+Requires-Dist: tensorflow (==2.11.0) ; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: tensorflow-addons (>=0.18,<0.20)
-Requires-Dist: tensorflow-cpu-aws (==2.11.0); sys_platform == "linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
-Requires-Dist: tensorflow-intel (==2.11.0); sys_platform == "win32"
-Requires-Dist: tensorflow-macos (==2.11.0); sys_platform == "darwin" and platform_machine == "arm64"
-Requires-Dist: tensorflow-metal (==0.5.1); (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "metal")
-Requires-Dist: tensorflow-text (==2.11.0); sys_platform != "win32" and platform_machine != "arm64"
+Requires-Dist: tensorflow-cpu-aws (==2.11.0) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
+Requires-Dist: tensorflow-intel (==2.11.0) ; sys_platform == "win32"
+Requires-Dist: tensorflow-macos (==2.11.0) ; sys_platform == "darwin" and platform_machine == "arm64"
+Requires-Dist: tensorflow-metal (==0.5.1) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "metal")
+Requires-Dist: tensorflow-text (==2.11.0) ; sys_platform != "win32" and platform_machine != "arm64"
 Requires-Dist: tensorflow_hub (>=0.12.0,<0.13.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tqdm (>=4.31,<5.0)
-Requires-Dist: transformers (>=4.13.0,<=4.26.0); extra == "transformers" or extra == "full"
+Requires-Dist: transformers (>=4.13.0,<=4.26.0) ; extra == "transformers" or extra == "full"
 Requires-Dist: twilio (>=6.26,<7.15)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Requires-Dist: typing-utils (>=0.1.0,<0.2.0)
 Requires-Dist: ujson (>=1.35,<6.0)
 Requires-Dist: webexteamssdk (>=1.1.1,<1.7.0)
 Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Documentation, https://rasa.com/docs
@@ -225,14 +226,19 @@
 
 ### Installing Poetry
 
 Rasa uses Poetry for packaging and dependency management. If you want to build it from source,
 you have to install Poetry first. Please follow
 [the official guide](https://python-poetry.org/docs/#installation) to see all possible options.
 
+To update an existing poetry version to the [version](.github/poetry_version.txt), currently used in rasa, run:
+```shell
+    poetry self update <version>
+```
+
 ### Managing environments
 
 The official [Poetry guide](https://python-poetry.org/docs/managing-environments/) suggests to use
 [pyenv](https://github.com/pyenv/pyenv) or any other similar tool to easily switch between Python versions.
 This is how it can be done:
 
 ```bash
```

