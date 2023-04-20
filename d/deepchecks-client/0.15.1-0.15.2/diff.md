# Comparing `tmp/deepchecks_client-0.15.1-py3-none-any.whl.zip` & `tmp/deepchecks_client-0.15.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,208 @@
-Zip file size: 36041 bytes, number of entries: 14
--rw-r--r--  2.0 unx    19765 b- defN 23-Apr-02 14:59 deepchecks_client/__init__.py
--rw-r--r--  2.0 unx     4750 b- defN 23-Apr-02 14:59 deepchecks_client/_shared_docs.py
--rw-r--r--  2.0 unx     1188 b- defN 22-Oct-31 15:39 deepchecks_client/core/AmazonRootCA1.cer
--rw-r--r--  2.0 unx      728 b- defN 22-Dec-06 13:27 deepchecks_client/core/__init__.py
--rw-r--r--  2.0 unx    36165 b- defN 23-Mar-22 18:11 deepchecks_client/core/api.py
--rw-r--r--  2.0 unx    26614 b- defN 23-Apr-02 14:59 deepchecks_client/core/client.py
--rw-r--r--  2.0 unx    13799 b- defN 23-Apr-02 14:59 deepchecks_client/core/utils.py
--rw-r--r--  2.0 unx      766 b- defN 22-Nov-21 08:38 deepchecks_client/tabular/__init__.py
--rw-r--r--  2.0 unx    37251 b- defN 23-Apr-02 14:59 deepchecks_client/tabular/client.py
--rw-r--r--  2.0 unx     6291 b- defN 23-Jan-10 15:59 deepchecks_client/tabular/utils.py
--rw-r--r--  2.0 unx      722 b- defN 23-Apr-05 07:01 deepchecks_client-0.15.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 07:01 deepchecks_client-0.15.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-05 07:01 deepchecks_client-0.15.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1248 b- defN 23-Apr-05 07:01 deepchecks_client-0.15.1.dist-info/RECORD
-14 files, 149397 bytes uncompressed, 33943 bytes compressed:  77.3%
+Zip file size: 340883 bytes, number of entries: 206
+-rw-r--r--  2.0 unx      672 b- defN 22-Jul-25 13:26 deepchecks_monitoring/__init__.py
+-rw-r--r--  2.0 unx     7676 b- defN 23-Apr-20 08:56 deepchecks_monitoring/app.py
+-rw-r--r--  2.0 unx     5802 b- defN 23-Mar-22 18:11 deepchecks_monitoring/cli.py
+-rw-r--r--  2.0 unx     6403 b- defN 23-Apr-20 08:56 deepchecks_monitoring/config.py
+-rw-r--r--  2.0 unx     5045 b- defN 23-Apr-02 14:59 deepchecks_monitoring/dependencies.py
+-rw-r--r--  2.0 unx     5500 b- defN 23-Apr-02 14:59 deepchecks_monitoring/exceptions.py
+-rw-r--r--  2.0 unx     3031 b- defN 23-Mar-20 14:56 deepchecks_monitoring/features_control.py
+-rw-r--r--  2.0 unx    18556 b- defN 23-Mar-28 06:34 deepchecks_monitoring/monitoring_utils.py
+-rw-r--r--  2.0 unx     5695 b- defN 23-Mar-08 17:54 deepchecks_monitoring/notifications.py
+-rw-r--r--  2.0 unx    14791 b- defN 23-Mar-20 14:56 deepchecks_monitoring/resources.py
+-rw-r--r--  2.0 unx      558 b- defN 22-Jul-10 10:04 deepchecks_monitoring/api/__init__.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-Mar-02 07:46 deepchecks_monitoring/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3457 b- defN 23-Jan-29 07:41 deepchecks_monitoring/api/v1/alert.py
+-rw-r--r--  2.0 unx    10964 b- defN 23-Apr-03 08:36 deepchecks_monitoring/api/v1/alert_rule.py
+-rw-r--r--  2.0 unx     4323 b- defN 23-Mar-28 06:34 deepchecks_monitoring/api/v1/alert_webhooks.py
+-rw-r--r--  2.0 unx    29419 b- defN 23-Apr-05 06:58 deepchecks_monitoring/api/v1/check.py
+-rw-r--r--  2.0 unx     5680 b- defN 23-Apr-03 08:36 deepchecks_monitoring/api/v1/configuration.py
+-rw-r--r--  2.0 unx     3364 b- defN 23-Jan-15 15:34 deepchecks_monitoring/api/v1/dashboard.py
+-rw-r--r--  2.0 unx    10326 b- defN 23-Apr-02 14:59 deepchecks_monitoring/api/v1/data_input.py
+-rw-r--r--  2.0 unx     3365 b- defN 23-Mar-22 18:11 deepchecks_monitoring/api/v1/e2e_support_api.py
+-rw-r--r--  2.0 unx    34864 b- defN 23-Apr-03 08:36 deepchecks_monitoring/api/v1/model.py
+-rw-r--r--  2.0 unx    28308 b- defN 23-Apr-02 14:59 deepchecks_monitoring/api/v1/model_version.py
+-rw-r--r--  2.0 unx    12689 b- defN 23-Apr-05 06:58 deepchecks_monitoring/api/v1/monitor.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Mar-02 07:46 deepchecks_monitoring/api/v1/router.py
+-rw-r--r--  2.0 unx      225 b- defN 23-Mar-08 17:54 deepchecks_monitoring/api/v1/global_api/__init__.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Mar-20 14:56 deepchecks_monitoring/api/v1/global_api/auth.py
+-rw-r--r--  2.0 unx      651 b- defN 22-Nov-30 13:28 deepchecks_monitoring/api/v1/global_api/global_router.py
+-rw-r--r--  2.0 unx      317 b- defN 22-Nov-30 13:28 deepchecks_monitoring/api/v1/global_api/helathcheck.py
+-rw-r--r--  2.0 unx     9937 b- defN 23-Mar-20 14:56 deepchecks_monitoring/api/v1/global_api/organization.py
+-rw-r--r--  2.0 unx     7520 b- defN 23-Mar-08 17:54 deepchecks_monitoring/api/v1/global_api/users.py
+-rw-r--r--  2.0 unx      575 b- defN 22-Sep-14 07:01 deepchecks_monitoring/bgtasks/__init__.py
+-rw-r--r--  2.0 unx    10862 b- defN 23-Apr-20 08:56 deepchecks_monitoring/bgtasks/actors.py
+-rw-r--r--  2.0 unx    40797 b- defN 23-Apr-02 14:59 deepchecks_monitoring/bgtasks/core.py
+-rw-r--r--  2.0 unx     1329 b- defN 23-Apr-02 14:59 deepchecks_monitoring/bgtasks/delete_db_table_task.py
+-rw-r--r--  2.0 unx     3837 b- defN 23-Feb-07 13:39 deepchecks_monitoring/bgtasks/model_version_cache_invalidation.py
+-rw-r--r--  2.0 unx     5249 b- defN 23-Mar-22 18:11 deepchecks_monitoring/bgtasks/model_version_offset_update.py
+-rw-r--r--  2.0 unx     5551 b- defN 23-Apr-20 08:56 deepchecks_monitoring/bgtasks/model_version_topic_delete.py
+-rw-r--r--  2.0 unx    15226 b- defN 23-Apr-20 08:56 deepchecks_monitoring/bgtasks/scheduler.py
+-rw-r--r--  2.0 unx     6682 b- defN 23-Mar-08 17:54 deepchecks_monitoring/bgtasks/tasks_queuer.py
+-rw-r--r--  2.0 unx     7252 b- defN 23-Apr-03 07:48 deepchecks_monitoring/bgtasks/tasks_runner.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Mar-08 17:54 deepchecks_monitoring/ee/__init__.py
+-rw-r--r--  2.0 unx     2213 b- defN 23-Mar-28 06:34 deepchecks_monitoring/ee/config.py
+-rw-r--r--  2.0 unx     3676 b- defN 23-Apr-02 14:59 deepchecks_monitoring/ee/features_control.py
+-rw-r--r--  2.0 unx     6763 b- defN 23-Mar-22 18:11 deepchecks_monitoring/ee/middlewares.py
+-rw-r--r--  2.0 unx     4620 b- defN 23-Mar-08 17:54 deepchecks_monitoring/ee/notifications.py
+-rw-r--r--  2.0 unx     5622 b- defN 23-Apr-20 08:56 deepchecks_monitoring/ee/resources.py
+-rw-r--r--  2.0 unx       17 b- defN 23-Mar-02 07:46 deepchecks_monitoring/ee/api/__init__.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Mar-08 17:54 deepchecks_monitoring/ee/api/v1/__init__.py
+-rw-r--r--  2.0 unx    13134 b- defN 23-Mar-28 06:34 deepchecks_monitoring/ee/api/v1/billing.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Mar-02 07:46 deepchecks_monitoring/ee/api/v1/routers.py
+-rw-r--r--  2.0 unx     8293 b- defN 23-Mar-28 06:34 deepchecks_monitoring/ee/api/v1/slack.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Mar-08 17:54 deepchecks_monitoring/ee/integrations/__init__.py
+-rw-r--r--  2.0 unx    10461 b- defN 23-Mar-22 11:52 deepchecks_monitoring/ee/integrations/slack.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Mar-08 17:54 deepchecks_monitoring/ee/utils/__init__.py
+-rw-r--r--  2.0 unx     1176 b- defN 23-Mar-08 17:54 deepchecks_monitoring/ee/utils/sentry.py
+-rw-r--r--  2.0 unx    21788 b- defN 23-Mar-22 18:11 deepchecks_monitoring/ee/utils/telemetry.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Mar-08 17:54 deepchecks_monitoring/integrations/__init__.py
+-rw-r--r--  2.0 unx     6183 b- defN 23-Mar-08 17:54 deepchecks_monitoring/integrations/email.py
+-rw-r--r--  2.0 unx      560 b- defN 22-Jul-10 10:04 deepchecks_monitoring/logic/__init__.py
+-rw-r--r--  2.0 unx     4459 b- defN 23-Jan-29 07:42 deepchecks_monitoring/logic/cache_functions.py
+-rw-r--r--  2.0 unx    36207 b- defN 23-Apr-17 12:10 deepchecks_monitoring/logic/check_logic.py
+-rw-r--r--  2.0 unx    23552 b- defN 23-Mar-28 06:34 deepchecks_monitoring/logic/data_ingestion.py
+-rw-r--r--  2.0 unx     2173 b- defN 23-Mar-22 18:11 deepchecks_monitoring/logic/kafka_consumer.py
+-rw-r--r--  2.0 unx     3122 b- defN 23-Mar-22 18:11 deepchecks_monitoring/logic/keys.py
+-rw-r--r--  2.0 unx    15313 b- defN 23-Apr-05 06:58 deepchecks_monitoring/logic/model_logic.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-Apr-03 08:36 deepchecks_monitoring/logic/monitor_alert_logic.py
+-rw-r--r--  2.0 unx     6366 b- defN 23-Apr-17 12:10 deepchecks_monitoring/logic/statistics.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-Mar-22 18:11 deepchecks_monitoring/logic/suite_logic.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Feb-28 14:40 deepchecks_monitoring/public_models/__init__.py
+-rw-r--r--  2.0 unx      309 b- defN 23-Feb-07 07:13 deepchecks_monitoring/public_models/base.py
+-rw-r--r--  2.0 unx     1582 b- defN 23-Mar-08 17:54 deepchecks_monitoring/public_models/billing.py
+-rw-r--r--  2.0 unx     1548 b- defN 23-Mar-20 14:56 deepchecks_monitoring/public_models/invitation.py
+-rw-r--r--  2.0 unx     4294 b- defN 23-Mar-08 17:54 deepchecks_monitoring/public_models/organization.py
+-rw-r--r--  2.0 unx     2051 b- defN 23-Jan-24 07:35 deepchecks_monitoring/public_models/task.py
+-rw-r--r--  2.0 unx     4021 b- defN 23-Mar-08 17:54 deepchecks_monitoring/public_models/user.py
+-rw-r--r--  2.0 unx      567 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/__init__.py
+-rw-r--r--  2.0 unx     4970 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_migrations/env.py
+-rw-r--r--  2.0 unx     2310 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/06711abb0d6e_added_event_table.py
+-rw-r--r--  2.0 unx     3194 b- defN 23-Feb-21 14:18 deepchecks_monitoring/schema_migrations/versions/0d2eb31dab85_monitors_schemas_update.py
+-rw-r--r--  2.0 unx     1478 b- defN 22-Dec-19 13:35 deepchecks_monitoring/schema_migrations/versions/0e37ca889b28_added_indexes_for_ingestionerror_.py
+-rw-r--r--  2.0 unx     2006 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/10bbb2fd4aac_refactor_model_version_schema_columns.py
+-rw-r--r--  2.0 unx     1493 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/14daeddd99d6_remove_monitors_table_deletion_triggers.py
+-rw-r--r--  2.0 unx     1499 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/1c09de380fe6_rename_last_process_column.py
+-rw-r--r--  2.0 unx     1350 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/21e565825df9_rename_non_features_to_additional_data_.py
+-rw-r--r--  2.0 unx     1712 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/224e3cab5cfc_alertrule_added_constrains.py
+-rw-r--r--  2.0 unx     1194 b- defN 22-Dec-02 14:52 deepchecks_monitoring/schema_migrations/versions/254559c8d23d_old_tasks_removal_trigger.py
+-rw-r--r--  2.0 unx     6628 b- defN 23-Mar-28 06:34 deepchecks_monitoring/schema_migrations/versions/294d2b30b20b_added_metadatamixin.py
+-rw-r--r--  2.0 unx    10729 b- defN 23-Apr-02 14:59 deepchecks_monitoring/schema_migrations/versions/29e9ef85d8fd_frequency_enumeration.py
+-rw-r--r--  2.0 unx     3410 b- defN 22-Dec-19 13:35 deepchecks_monitoring/schema_migrations/versions/2aff25ef5915_add_logged_time.py
+-rw-r--r--  2.0 unx     1590 b- defN 23-Feb-19 07:29 deepchecks_monitoring/schema_migrations/versions/320b2ed2c803_add_balance_classes.py
+-rw-r--r--  2.0 unx     1846 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/3ad1774b9ba0_added_indexes.py
+-rw-r--r--  2.0 unx     1961 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/47b0e3008c9d_added_multi_oprator.py
+-rw-r--r--  2.0 unx     2279 b- defN 22-Dec-26 09:02 deepchecks_monitoring/schema_migrations/versions/48ecb1727677_add_start_end_times_to_model.py
+-rw-r--r--  2.0 unx     1276 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/4b323d8c6edd_added_label_map.py
+-rw-r--r--  2.0 unx     3883 b- defN 22-Dec-06 07:28 deepchecks_monitoring/schema_migrations/versions/4ba6a640c364_added_webhooks_table.py
+-rw-r--r--  2.0 unx     1669 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/4cd3c6e0688d_add_ingestion_error.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_migrations/versions/53ef59cd095c_add_alert_rule_start_time.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Jan-29 07:42 deepchecks_monitoring/schema_migrations/versions/5595c044948b_update_alerts_end_time.py
+-rw-r--r--  2.0 unx     2410 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/59e285f86ad1_added_alert_value.py
+-rw-r--r--  2.0 unx     1988 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/5a3eb258120c_changed_alert_rule_constraint.py
+-rw-r--r--  2.0 unx     1268 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/6b5bc12a5659_changed_monitor_frequency_constraint.py
+-rw-r--r--  2.0 unx     1447 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/7a58ef90ea7c_add_trigger_on_model_version_delete.py
+-rw-r--r--  2.0 unx     3430 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_migrations/versions/7c9e3307dffc_tasks_table.py
+-rw-r--r--  2.0 unx     1723 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/7efcef46aef9_add_model_version_times.py
+-rw-r--r--  2.0 unx     1289 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/7fc188dbba95_alert_rule_scheduling_start.py
+-rw-r--r--  2.0 unx     2551 b- defN 22-Dec-02 14:52 deepchecks_monitoring/schema_migrations/versions/8a9bc6d69ca3_moved_slack_tables.py
+-rw-r--r--  2.0 unx     1245 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/95d7fe3b963b_add_resolved_field_to_alert.py
+-rw-r--r--  2.0 unx     1814 b- defN 23-Mar-20 14:56 deepchecks_monitoring/schema_migrations/versions/9981564b113b_l2_to_l3.py
+-rw-r--r--  2.0 unx     1597 b- defN 23-Feb-05 08:35 deepchecks_monitoring/schema_migrations/versions/9f485bd47729_added_modelnote_entity.py
+-rw-r--r--  2.0 unx      528 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/__init__.py
+-rw-r--r--  2.0 unx     2866 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_migrations/versions/a04f0f00b5f0_updated_filter_way_and_added_model_task_.py
+-rw-r--r--  2.0 unx     2397 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_migrations/versions/a1d70019e14d_alert_name_to_id.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jan-15 09:02 deepchecks_monitoring/schema_migrations/versions/a6ac6c689b56_update_monitor_filters.py
+-rw-r--r--  2.0 unx     1510 b- defN 22-Dec-26 09:02 deepchecks_monitoring/schema_migrations/versions/a8341cc95913_remove_vision_task_type.py
+-rw-r--r--  2.0 unx     5302 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_migrations/versions/ad67b0cf252f_rename_alerts_and_events.py
+-rw-r--r--  2.0 unx     1873 b- defN 23-Feb-05 08:35 deepchecks_monitoring/schema_migrations/versions/ae5aec6f986a_update_model_version_last_update_time.py
+-rw-r--r--  2.0 unx     4251 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/b75212c5da00_added_modified_cascade.py
+-rw-r--r--  2.0 unx     2390 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/b85e265f38ee_moved_alert_rule_to_monitor.py
+-rw-r--r--  2.0 unx     1278 b- defN 23-Apr-02 14:59 deepchecks_monitoring/schema_migrations/versions/ba2e7acc66c2_added_model_timezone.py
+-rw-r--r--  2.0 unx     1017 b- defN 23-Mar-22 11:52 deepchecks_monitoring/schema_migrations/versions/bfca690f5a74_renamed_alerts_name_mid_to_medium.py
+-rw-r--r--  2.0 unx     1730 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/c06a732efcc4_added_monitor_table.py
+-rw-r--r--  2.0 unx     4241 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/c5d2ffb432e7_move_scheduling_logic_to_monitor.py
+-rw-r--r--  2.0 unx     5893 b- defN 23-Mar-22 18:11 deepchecks_monitoring/schema_migrations/versions/cc61786f5880_labels_refactor.py
+-rw-r--r--  2.0 unx     1022 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/d18e5a487cfe_add_classes_to_model_version.py
+-rw-r--r--  2.0 unx     1195 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/d2fd35a0db92_monitoring_table_schema_fix.py
+-rw-r--r--  2.0 unx     1317 b- defN 23-Jan-03 15:13 deepchecks_monitoring/schema_migrations/versions/d568613130f0_remove_schedule_start_column.py
+-rw-r--r--  2.0 unx     3213 b- defN 23-Feb-23 08:00 deepchecks_monitoring/schema_migrations/versions/dcab2cc8515b_added_modelversion_private_reference_.py
+-rw-r--r--  2.0 unx     1563 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/e0ec67ddf099_updated_task_type.py
+-rw-r--r--  2.0 unx     1862 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/e45cd02bc493_added_dashboard.py
+-rw-r--r--  2.0 unx     1849 b- defN 23-Apr-17 12:10 deepchecks_monitoring/schema_migrations/versions/e8a5d4213c45_tables_fix.py
+-rw-r--r--  2.0 unx     1369 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/f2ec131ea7a5_add_is_active_to_alert_rule.py
+-rw-r--r--  2.0 unx     2686 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/f3774099d232_cache_invalidation_and_ingestion_errors.py
+-rw-r--r--  2.0 unx     3565 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_migrations/versions/fb9160d139d5_create_initial_models.py
+-rw-r--r--  2.0 unx     1350 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_models/__init__.py
+-rw-r--r--  2.0 unx     1712 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_models/alert.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-Apr-03 08:36 deepchecks_monitoring/schema_models/alert_rule.py
+-rw-r--r--  2.0 unx    14334 b- defN 23-Apr-20 08:56 deepchecks_monitoring/schema_models/alert_webhook.py
+-rw-r--r--  2.0 unx     2068 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_models/base.py
+-rw-r--r--  2.0 unx     2621 b- defN 23-Mar-28 06:34 deepchecks_monitoring/schema_models/check.py
+-rw-r--r--  2.0 unx     6170 b- defN 23-Mar-22 18:11 deepchecks_monitoring/schema_models/column_type.py
+-rw-r--r--  2.0 unx     1202 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_models/dashboard.py
+-rw-r--r--  2.0 unx     1611 b- defN 23-Feb-07 07:13 deepchecks_monitoring/schema_models/ingestion_errors.py
+-rw-r--r--  2.0 unx     6777 b- defN 23-Apr-02 14:59 deepchecks_monitoring/schema_models/model.py
+-rw-r--r--  2.0 unx    12649 b- defN 23-Mar-28 06:34 deepchecks_monitoring/schema_models/model_version.py
+-rw-r--r--  2.0 unx     7461 b- defN 23-Apr-02 14:59 deepchecks_monitoring/schema_models/monitor.py
+-rw-r--r--  2.0 unx     1453 b- defN 22-Nov-30 13:28 deepchecks_monitoring/schema_models/pydantic_type.py
+-rw-r--r--  2.0 unx     3226 b- defN 23-Mar-28 06:34 deepchecks_monitoring/schema_models/slack.py
+-rw-r--r--  2.0 unx      687 b- defN 23-Mar-22 18:11 deepchecks_monitoring/schema_models/task_type.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Mar-08 17:54 deepchecks_monitoring/templates/__init__.py
+-rw-r--r--  2.0 unx       47 b- defN 22-Nov-30 13:28 deepchecks_monitoring/utils/__init__.py
+-rw-r--r--  2.0 unx      610 b- defN 23-Feb-07 07:13 deepchecks_monitoring/utils/alerts.py
+-rw-r--r--  2.0 unx    11024 b- defN 23-Apr-02 14:59 deepchecks_monitoring/utils/auth.py
+-rw-r--r--  2.0 unx     8781 b- defN 23-Jan-31 08:44 deepchecks_monitoring/utils/database.py
+-rw-r--r--  2.0 unx     4430 b- defN 23-Mar-08 17:54 deepchecks_monitoring/utils/notebook_util.py
+-rw-r--r--  2.0 unx     4176 b- defN 23-Apr-20 08:56 deepchecks_monitoring/utils/other.py
+-rw-r--r--  2.0 unx      707 b- defN 22-Dec-04 10:07 deepchecks_monitoring/utils/text.py
+-rw-r--r--  2.0 unx      420 b- defN 23-Apr-02 14:59 deepchecks_monitoring/utils/typing.py
+-rw-r--r--  2.0 unx      516 b- defN 22-Jul-10 10:04 tests/__init__.py
+-rw-r--r--  2.0 unx    56222 b- defN 23-Apr-03 08:36 tests/common.py
+-rw-r--r--  2.0 unx    13172 b- defN 23-Mar-22 18:11 tests/conftest.py
+-rw-r--r--  2.0 unx     8238 b- defN 22-Nov-30 13:28 tests/utils.py
+-rw-r--r--  2.0 unx      516 b- defN 22-Jul-10 10:04 tests/api/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Apr-02 14:59 tests/api/test_access_restrictions.py
+-rw-r--r--  2.0 unx    10032 b- defN 23-Mar-22 11:52 tests/api/test_alert_rules.py
+-rw-r--r--  2.0 unx     2429 b- defN 23-Apr-02 14:59 tests/api/test_alert_webhooks.py
+-rw-r--r--  2.0 unx     3408 b- defN 23-Mar-22 11:52 tests/api/test_alerts.py
+-rw-r--r--  2.0 unx    42969 b- defN 23-Apr-02 14:59 tests/api/test_check.py
+-rw-r--r--  2.0 unx     2333 b- defN 22-Dec-26 09:02 tests/api/test_dashboards.py
+-rw-r--r--  2.0 unx    14212 b- defN 23-Apr-02 14:59 tests/api/test_data_input.py
+-rw-r--r--  2.0 unx    12094 b- defN 23-Apr-02 14:59 tests/api/test_model_version.py
+-rw-r--r--  2.0 unx    12569 b- defN 23-Apr-03 08:36 tests/api/test_models.py
+-rw-r--r--  2.0 unx    20021 b- defN 23-Apr-02 14:59 tests/api/test_monitor.py
+-rw-r--r--  2.0 unx     8697 b- defN 23-Apr-02 14:59 tests/api/test_organization_api.py
+-rw-r--r--  2.0 unx     5700 b- defN 23-Mar-02 07:46 tests/api/test_slack_integration.py
+-rw-r--r--  2.0 unx     1991 b- defN 23-Mar-22 18:11 tests/api/test_suite_execution.py
+-rw-r--r--  2.0 unx     2665 b- defN 22-Dec-11 06:56 tests/api/test_users_api.py
+-rw-r--r--  2.0 unx      515 b- defN 22-Sep-14 07:01 tests/logic/__init__.py
+-rw-r--r--  2.0 unx     3692 b- defN 23-Jan-24 17:06 tests/logic/test_cache_functions.py
+-rw-r--r--  2.0 unx     1924 b- defN 22-Dec-26 09:02 tests/logic/test_statistics.py
+-rw-r--r--  2.0 unx      516 b- defN 22-Sep-15 12:38 tests/sdk/__init__.py
+-rw-r--r--  2.0 unx      515 b- defN 22-Oct-13 06:03 tests/sdk/core/__init__.py
+-rw-r--r--  2.0 unx     1243 b- defN 23-Jan-24 07:35 tests/sdk/core/test_api.py
+-rw-r--r--  2.0 unx     5712 b- defN 23-Mar-22 18:11 tests/sdk/core/test_data_retrieval.py
+-rw-r--r--  2.0 unx     2732 b- defN 23-Apr-20 08:56 tests/sdk/core/test_model.py
+-rw-r--r--  2.0 unx     2269 b- defN 23-Mar-22 18:11 tests/sdk/core/test_model_version.py
+-rw-r--r--  2.0 unx      516 b- defN 22-Sep-15 12:38 tests/sdk/tabular/__init__.py
+-rw-r--r--  2.0 unx    16550 b- defN 23-Mar-22 18:11 tests/sdk/tabular/test_log_data.py
+-rw-r--r--  2.0 unx     4375 b- defN 23-Mar-08 17:54 tests/sdk/tabular/test_model.py
+-rw-r--r--  2.0 unx    10990 b- defN 23-Apr-02 14:59 tests/sdk/tabular/test_model_version.py
+-rw-r--r--  2.0 unx     8649 b- defN 23-Mar-22 18:11 tests/sdk/tabular/test_quick_create.py
+-rw-r--r--  2.0 unx    11599 b- defN 23-Apr-02 14:59 tests/sdk/tabular/test_upload_reference.py
+-rw-r--r--  2.0 unx      515 b- defN 22-Sep-14 07:01 tests/unittests/__init__.py
+-rw-r--r--  2.0 unx     1110 b- defN 23-Mar-08 17:54 tests/unittests/conftest.py
+-rw-r--r--  2.0 unx     9621 b- defN 23-Apr-17 12:10 tests/unittests/test_alert_notificator.py
+-rw-r--r--  2.0 unx     6929 b- defN 23-Apr-02 14:59 tests/unittests/test_alert_webhooks.py
+-rw-r--r--  2.0 unx    18216 b- defN 23-Apr-02 14:59 tests/unittests/test_alerts_scheduler.py
+-rw-r--r--  2.0 unx     2802 b- defN 22-Nov-30 13:28 tests/unittests/test_database_utils.py
+-rw-r--r--  2.0 unx      605 b- defN 23-Mar-08 17:54 tests/unittests/test_email_sender.py
+-rw-r--r--  2.0 unx    13012 b- defN 23-Apr-02 14:59 tests/unittests/test_monitor_alert_rules_executor.py
+-rw-r--r--  2.0 unx     4593 b- defN 22-Nov-30 13:28 tests/unittests/test_tasks_broker.py
+-rw-r--r--  2.0 unx     1874 b- defN 22-Nov-30 13:28 tests/unittests/test_user_creation.py
+-rw-r--r--  2.0 unx    20471 b- defN 23-Feb-02 14:28 tests/unittests/test_worker.py
+-rw-r--r--  2.0 unx      722 b- defN 23-Apr-20 08:56 deepchecks_client-0.15.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 08:56 deepchecks_client-0.15.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-20 08:56 deepchecks_client-0.15.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    22561 b- defN 23-Apr-20 08:56 deepchecks_client-0.15.2.dist-info/RECORD
+206 files, 1167009 bytes uncompressed, 303441 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,43 +1,619 @@
-Filename: deepchecks_client/__init__.py
+Filename: deepchecks_monitoring/__init__.py
 Comment: 
 
-Filename: deepchecks_client/_shared_docs.py
+Filename: deepchecks_monitoring/app.py
 Comment: 
 
-Filename: deepchecks_client/core/AmazonRootCA1.cer
+Filename: deepchecks_monitoring/cli.py
 Comment: 
 
-Filename: deepchecks_client/core/__init__.py
+Filename: deepchecks_monitoring/config.py
 Comment: 
 
-Filename: deepchecks_client/core/api.py
+Filename: deepchecks_monitoring/dependencies.py
 Comment: 
 
-Filename: deepchecks_client/core/client.py
+Filename: deepchecks_monitoring/exceptions.py
 Comment: 
 
-Filename: deepchecks_client/core/utils.py
+Filename: deepchecks_monitoring/features_control.py
 Comment: 
 
-Filename: deepchecks_client/tabular/__init__.py
+Filename: deepchecks_monitoring/monitoring_utils.py
 Comment: 
 
-Filename: deepchecks_client/tabular/client.py
+Filename: deepchecks_monitoring/notifications.py
 Comment: 
 
-Filename: deepchecks_client/tabular/utils.py
+Filename: deepchecks_monitoring/resources.py
 Comment: 
 
-Filename: deepchecks_client-0.15.1.dist-info/METADATA
+Filename: deepchecks_monitoring/api/__init__.py
 Comment: 
 
-Filename: deepchecks_client-0.15.1.dist-info/WHEEL
+Filename: deepchecks_monitoring/api/v1/__init__.py
 Comment: 
 
-Filename: deepchecks_client-0.15.1.dist-info/top_level.txt
+Filename: deepchecks_monitoring/api/v1/alert.py
 Comment: 
 
-Filename: deepchecks_client-0.15.1.dist-info/RECORD
+Filename: deepchecks_monitoring/api/v1/alert_rule.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/alert_webhooks.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/check.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/configuration.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/dashboard.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/data_input.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/e2e_support_api.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/model.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/model_version.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/monitor.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/router.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/global_api/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/global_api/auth.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/global_api/global_router.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/global_api/helathcheck.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/global_api/organization.py
+Comment: 
+
+Filename: deepchecks_monitoring/api/v1/global_api/users.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/actors.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/core.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/delete_db_table_task.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/model_version_cache_invalidation.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/model_version_offset_update.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/model_version_topic_delete.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/scheduler.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/tasks_queuer.py
+Comment: 
+
+Filename: deepchecks_monitoring/bgtasks/tasks_runner.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/config.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/features_control.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/middlewares.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/notifications.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/resources.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/api/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/api/v1/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/api/v1/billing.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/api/v1/routers.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/api/v1/slack.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/integrations/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/integrations/slack.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/utils/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/utils/sentry.py
+Comment: 
+
+Filename: deepchecks_monitoring/ee/utils/telemetry.py
+Comment: 
+
+Filename: deepchecks_monitoring/integrations/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/integrations/email.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/cache_functions.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/check_logic.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/data_ingestion.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/kafka_consumer.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/keys.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/model_logic.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/monitor_alert_logic.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/statistics.py
+Comment: 
+
+Filename: deepchecks_monitoring/logic/suite_logic.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/base.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/billing.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/invitation.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/organization.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/task.py
+Comment: 
+
+Filename: deepchecks_monitoring/public_models/user.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/env.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/06711abb0d6e_added_event_table.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/0d2eb31dab85_monitors_schemas_update.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/0e37ca889b28_added_indexes_for_ingestionerror_.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/10bbb2fd4aac_refactor_model_version_schema_columns.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/14daeddd99d6_remove_monitors_table_deletion_triggers.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/1c09de380fe6_rename_last_process_column.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/21e565825df9_rename_non_features_to_additional_data_.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/224e3cab5cfc_alertrule_added_constrains.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/254559c8d23d_old_tasks_removal_trigger.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/294d2b30b20b_added_metadatamixin.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/29e9ef85d8fd_frequency_enumeration.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/2aff25ef5915_add_logged_time.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/320b2ed2c803_add_balance_classes.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/3ad1774b9ba0_added_indexes.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/47b0e3008c9d_added_multi_oprator.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/48ecb1727677_add_start_end_times_to_model.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/4b323d8c6edd_added_label_map.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/4ba6a640c364_added_webhooks_table.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/4cd3c6e0688d_add_ingestion_error.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/53ef59cd095c_add_alert_rule_start_time.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/5595c044948b_update_alerts_end_time.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/59e285f86ad1_added_alert_value.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/5a3eb258120c_changed_alert_rule_constraint.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/6b5bc12a5659_changed_monitor_frequency_constraint.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/7a58ef90ea7c_add_trigger_on_model_version_delete.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/7c9e3307dffc_tasks_table.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/7efcef46aef9_add_model_version_times.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/7fc188dbba95_alert_rule_scheduling_start.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/8a9bc6d69ca3_moved_slack_tables.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/95d7fe3b963b_add_resolved_field_to_alert.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/9981564b113b_l2_to_l3.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/9f485bd47729_added_modelnote_entity.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/a04f0f00b5f0_updated_filter_way_and_added_model_task_.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/a1d70019e14d_alert_name_to_id.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/a6ac6c689b56_update_monitor_filters.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/a8341cc95913_remove_vision_task_type.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/ad67b0cf252f_rename_alerts_and_events.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/ae5aec6f986a_update_model_version_last_update_time.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/b75212c5da00_added_modified_cascade.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/b85e265f38ee_moved_alert_rule_to_monitor.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/ba2e7acc66c2_added_model_timezone.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/bfca690f5a74_renamed_alerts_name_mid_to_medium.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/c06a732efcc4_added_monitor_table.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/c5d2ffb432e7_move_scheduling_logic_to_monitor.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/cc61786f5880_labels_refactor.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/d18e5a487cfe_add_classes_to_model_version.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/d2fd35a0db92_monitoring_table_schema_fix.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/d568613130f0_remove_schedule_start_column.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/dcab2cc8515b_added_modelversion_private_reference_.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/e0ec67ddf099_updated_task_type.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/e45cd02bc493_added_dashboard.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/e8a5d4213c45_tables_fix.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/f2ec131ea7a5_add_is_active_to_alert_rule.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/f3774099d232_cache_invalidation_and_ingestion_errors.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_migrations/versions/fb9160d139d5_create_initial_models.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/alert.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/alert_rule.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/alert_webhook.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/base.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/check.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/column_type.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/dashboard.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/ingestion_errors.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/model.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/model_version.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/monitor.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/pydantic_type.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/slack.py
+Comment: 
+
+Filename: deepchecks_monitoring/schema_models/task_type.py
+Comment: 
+
+Filename: deepchecks_monitoring/templates/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/__init__.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/alerts.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/auth.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/database.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/notebook_util.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/other.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/text.py
+Comment: 
+
+Filename: deepchecks_monitoring/utils/typing.py
+Comment: 
+
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/common.py
+Comment: 
+
+Filename: tests/conftest.py
+Comment: 
+
+Filename: tests/utils.py
+Comment: 
+
+Filename: tests/api/__init__.py
+Comment: 
+
+Filename: tests/api/test_access_restrictions.py
+Comment: 
+
+Filename: tests/api/test_alert_rules.py
+Comment: 
+
+Filename: tests/api/test_alert_webhooks.py
+Comment: 
+
+Filename: tests/api/test_alerts.py
+Comment: 
+
+Filename: tests/api/test_check.py
+Comment: 
+
+Filename: tests/api/test_dashboards.py
+Comment: 
+
+Filename: tests/api/test_data_input.py
+Comment: 
+
+Filename: tests/api/test_model_version.py
+Comment: 
+
+Filename: tests/api/test_models.py
+Comment: 
+
+Filename: tests/api/test_monitor.py
+Comment: 
+
+Filename: tests/api/test_organization_api.py
+Comment: 
+
+Filename: tests/api/test_slack_integration.py
+Comment: 
+
+Filename: tests/api/test_suite_execution.py
+Comment: 
+
+Filename: tests/api/test_users_api.py
+Comment: 
+
+Filename: tests/logic/__init__.py
+Comment: 
+
+Filename: tests/logic/test_cache_functions.py
+Comment: 
+
+Filename: tests/logic/test_statistics.py
+Comment: 
+
+Filename: tests/sdk/__init__.py
+Comment: 
+
+Filename: tests/sdk/core/__init__.py
+Comment: 
+
+Filename: tests/sdk/core/test_api.py
+Comment: 
+
+Filename: tests/sdk/core/test_data_retrieval.py
+Comment: 
+
+Filename: tests/sdk/core/test_model.py
+Comment: 
+
+Filename: tests/sdk/core/test_model_version.py
+Comment: 
+
+Filename: tests/sdk/tabular/__init__.py
+Comment: 
+
+Filename: tests/sdk/tabular/test_log_data.py
+Comment: 
+
+Filename: tests/sdk/tabular/test_model.py
+Comment: 
+
+Filename: tests/sdk/tabular/test_model_version.py
+Comment: 
+
+Filename: tests/sdk/tabular/test_quick_create.py
+Comment: 
+
+Filename: tests/sdk/tabular/test_upload_reference.py
+Comment: 
+
+Filename: tests/unittests/__init__.py
+Comment: 
+
+Filename: tests/unittests/conftest.py
+Comment: 
+
+Filename: tests/unittests/test_alert_notificator.py
+Comment: 
+
+Filename: tests/unittests/test_alert_webhooks.py
+Comment: 
+
+Filename: tests/unittests/test_alerts_scheduler.py
+Comment: 
+
+Filename: tests/unittests/test_database_utils.py
+Comment: 
+
+Filename: tests/unittests/test_email_sender.py
+Comment: 
+
+Filename: tests/unittests/test_monitor_alert_rules_executor.py
+Comment: 
+
+Filename: tests/unittests/test_tasks_broker.py
+Comment: 
+
+Filename: tests/unittests/test_user_creation.py
+Comment: 
+
+Filename: tests/unittests/test_worker.py
+Comment: 
+
+Filename: deepchecks_client-0.15.2.dist-info/METADATA
+Comment: 
+
+Filename: deepchecks_client-0.15.2.dist-info/WHEEL
+Comment: 
+
+Filename: deepchecks_client-0.15.2.dist-info/top_level.txt
+Comment: 
+
+Filename: deepchecks_client-0.15.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `deepchecks_client/core/__init__.py` & `deepchecks_monitoring/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,12 +3,9 @@
 #
 # This file is part of Deepchecks.
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
-#
-"""Module defining the core client functionality."""
-from deepchecks_client.core.utils import ColumnType, DataFilter, OperatorsEnum, TaskType
 
-__all__ = ['ColumnType', 'TaskType', 'DataFilter', 'OperatorsEnum']
+"""Module defining the API of the app."""
```

## Comparing `deepchecks_client/tabular/__init__.py` & `deepchecks_monitoring/api/v1/router.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,26 @@
 #
 # This file is part of Deepchecks.
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
-#
-"""Module defining the tabular client functionality."""
-from deepchecks.tabular.utils.task_type import TaskType as DeepchecksTaskType
-from deepchecks_client.tabular.utils import create_schema, read_schema
+"""Module defining the Router for V1 API."""
+from fastapi import APIRouter
+
+from deepchecks_monitoring import __version__
+
+__all__ = ['router']
+
+
+router = APIRouter(prefix='/api/v1')
+
+
+@router.get('/say-hello')
+async def hello_world() -> str:
+    return 'Hello world'
+
 
-__all__ = ['create_schema', 'read_schema']
+@router.get('/backend-version')
+async def retrieve_backend_version():
+    return {'version': __version__}
```

