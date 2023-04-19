# Comparing `tmp/spellbot-8.9.1.tar.gz` & `tmp/spellbot-8.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spellbot-8.9.1.tar", max compression
+gzip compressed data, was "spellbot-8.9.3.tar", max compression
```

## Comparing `spellbot-8.9.1.tar` & `spellbot-8.9.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-8.9.1/LICENSE.md
--rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-8.9.1/README.md
--rw-r--r--   0        0        0     3341 2023-04-18 22:54:00.394418 spellbot-8.9.1/pyproject.toml
--rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-8.9.1/src/spellbot/__init__.py
--rw-r--r--   0        0        0     1801 2023-04-18 21:36:17.604229 spellbot-8.9.1/src/spellbot/_version.py
--rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-8.9.1/src/spellbot/actions/__init__.py
--rw-r--r--   0        0        0    14123 2023-04-18 21:36:17.604426 spellbot-8.9.1/src/spellbot/actions/admin_action.py
--rw-r--r--   0        0        0     3567 2023-04-18 21:36:17.604506 spellbot-8.9.1/src/spellbot/actions/base_action.py
--rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-8.9.1/src/spellbot/actions/block_action.py
--rw-r--r--   0        0        0     1542 2023-04-18 21:36:17.604645 spellbot-8.9.1/src/spellbot/actions/config_action.py
--rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.604693 spellbot-8.9.1/src/spellbot/actions/leave_action.py
--rw-r--r--   0        0        0    17124 2023-04-18 21:36:17.604820 spellbot-8.9.1/src/spellbot/actions/lfg_action.py
--rw-r--r--   0        0        0     3120 2023-04-18 21:36:17.604898 spellbot-8.9.1/src/spellbot/actions/score_action.py
--rw-r--r--   0        0        0     7402 2023-04-18 21:36:17.604981 spellbot-8.9.1/src/spellbot/actions/tasks_action.py
--rw-r--r--   0        0        0      943 2023-04-18 21:36:17.605035 spellbot-8.9.1/src/spellbot/actions/verify_action.py
--rw-r--r--   0        0        0     3860 2023-04-18 21:36:17.605103 spellbot-8.9.1/src/spellbot/actions/watch_action.py
--rw-r--r--   0        0        0     4456 2023-04-18 21:36:17.605183 spellbot-8.9.1/src/spellbot/cli.py
--rw-r--r--   0        0        0     6425 2023-04-18 21:36:17.605285 spellbot-8.9.1/src/spellbot/client.py
--rw-r--r--   0        0        0     2083 2023-04-18 21:36:17.605376 spellbot-8.9.1/src/spellbot/cogs/__init__.py
--rw-r--r--   0        0        0     1971 2023-04-18 22:08:37.549352 spellbot-8.9.1/src/spellbot/cogs/about_cog.py
--rw-r--r--   0        0        0     9846 2023-04-18 21:36:17.605517 spellbot-8.9.1/src/spellbot/cogs/admin_cog.py
--rw-r--r--   0        0        0     1531 2023-04-18 21:36:17.605622 spellbot-8.9.1/src/spellbot/cogs/block_cog.py
--rw-r--r--   0        0        0     1701 2023-04-18 21:36:17.605683 spellbot-8.9.1/src/spellbot/cogs/config_cog.py
--rw-r--r--   0        0        0     1602 2023-04-18 21:36:17.605748 spellbot-8.9.1/src/spellbot/cogs/events_cog.py
--rw-r--r--   0        0        0     1180 2023-04-18 21:36:17.605806 spellbot-8.9.1/src/spellbot/cogs/leave_cog.py
--rw-r--r--   0        0        0     1930 2023-04-18 21:36:17.605872 spellbot-8.9.1/src/spellbot/cogs/lfg_cog.py
--rw-r--r--   0        0        0     3071 2023-04-18 21:36:17.605938 spellbot-8.9.1/src/spellbot/cogs/owner_cog.py
--rw-r--r--   0        0        0     2166 2023-04-18 21:36:17.605998 spellbot-8.9.1/src/spellbot/cogs/score_cog.py
--rw-r--r--   0        0        0     1106 2023-04-18 21:36:17.606052 spellbot-8.9.1/src/spellbot/cogs/sync_cog.py
--rw-r--r--   0        0        0     2224 2023-04-18 21:36:17.606117 spellbot-8.9.1/src/spellbot/cogs/tasks_cog.py
--rw-r--r--   0        0        0     1642 2023-04-18 21:36:17.606166 spellbot-8.9.1/src/spellbot/cogs/verify_cog.py
--rw-r--r--   0        0        0     2559 2023-04-18 21:36:17.606227 spellbot-8.9.1/src/spellbot/cogs/watch_cog.py
--rw-r--r--   0        0        0     4573 2023-04-18 21:36:17.606307 spellbot-8.9.1/src/spellbot/database.py
--rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-8.9.1/src/spellbot/environment.py
--rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.606418 spellbot-8.9.1/src/spellbot/errors.py
--rw-r--r--   0        0        0      931 2023-04-18 21:36:17.606470 spellbot-8.9.1/src/spellbot/logs.py
--rw-r--r--   0        0        0     4647 2023-04-18 21:36:17.606533 spellbot-8.9.1/src/spellbot/metrics.py
--rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-8.9.1/src/spellbot/migrations/alembic.ini
--rw-r--r--   0        0        0     1622 2023-04-18 21:36:17.606704 spellbot-8.9.1/src/spellbot/migrations/env.py
--rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-8.9.1/src/spellbot/migrations/script.py.mako
--rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-8.9.1/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
--rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-8.9.1/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
--rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-8.9.1/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
--rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-8.9.1/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
--rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-8.9.1/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
--rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-8.9.1/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
--rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-8.9.1/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
--rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-8.9.1/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
--rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-8.9.1/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
--rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-8.9.1/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
--rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-8.9.1/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
--rw-r--r--   0        0        0     1261 2023-04-18 21:36:17.607532 spellbot-8.9.1/src/spellbot/models/__init__.py
--rw-r--r--   0        0        0     3172 2023-04-18 21:36:17.607622 spellbot-8.9.1/src/spellbot/models/award.py
--rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.607688 spellbot-8.9.1/src/spellbot/models/base.py
--rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-8.9.1/src/spellbot/models/block.py
--rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-8.9.1/src/spellbot/models/channel.py
--rw-r--r--   0        0        0     1059 2023-04-18 21:36:17.607885 spellbot-8.9.1/src/spellbot/models/config.py
--rw-r--r--   0        0        0    10471 2023-04-18 21:36:17.607972 spellbot-8.9.1/src/spellbot/models/game.py
--rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-8.9.1/src/spellbot/models/guild.py
--rw-r--r--   0        0        0      896 2023-04-18 21:36:17.608085 spellbot-8.9.1/src/spellbot/models/play.py
--rw-r--r--   0        0        0     3656 2023-04-18 21:36:17.608138 spellbot-8.9.1/src/spellbot/models/user.py
--rw-r--r--   0        0        0      740 2023-04-18 21:36:17.608210 spellbot-8.9.1/src/spellbot/models/verify.py
--rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-8.9.1/src/spellbot/models/watch.py
--rw-r--r--   0        0        0    17438 2023-04-18 22:53:49.516511 spellbot-8.9.1/src/spellbot/operations.py
--rw-r--r--   0        0        0     1051 2023-04-18 21:36:17.608469 spellbot-8.9.1/src/spellbot/services/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-18 21:36:17.608528 spellbot-8.9.1/src/spellbot/services/awards.py
--rw-r--r--   0        0        0     4898 2023-04-18 21:36:17.608610 spellbot-8.9.1/src/spellbot/services/channels.py
--rw-r--r--   0        0        0     1554 2023-04-18 21:36:17.608676 spellbot-8.9.1/src/spellbot/services/configs.py
--rw-r--r--   0        0        0    13240 2023-04-18 21:36:17.608775 spellbot-8.9.1/src/spellbot/services/games.py
--rw-r--r--   0        0        0     4828 2023-04-18 21:36:17.608845 spellbot-8.9.1/src/spellbot/services/guilds.py
--rw-r--r--   0        0        0     7516 2023-04-18 21:36:17.608922 spellbot-8.9.1/src/spellbot/services/plays.py
--rw-r--r--   0        0        0     5369 2023-04-18 21:36:17.608981 spellbot-8.9.1/src/spellbot/services/users.py
--rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.609034 spellbot-8.9.1/src/spellbot/services/verifies.py
--rw-r--r--   0        0        0      502 2023-04-18 21:36:17.609093 spellbot-8.9.1/src/spellbot/services/watches.py
--rw-r--r--   0        0        0     3770 2023-04-18 21:36:17.609161 spellbot-8.9.1/src/spellbot/settings.py
--rw-r--r--   0        0        0     2300 2023-04-18 21:36:17.609223 spellbot-8.9.1/src/spellbot/spelltable.py
--rw-r--r--   0        0        0    10441 2023-04-18 22:53:49.516743 spellbot-8.9.1/src/spellbot/utils.py
--rw-r--r--   0        0        0      251 2023-04-18 21:36:17.609422 spellbot-8.9.1/src/spellbot/views/__init__.py
--rw-r--r--   0        0        0      294 2023-04-18 21:36:17.609477 spellbot-8.9.1/src/spellbot/views/base_view.py
--rw-r--r--   0        0        0     3881 2023-04-18 21:36:17.609557 spellbot-8.9.1/src/spellbot/views/lfg_view.py
--rw-r--r--   0        0        0     2413 2023-04-18 21:36:17.609615 spellbot-8.9.1/src/spellbot/views/setup_view.py
--rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-8.9.1/src/spellbot/web/__init__.py
--rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-8.9.1/src/spellbot/web/api/__init__.py
--rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-8.9.1/src/spellbot/web/api/ping.py
--rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-8.9.1/src/spellbot/web/api/record.py
--rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-8.9.1/src/spellbot/web/builder.py
--rw-r--r--   0        0        0      647 2023-04-18 21:36:17.610025 spellbot-8.9.1/src/spellbot/web/server.py
--rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-8.9.1/src/spellbot/web/templates/channel_record.html.j2
--rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-8.9.1/src/spellbot/web/templates/record.css
--rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-8.9.1/src/spellbot/web/templates/record_base.html.j2
--rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-8.9.1/src/spellbot/web/templates/table2CSV.js
--rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-8.9.1/src/spellbot/web/templates/user_record.html.j2
--rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 spellbot-8.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-8.9.3/LICENSE.md
+-rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-8.9.3/README.md
+-rw-r--r--   0        0        0     3274 2023-04-19 22:52:42.224281 spellbot-8.9.3/pyproject.toml
+-rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-8.9.3/src/spellbot/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-18 21:36:17.604229 spellbot-8.9.3/src/spellbot/_version.py
+-rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-8.9.3/src/spellbot/actions/__init__.py
+-rw-r--r--   0        0        0    14123 2023-04-18 21:36:17.604426 spellbot-8.9.3/src/spellbot/actions/admin_action.py
+-rw-r--r--   0        0        0     3567 2023-04-18 21:36:17.604506 spellbot-8.9.3/src/spellbot/actions/base_action.py
+-rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-8.9.3/src/spellbot/actions/block_action.py
+-rw-r--r--   0        0        0     1542 2023-04-18 21:36:17.604645 spellbot-8.9.3/src/spellbot/actions/config_action.py
+-rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.604693 spellbot-8.9.3/src/spellbot/actions/leave_action.py
+-rw-r--r--   0        0        0    17124 2023-04-18 21:36:17.604820 spellbot-8.9.3/src/spellbot/actions/lfg_action.py
+-rw-r--r--   0        0        0     3124 2023-04-19 04:04:51.454273 spellbot-8.9.3/src/spellbot/actions/score_action.py
+-rw-r--r--   0        0        0     7402 2023-04-18 21:36:17.604981 spellbot-8.9.3/src/spellbot/actions/tasks_action.py
+-rw-r--r--   0        0        0      943 2023-04-18 21:36:17.605035 spellbot-8.9.3/src/spellbot/actions/verify_action.py
+-rw-r--r--   0        0        0     3860 2023-04-18 21:36:17.605103 spellbot-8.9.3/src/spellbot/actions/watch_action.py
+-rw-r--r--   0        0        0     4456 2023-04-18 21:36:17.605183 spellbot-8.9.3/src/spellbot/cli.py
+-rw-r--r--   0        0        0     6425 2023-04-18 21:36:17.605285 spellbot-8.9.3/src/spellbot/client.py
+-rw-r--r--   0        0        0     2082 2023-04-19 04:04:51.454571 spellbot-8.9.3/src/spellbot/cogs/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-18 22:08:37.549352 spellbot-8.9.3/src/spellbot/cogs/about_cog.py
+-rw-r--r--   0        0        0     9846 2023-04-18 21:36:17.605517 spellbot-8.9.3/src/spellbot/cogs/admin_cog.py
+-rw-r--r--   0        0        0     1531 2023-04-18 21:36:17.605622 spellbot-8.9.3/src/spellbot/cogs/block_cog.py
+-rw-r--r--   0        0        0     1701 2023-04-18 21:36:17.605683 spellbot-8.9.3/src/spellbot/cogs/config_cog.py
+-rw-r--r--   0        0        0     1602 2023-04-18 21:36:17.605748 spellbot-8.9.3/src/spellbot/cogs/events_cog.py
+-rw-r--r--   0        0        0     1180 2023-04-18 21:36:17.605806 spellbot-8.9.3/src/spellbot/cogs/leave_cog.py
+-rw-r--r--   0        0        0     1930 2023-04-18 21:36:17.605872 spellbot-8.9.3/src/spellbot/cogs/lfg_cog.py
+-rw-r--r--   0        0        0     3071 2023-04-18 21:36:17.605938 spellbot-8.9.3/src/spellbot/cogs/owner_cog.py
+-rw-r--r--   0        0        0     2166 2023-04-18 21:36:17.605998 spellbot-8.9.3/src/spellbot/cogs/score_cog.py
+-rw-r--r--   0        0        0     1106 2023-04-18 21:36:17.606052 spellbot-8.9.3/src/spellbot/cogs/sync_cog.py
+-rw-r--r--   0        0        0     2224 2023-04-18 21:36:17.606117 spellbot-8.9.3/src/spellbot/cogs/tasks_cog.py
+-rw-r--r--   0        0        0     1642 2023-04-18 21:36:17.606166 spellbot-8.9.3/src/spellbot/cogs/verify_cog.py
+-rw-r--r--   0        0        0     2559 2023-04-18 21:36:17.606227 spellbot-8.9.3/src/spellbot/cogs/watch_cog.py
+-rw-r--r--   0        0        0     4573 2023-04-18 21:36:17.606307 spellbot-8.9.3/src/spellbot/database.py
+-rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-8.9.3/src/spellbot/environment.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.606418 spellbot-8.9.3/src/spellbot/errors.py
+-rw-r--r--   0        0        0      931 2023-04-18 21:36:17.606470 spellbot-8.9.3/src/spellbot/logs.py
+-rw-r--r--   0        0        0     4647 2023-04-18 21:36:17.606533 spellbot-8.9.3/src/spellbot/metrics.py
+-rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-8.9.3/src/spellbot/migrations/alembic.ini
+-rw-r--r--   0        0        0     1622 2023-04-18 21:36:17.606704 spellbot-8.9.3/src/spellbot/migrations/env.py
+-rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-8.9.3/src/spellbot/migrations/script.py.mako
+-rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-8.9.3/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
+-rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-8.9.3/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
+-rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-8.9.3/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
+-rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-8.9.3/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
+-rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-8.9.3/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
+-rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-8.9.3/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
+-rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-8.9.3/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
+-rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-8.9.3/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
+-rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-8.9.3/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
+-rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-8.9.3/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
+-rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-8.9.3/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
+-rw-r--r--   0        0        0     1261 2023-04-18 21:36:17.607532 spellbot-8.9.3/src/spellbot/models/__init__.py
+-rw-r--r--   0        0        0     3172 2023-04-18 21:36:17.607622 spellbot-8.9.3/src/spellbot/models/award.py
+-rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.607688 spellbot-8.9.3/src/spellbot/models/base.py
+-rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-8.9.3/src/spellbot/models/block.py
+-rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-8.9.3/src/spellbot/models/channel.py
+-rw-r--r--   0        0        0     1059 2023-04-18 21:36:17.607885 spellbot-8.9.3/src/spellbot/models/config.py
+-rw-r--r--   0        0        0    10471 2023-04-18 21:36:17.607972 spellbot-8.9.3/src/spellbot/models/game.py
+-rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-8.9.3/src/spellbot/models/guild.py
+-rw-r--r--   0        0        0      896 2023-04-18 21:36:17.608085 spellbot-8.9.3/src/spellbot/models/play.py
+-rw-r--r--   0        0        0     3656 2023-04-18 21:36:17.608138 spellbot-8.9.3/src/spellbot/models/user.py
+-rw-r--r--   0        0        0      740 2023-04-18 21:36:17.608210 spellbot-8.9.3/src/spellbot/models/verify.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-8.9.3/src/spellbot/models/watch.py
+-rw-r--r--   0        0        0    17438 2023-04-18 22:53:49.516511 spellbot-8.9.3/src/spellbot/operations.py
+-rw-r--r--   0        0        0     1051 2023-04-18 21:36:17.608469 spellbot-8.9.3/src/spellbot/services/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-18 21:36:17.608528 spellbot-8.9.3/src/spellbot/services/awards.py
+-rw-r--r--   0        0        0     4900 2023-04-19 04:04:51.454821 spellbot-8.9.3/src/spellbot/services/channels.py
+-rw-r--r--   0        0        0     1553 2023-04-19 04:04:51.455067 spellbot-8.9.3/src/spellbot/services/configs.py
+-rw-r--r--   0        0        0    13239 2023-04-19 22:44:57.751042 spellbot-8.9.3/src/spellbot/services/games.py
+-rw-r--r--   0        0        0     4830 2023-04-19 04:04:51.455764 spellbot-8.9.3/src/spellbot/services/guilds.py
+-rw-r--r--   0        0        0     7516 2023-04-18 21:36:17.608922 spellbot-8.9.3/src/spellbot/services/plays.py
+-rw-r--r--   0        0        0     5372 2023-04-19 04:04:51.455984 spellbot-8.9.3/src/spellbot/services/users.py
+-rw-r--r--   0        0        0     1660 2023-04-19 04:04:51.456240 spellbot-8.9.3/src/spellbot/services/verifies.py
+-rw-r--r--   0        0        0      502 2023-04-18 21:36:17.609093 spellbot-8.9.3/src/spellbot/services/watches.py
+-rw-r--r--   0        0        0     3770 2023-04-18 21:36:17.609161 spellbot-8.9.3/src/spellbot/settings.py
+-rw-r--r--   0        0        0     2300 2023-04-18 21:36:17.609223 spellbot-8.9.3/src/spellbot/spelltable.py
+-rw-r--r--   0        0        0    10441 2023-04-18 22:53:49.516743 spellbot-8.9.3/src/spellbot/utils.py
+-rw-r--r--   0        0        0      251 2023-04-18 21:36:17.609422 spellbot-8.9.3/src/spellbot/views/__init__.py
+-rw-r--r--   0        0        0      294 2023-04-18 21:36:17.609477 spellbot-8.9.3/src/spellbot/views/base_view.py
+-rw-r--r--   0        0        0     3881 2023-04-18 21:36:17.609557 spellbot-8.9.3/src/spellbot/views/lfg_view.py
+-rw-r--r--   0        0        0     2413 2023-04-18 21:36:17.609615 spellbot-8.9.3/src/spellbot/views/setup_view.py
+-rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-8.9.3/src/spellbot/web/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-8.9.3/src/spellbot/web/api/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-8.9.3/src/spellbot/web/api/ping.py
+-rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-8.9.3/src/spellbot/web/api/record.py
+-rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-8.9.3/src/spellbot/web/builder.py
+-rw-r--r--   0        0        0      647 2023-04-18 21:36:17.610025 spellbot-8.9.3/src/spellbot/web/server.py
+-rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-8.9.3/src/spellbot/web/templates/channel_record.html.j2
+-rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-8.9.3/src/spellbot/web/templates/record.css
+-rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-8.9.3/src/spellbot/web/templates/record_base.html.j2
+-rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-8.9.3/src/spellbot/web/templates/table2CSV.js
+-rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-8.9.3/src/spellbot/web/templates/user_record.html.j2
+-rw-r--r--   0        0        0    12969 1970-01-01 00:00:00.000000 spellbot-8.9.3/PKG-INFO
```

### Comparing `spellbot-8.9.1/LICENSE.md` & `spellbot-8.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/README.md` & `spellbot-8.9.3/README.md`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/pyproject.toml` & `spellbot-8.9.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -69,84 +69,81 @@
 license = 'MIT'
 name = 'spellbot'
 packages = [
   {include = "spellbot", from = "src"},
 ]
 readme = 'README.md'
 repository = 'https://github.com/lexicalunit/spellbot'
-version = "8.9.1"
+version = "8.9.3"
 
 [tool.poetry.dependencies]
-Babel = "^2.11.0"
-PyYAML = "^6.0"
-SQLAlchemy = "^1.4.44"
-SQLAlchemy-Utils = "^0.39.0"
-aiohttp = "^3.8.1"
-aiohttp-jinja2 = "^1.5"
+aiohttp = "^3.8.4"
+aiohttp-jinja2 = "^1.5.1"
 aiohttp-retry = "^2.8.3"
-alembic = "^1.8.0"
-asgiref = "^3.5.2"
+alembic = "^1.10.3"
+asgiref = "^3.6.0"
+babel = "^2.12.1"
 certifi = "^2022.12.7"
-charset-normalizer = "2.1.1"
 click = "^8.1.3"
 coloredlogs = "^15.0.1"
-datadog = "^0.44.0"
-ddtrace = "^1.6.1"
-"discord.py" = "^2.1.0"
-dunamai = "^1.14.1"
+datadog = "^0.45.0"
+ddtrace = "^1.12.0"
+discord-py = "^2.2.2"
+dunamai = "^1.16.0"
 expiringdict = "^1.2.2"
 gunicorn = "^20.1.0"
-humanize = "^4.3.0"
-hupper = "^1.10.3"
-importlib-resources = "^5.10.2"
-packaging = "22.0"
-psycopg2-binary = "^2.9.3"
-python = '>=3.10,<4'
+humanize = "^4.6.0"
+hupper = "^1.12"
+importlib-resources = "^5.12.0"
+packaging = "^23.1"
+psycopg2-binary = "^2.9.6"
+python = ">=3.10,<4"
 python-dateutil = "^2.8.2"
-python-dotenv = "^0.21.0"
-pytz = "^2022.6"
-requests = "2.28.1"
-supervisor = "^4.2.4"
+python-dotenv = "^1.0.0"
+pytz = "^2023.3"
+pyyaml = "^6.0"
+requests = "^2.28.2"
+sqlalchemy = "^2.0.9"
+sqlalchemy-utils = "^0.41.0"
+supervisor = "^4.2.5"
 toml = "^0.10.2"
 uvloop = "^0.17.0"
-wrapt = "^1.14.1"
+wrapt = "^1.15.0"
 
-[tool.poetry.dev-dependencies]
-Faker = "^15"
-GitPython = "^3"
-black = "^22"
+[tool.poetry.scripts]
+spellbot = 'spellbot:main'
+
+[tool.poetry.group.dev.dependencies]
+black = "^23"
 callee = "^0"
 coverage = "^7"
 exceptiongroup = "^1"
 factory-boy = "^3"
-flake8-print = "^5"
-isort = "^5"
+faker = "^18"
+gitpython = "^3"
 pexpect = "^4"
 ptyprocess = "^0"
-pylic = "^3"
-pylint = "2.15.9"
+pylic = "^3.5.0"
+pylint = "2.17.2"
 pyright = "^1"
 pytest = "^7"
 pytest-aiohttp = "^1"
 pytest-asyncio = "^0"
 pytest-cov = "^4"
 pytest-freezegun = "^0"
 pytest-mock = "^3"
 ruff = "^0"
 shellingham = "^1"
 sqlalchemy-stubs = "^0"
-syrupy = "^3"
+syrupy = "^4"
 tomli = "^2"
 tomlkit = "^0"
-types-PyYAML = "^6.0"
-types-freezegun = "^1.1"
-types-python-dateutil = "^2.8"
-types-pytz = "^2022.6.0.1"
-types-toml = "^0.10"
+types-freezegun = "^1"
+types-python-dateutil = "^2"
+types-pytz = "^2023"
+types-pyyaml = "^6"
+types-toml = "^0"
 virtualenv = "^20"
 
-[tool.poetry.scripts]
-spellbot = 'spellbot:main'
-
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.8"]
```

### Comparing `spellbot-8.9.1/src/spellbot/_version.py` & `spellbot-8.9.3/src/spellbot/_version.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/__init__.py` & `spellbot-8.9.3/src/spellbot/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/admin_action.py` & `spellbot-8.9.3/src/spellbot/actions/admin_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/base_action.py` & `spellbot-8.9.3/src/spellbot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/block_action.py` & `spellbot-8.9.3/src/spellbot/actions/block_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/config_action.py` & `spellbot-8.9.3/src/spellbot/actions/config_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/leave_action.py` & `spellbot-8.9.3/src/spellbot/actions/leave_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/lfg_action.py` & `spellbot-8.9.3/src/spellbot/actions/lfg_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/score_action.py` & `spellbot-8.9.3/src/spellbot/actions/score_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
         guild_xid = self.interaction.guild_id
 
         data = await self.services.plays.top_records(guild_xid, channel_xid, monthly, ago)
 
         settings = Settings()
         embed = discord.Embed()
         embed.set_thumbnail(url=settings.ICO_URL)
-        range = f"{ago} months ago" if ago else "this month" if monthly else "all time"
-        embed.title = f"Top players in #{channel_name} ({range})"
+        range_s = f"{ago} months ago" if ago else "this month" if monthly else "all time"
+        embed.title = f"Top players in #{channel_name} ({range_s})"
         description = ""
         description += "Rank \xa0\xa0\xa0 Games \xa0\xa0\xa0 Player\n"
         for rank, datum in enumerate(data):
             user_xid, count = datum
             description += f"{rank+1:\xa0>6}\xa0{count:\xa0>20}\xa0\xa0\xa0<@{user_xid}>\n"
         embed.description = description
         embed.color = settings.EMBED_COLOR
```

### Comparing `spellbot-8.9.1/src/spellbot/actions/tasks_action.py` & `spellbot-8.9.3/src/spellbot/actions/tasks_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/verify_action.py` & `spellbot-8.9.3/src/spellbot/actions/verify_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/actions/watch_action.py` & `spellbot-8.9.3/src/spellbot/actions/watch_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cli.py` & `spellbot-8.9.3/src/spellbot/cli.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/client.py` & `spellbot-8.9.3/src/spellbot/client.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/__init__.py` & `spellbot-8.9.3/src/spellbot/cogs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 ]
 
 
 async def load_all_cogs(bot: AutoShardedBot) -> AutoShardedBot:
     # iterate through the modules in the current package
     package_dir = Path(__file__).resolve().parent
     for info in iter_modules([str(package_dir)]):
-
         # import the module and iterate through its attributes
         module = import_module(f"{__name__}.{info.name}")
         for attribute_name in dir(module):  # pragma: no cover
             attribute = getattr(module, attribute_name)
 
             # Only load cogs in this module if they're exported
             if (
```

### Comparing `spellbot-8.9.1/src/spellbot/cogs/about_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/about_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/admin_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/admin_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/block_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/block_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/config_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/config_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/events_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/events_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/leave_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/leave_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/lfg_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/lfg_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/owner_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/owner_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/score_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/score_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/sync_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/sync_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/tasks_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/tasks_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/verify_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/verify_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/cogs/watch_cog.py` & `spellbot-8.9.3/src/spellbot/cogs/watch_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/database.py` & `spellbot-8.9.3/src/spellbot/database.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/errors.py` & `spellbot-8.9.3/src/spellbot/errors.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/logs.py` & `spellbot-8.9.3/src/spellbot/logs.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/metrics.py` & `spellbot-8.9.3/src/spellbot/metrics.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/alembic.ini` & `spellbot-8.9.3/src/spellbot/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/env.py` & `spellbot-8.9.3/src/spellbot/migrations/env.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py` & `spellbot-8.9.3/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/__init__.py` & `spellbot-8.9.3/src/spellbot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/award.py` & `spellbot-8.9.3/src/spellbot/models/award.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/base.py` & `spellbot-8.9.3/src/spellbot/models/base.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/block.py` & `spellbot-8.9.3/src/spellbot/models/block.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/channel.py` & `spellbot-8.9.3/src/spellbot/models/channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/config.py` & `spellbot-8.9.3/src/spellbot/models/config.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/game.py` & `spellbot-8.9.3/src/spellbot/models/game.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/guild.py` & `spellbot-8.9.3/src/spellbot/models/guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/play.py` & `spellbot-8.9.3/src/spellbot/models/play.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/user.py` & `spellbot-8.9.3/src/spellbot/models/user.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/verify.py` & `spellbot-8.9.3/src/spellbot/models/verify.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/models/watch.py` & `spellbot-8.9.3/src/spellbot/models/watch.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/operations.py` & `spellbot-8.9.3/src/spellbot/operations.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/services/__init__.py` & `spellbot-8.9.3/src/spellbot/services/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/services/awards.py` & `spellbot-8.9.3/src/spellbot/services/awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/services/channels.py` & `spellbot-8.9.3/src/spellbot/services/channels.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,18 @@
             "name": name,
             "updated_at": datetime.utcnow(),
         }
         upsert = insert(Channel).values(**values)
         upsert = upsert.on_conflict_do_update(
             index_elements=[Channel.xid],
             index_where=Channel.xid == values["xid"],
-            set_=dict(
-                name=upsert.excluded.name,
-                updated_at=upsert.excluded.updated_at,
-            ),
+            set_={
+                "name": upsert.excluded.name,
+                "updated_at": upsert.excluded.updated_at,
+            },
         )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
 
         channel = DatabaseSession.query(Channel).filter(Channel.xid == channel.id).one()
         return channel.to_dict()
```

### Comparing `spellbot-8.9.1/src/spellbot/services/configs.py` & `spellbot-8.9.3/src/spellbot/services/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,14 @@
         upsert = insert(Config).values(**values)
         upsert = upsert.on_conflict_do_update(
             constraint="configs_pkey",
             index_where=and_(
                 Config.guild_xid == values["guild_xid"],
                 Config.user_xid == values["user_xid"],
             ),
-            set_=dict(power_level=upsert.excluded.power_level),
+            set_={"power_level": upsert.excluded.power_level},
         )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
         data = self._select(guild_xid, user_xid)
         assert data is not None
         return data
```

### Comparing `spellbot-8.9.1/src/spellbot/services/games.py` & `spellbot-8.9.3/src/spellbot/services/games.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Optional
 
 import discord
 from asgiref.sync import sync_to_async
 from ddtrace import tracer
 from sqlalchemy import update
 from sqlalchemy.dialects.postgresql import insert
+from sqlalchemy.orm import aliased
 from sqlalchemy.sql.expression import and_, asc, column, or_, select
 from sqlalchemy.sql.functions import count
 
 from ..database import DatabaseSession
 from ..models import Block, Game, GameStatus, Play, User, UserAward, Watch
 from ..settings import Settings
 
@@ -140,58 +141,54 @@
         friends: list[int],
         seats: int,
         format: int,
     ) -> Optional[Game]:
         required_seats = 1 + len(friends)
         inner = (
             select(
-                [
-                    Game,
-                    User.xid.label("users_xid"),
-                    count(User.xid).over(partition_by=Game.id).label("player_count"),
-                ],
+                Game,
+                User.xid.label("users_xid"),
+                count(User.xid)
+                .over(partition_by=Game.id)  # type: ignore .over()
+                .label("player_count"),
             )
             .join(User, isouter=True)
-            .filter(  # type: ignore
+            .filter(  # type: ignore .filter()
                 and_(
                     Game.guild_xid == guild_xid,
                     Game.channel_xid == channel_xid,
                     Game.seats == seats,
                     Game.format == format,
                     Game.status == GameStatus.PENDING.value,
                     Game.deleted_at.is_(None),
                 ),
             )
             .group_by(Game, User.xid)
             .order_by(asc(Game.updated_at))
             .alias("inner")
         )
-        outer = (
-            DatabaseSession.query(Game)
-            # Note: select_entity_from() is deprecated and may need to be replaced
-            #       with an altenative method eventually. See: https://docs.sqlalchemy.org
-            #       /en/latest/orm/query.html#sqlalchemy.orm.Query.select_entity_from
-            .select_entity_from(inner).filter(
-                or_(
-                    column("player_count") == 0,
-                    and_(
-                        column("player_count") > 0,
-                        column("player_count") <= seats - required_seats,
-                    ),
+        outer = aliased(Game, inner)
+        found = DatabaseSession.query(outer).filter(
+            or_(
+                column("player_count") == 0,
+                and_(
+                    column("player_count") > 0,
+                    column("player_count") <= seats - required_seats,
                 ),
-            )
+            ),
         )
+
         joiners = [author_xid, *friends]
         xids_blocked_by_joiners = [
             row.blocked_user_xid
             for row in DatabaseSession.query(Block).filter(Block.user_xid.in_(joiners))
         ]
 
         game: Game
-        for game in outer.all():
+        for game in found.all():
             players = [player.xid for player in game.players]
             if any(xid in players for xid in xids_blocked_by_joiners):
                 continue  # a joiner has blocked one of the players
 
             xids_blocked_by_players = [
                 row.blocked_user_xid
                 for row in DatabaseSession.query(Block).filter(
@@ -270,24 +267,36 @@
         game_id = self.game.id
         guild_xid = self.game.guild_xid
 
         # upsert into plays
         DatabaseSession.execute(
             insert(Play)
             .values(
-                [dict(user_xid=player_xid, game_id=game_id) for player_xid in player_xids],
+                [
+                    {
+                        "user_xid": player_xid,
+                        "game_id": game_id,
+                    }
+                    for player_xid in player_xids
+                ],
             )
             .on_conflict_do_nothing(),
         )
 
         # upsert into user_awards
         DatabaseSession.execute(
             insert(UserAward)
             .values(
-                [dict(guild_xid=guild_xid, user_xid=player_xid) for player_xid in player_xids],
+                [
+                    {
+                        "guild_xid": guild_xid,
+                        "user_xid": player_xid,
+                    }
+                    for player_xid in player_xids
+                ],
             )
             .on_conflict_do_nothing(),
         )
 
         DatabaseSession.commit()
 
     @sync_to_async
@@ -375,15 +384,15 @@
         upsert = insert(Play).values(**values)
         upsert = upsert.on_conflict_do_update(
             constraint="plays_pkey",
             index_where=and_(
                 Play.user_xid == values["user_xid"],
                 Play.game_id == values["game_id"],
             ),
-            set_=dict(points=upsert.excluded.points),
+            set_={"points": upsert.excluded.points},
         )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
 
     @sync_to_async
     @tracer.wrap()
     def to_dict(self) -> dict[str, Any]:
```

### Comparing `spellbot-8.9.1/src/spellbot/services/guilds.py` & `spellbot-8.9.3/src/spellbot/services/guilds.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
             "name": name,
             "updated_at": datetime.utcnow(),
         }
         upsert = insert(Guild).values(**values)
         upsert = upsert.on_conflict_do_update(
             index_elements=[Guild.xid],
             index_where=Guild.xid == values["xid"],
-            set_=dict(
-                name=upsert.excluded.name,
-                updated_at=upsert.excluded.updated_at,
-            ),
+            set_={
+                "name": upsert.excluded.name,
+                "updated_at": upsert.excluded.updated_at,
+            },
         )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
         self.guild = (
             DatabaseSession.query(Guild)
             .filter(
                 Guild.xid == guild.id,
```

### Comparing `spellbot-8.9.1/src/spellbot/services/plays.py` & `spellbot-8.9.3/src/spellbot/services/plays.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/services/users.py` & `spellbot-8.9.3/src/spellbot/services/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         raw_name = getattr(target, "display_name", "")
         name = raw_name[:max_name_len]
         values = {"xid": xid, "name": name, "updated_at": datetime.utcnow()}
         upsert = insert(User).values(**values)
         upsert = upsert.on_conflict_do_update(
             index_elements=[User.xid],
             index_where=User.xid == values["xid"],
-            set_=dict(
-                name=upsert.excluded.name,
-                updated_at=upsert.excluded.updated_at,
-            ),
+            set_={
+                "name": upsert.excluded.name,
+                "updated_at": upsert.excluded.updated_at,
+            },
         )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
         self.user = DatabaseSession.query(User).get(xid)
         assert self.user
         return self.user.to_dict()
 
@@ -53,18 +53,18 @@
             "updated_at": datetime.utcnow(),
             "banned": banned,
         }
         upsert = insert(User).values(**values)
         upsert = upsert.on_conflict_do_update(
             index_elements=[User.xid],
             index_where=User.xid == values["xid"],
-            set_=dict(
-                updated_at=upsert.excluded.updated_at,
-                banned=upsert.excluded.banned,
-            ),
+            set_={
+                "updated_at": upsert.excluded.updated_at,
+                "banned": upsert.excluded.banned,
+            },
         )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
 
     @sync_to_async
     def current_game_id(self) -> Optional[int]:
         assert self.user
@@ -137,15 +137,15 @@
             values["note"] = note[:max_note_len]
             upsert = upsert.on_conflict_do_update(
                 constraint="watches_pkey",
                 index_where=and_(
                     Watch.guild_xid == values["guild_xid"],
                     Watch.user_xid == values["user_xid"],
                 ),
-                set_=dict(note=upsert.excluded.note),
+                set_={"note": upsert.excluded.note},
             )
         else:
             upsert = upsert.on_conflict_do_nothing()
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
 
     @sync_to_async
```

### Comparing `spellbot-8.9.1/src/spellbot/services/verifies.py` & `spellbot-8.9.3/src/spellbot/services/verifies.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         else:
             upsert = upsert.on_conflict_do_update(
                 constraint="verify_pkey",
                 index_where=and_(
                     Verify.guild_xid == values["guild_xid"],
                     Verify.user_xid == values["user_xid"],
                 ),
-                set_=dict(verified=upsert.excluded.verified),
+                set_={"verified": upsert.excluded.verified},
             )
         DatabaseSession.execute(upsert, values)
         DatabaseSession.commit()
         self.current = (
             DatabaseSession.query(Verify)
             .filter(
                 and_(
```

### Comparing `spellbot-8.9.1/src/spellbot/settings.py` & `spellbot-8.9.3/src/spellbot/settings.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/spelltable.py` & `spellbot-8.9.3/src/spellbot/spelltable.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/utils.py` & `spellbot-8.9.3/src/spellbot/utils.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/views/lfg_view.py` & `spellbot-8.9.3/src/spellbot/views/lfg_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/views/setup_view.py` & `spellbot-8.9.3/src/spellbot/views/setup_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/api/record.py` & `spellbot-8.9.3/src/spellbot/web/api/record.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/builder.py` & `spellbot-8.9.3/src/spellbot/web/builder.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/server.py` & `spellbot-8.9.3/src/spellbot/web/server.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/templates/channel_record.html.j2` & `spellbot-8.9.3/src/spellbot/web/templates/channel_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/templates/record.css` & `spellbot-8.9.3/src/spellbot/web/templates/record.css`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/templates/record_base.html.j2` & `spellbot-8.9.3/src/spellbot/web/templates/record_base.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/templates/table2CSV.js` & `spellbot-8.9.3/src/spellbot/web/templates/table2CSV.js`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/src/spellbot/web/templates/user_record.html.j2` & `spellbot-8.9.3/src/spellbot/web/templates/user_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.1/PKG-INFO` & `spellbot-8.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spellbot
-Version: 8.9.1
+Version: 8.9.3
 Summary: The Discord bot for SpellTable
 Home-page: http://spellbot.io/
 License: MIT
 Keywords: discord,magic,bot,mtg,SpellTable
 Author: Amy Troschinetz
 Author-email: spellbot@lexicalunit.com
 Requires-Python: >=3.10,<4
@@ -13,46 +13,45 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Games/Entertainment :: Board Games
-Requires-Dist: Babel (>=2.11.0,<3.0.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: SQLAlchemy (>=1.4.44,<2.0.0)
-Requires-Dist: SQLAlchemy-Utils (>=0.39.0,<0.40.0)
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: aiohttp-jinja2 (>=1.5,<2.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: aiohttp-jinja2 (>=1.5.1,<2.0.0)
 Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0)
-Requires-Dist: alembic (>=1.8.0,<2.0.0)
-Requires-Dist: asgiref (>=3.5.2,<4.0.0)
+Requires-Dist: alembic (>=1.10.3,<2.0.0)
+Requires-Dist: asgiref (>=3.6.0,<4.0.0)
+Requires-Dist: babel (>=2.12.1,<3.0.0)
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
-Requires-Dist: charset-normalizer (==2.1.1)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
-Requires-Dist: datadog (>=0.44.0,<0.45.0)
-Requires-Dist: ddtrace (>=1.6.1,<2.0.0)
-Requires-Dist: discord.py (>=2.1.0,<3.0.0)
-Requires-Dist: dunamai (>=1.14.1,<2.0.0)
+Requires-Dist: datadog (>=0.45.0,<0.46.0)
+Requires-Dist: ddtrace (>=1.12.0,<2.0.0)
+Requires-Dist: discord-py (>=2.2.2,<3.0.0)
+Requires-Dist: dunamai (>=1.16.0,<2.0.0)
 Requires-Dist: expiringdict (>=1.2.2,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: humanize (>=4.3.0,<5.0.0)
-Requires-Dist: hupper (>=1.10.3,<2.0.0)
-Requires-Dist: importlib-resources (>=5.10.2,<6.0.0)
-Requires-Dist: packaging (==22.0)
-Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
+Requires-Dist: humanize (>=4.6.0,<5.0.0)
+Requires-Dist: hupper (>=1.12,<2.0)
+Requires-Dist: importlib-resources (>=5.12.0,<6.0.0)
+Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
-Requires-Dist: pytz (>=2022.6,<2023.0)
-Requires-Dist: requests (==2.28.1)
-Requires-Dist: supervisor (>=4.2.4,<5.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.9,<3.0.0)
+Requires-Dist: sqlalchemy-utils (>=0.41.0,<0.42.0)
+Requires-Dist: supervisor (>=4.2.5,<5.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
-Requires-Dist: wrapt (>=1.14.1,<2.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Project-URL: Repository, https://github.com/lexicalunit/spellbot
 Description-Content-Type: text/markdown
 
 <img
     align="right"
     width="200"
     alt="spellbot"
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: spellbot Version: 8.9.1 Summary: The Discord bot
+Metadata-Version: 2.1 Name: spellbot Version: 8.9.3 Summary: The Discord bot
 for SpellTable Home-page: http://spellbot.io/ License: MIT Keywords:
 discord,magic,bot,mtg,SpellTable Author: Amy Troschinetz Author-email:
 spellbot@lexicalunit.com Requires-Python: >=3.10,<4 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Games/Entertainment :: Board Games Requires-Dist: Babel
-(>=2.11.0,<3.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: SQLAlchemy
-(>=1.4.44,<2.0.0) Requires-Dist: SQLAlchemy-Utils (>=0.39.0,<0.40.0) Requires-
-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: aiohttp-jinja2 (>=1.5,<2.0)
-Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist: alembic
-(>=1.8.0,<2.0.0) Requires-Dist: asgiref (>=3.5.2,<4.0.0) Requires-Dist: certifi
-(>=2022.12.7,<2023.0.0) Requires-Dist: charset-normalizer (==2.1.1) Requires-
-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
-Requires-Dist: datadog (>=0.44.0,<0.45.0) Requires-Dist: ddtrace
-(>=1.6.1,<2.0.0) Requires-Dist: discord.py (>=2.1.0,<3.0.0) Requires-Dist:
-dunamai (>=1.14.1,<2.0.0) Requires-Dist: expiringdict (>=1.2.2,<2.0.0)
-Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: humanize
-(>=4.3.0,<5.0.0) Requires-Dist: hupper (>=1.10.3,<2.0.0) Requires-Dist:
-importlib-resources (>=5.10.2,<6.0.0) Requires-Dist: packaging (==22.0)
-Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0) Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) Requires-Dist: python-dotenv (>=0.21.0,<0.22.0) Requires-Dist:
-pytz (>=2022.6,<2023.0) Requires-Dist: requests (==2.28.1) Requires-Dist:
-supervisor (>=4.2.4,<5.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-
-Dist: uvloop (>=0.17.0,<0.18.0) Requires-Dist: wrapt (>=1.14.1,<2.0.0) Project-
-URL: Repository, https://github.com/lexicalunit/spellbot Description-Content-
-Type: text/markdown [spellbot] # SpellBot [![build][build-badge]][build] [!
-[uptime][uptime-badge]][uptime] [![codecov][codecov-badge]][codecov] [![heroku]
-[heroku-badge]][heroku] [![python][python-badge]][python] [![pypi][pypi-badge]]
-[pypi] [![discord.py][discord-py-badge]][discord-py] [![docker][docker-badge]]
-[docker-hub] [![black][black-badge]][black] [![mit][mit-badge]][mit] [!
-[metrics][metrics-badge]][metrics] [![datadog][datadog-badge]][datadog] [!
-[patreon][patreon-button]][patreon] [![follow][follow-badge]][follow]
+Classifier: Topic :: Games/Entertainment :: Board Games Requires-Dist: aiohttp
+(>=3.8.4,<4.0.0) Requires-Dist: aiohttp-jinja2 (>=1.5.1,<2.0.0) Requires-Dist:
+aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist: alembic (>=1.10.3,<2.0.0)
+Requires-Dist: asgiref (>=3.6.0,<4.0.0) Requires-Dist: babel (>=2.12.1,<3.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0) Requires-Dist: click
+(>=8.1.3,<9.0.0) Requires-Dist: coloredlogs (>=15.0.1,<16.0.0) Requires-Dist:
+datadog (>=0.45.0,<0.46.0) Requires-Dist: ddtrace (>=1.12.0,<2.0.0) Requires-
+Dist: discord-py (>=2.2.2,<3.0.0) Requires-Dist: dunamai (>=1.16.0,<2.0.0)
+Requires-Dist: expiringdict (>=1.2.2,<2.0.0) Requires-Dist: gunicorn
+(>=20.1.0,<21.0.0) Requires-Dist: humanize (>=4.6.0,<5.0.0) Requires-Dist:
+hupper (>=1.12,<2.0) Requires-Dist: importlib-resources (>=5.12.0,<6.0.0)
+Requires-Dist: packaging (>=23.1,<24.0) Requires-Dist: psycopg2-binary
+(>=2.9.6,<3.0.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist:
+python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: pytz (>=2023.3,<2024.0) Requires-
+Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-
+Dist: sqlalchemy (>=2.0.9,<3.0.0) Requires-Dist: sqlalchemy-utils
+(>=0.41.0,<0.42.0) Requires-Dist: supervisor (>=4.2.5,<5.0.0) Requires-Dist:
+toml (>=0.10.2,<0.11.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Requires-Dist:
+wrapt (>=1.15.0,<2.0.0) Project-URL: Repository, https://github.com/
+lexicalunit/spellbot Description-Content-Type: text/markdown [spellbot] #
+SpellBot [![build][build-badge]][build] [![uptime][uptime-badge]][uptime] [!
+[codecov][codecov-badge]][codecov] [![heroku][heroku-badge]][heroku] [![python]
+[python-badge]][python] [![pypi][pypi-badge]][pypi] [![discord.py][discord-py-
+badge]][discord-py] [![docker][docker-badge]][docker-hub] [![black][black-
+badge]][black] [![mit][mit-badge]][mit] [![metrics][metrics-badge]][metrics] [!
+[datadog][datadog-badge]][datadog] [![patreon][patreon-button]][patreon] [!
+[follow][follow-badge]][follow]
 
 
 
                                [Add_to_Discord]
                         The Discord bot for SpellTable
 
 ## ð¤ Using SpellBot SpellBot helps you find _Magic: The Gathering_ games on
```

