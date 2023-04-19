# Comparing `tmp/corellium-api-0.2.0.tar.gz` & `tmp/corellium-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corellium-api-0.2.0.tar", last modified: Fri Feb 24 02:27:47 2023, max compression
+gzip compressed data, was "corellium-api-0.3.0.tar", last modified: Wed Apr 19 23:37:42 2023, max compression
```

## Comparing `corellium-api-0.2.0.tar` & `corellium-api-0.3.0.tar`

### file list

```diff
@@ -1,222 +1,228 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-02-24 02:27:47.954489 corellium-api-0.2.0/
--rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-02-24 02:27:47.954489 corellium-api-0.2.0/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)    27569 2023-02-24 01:35:14.000000 corellium-api-0.2.0/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-02-24 02:27:47.890491 corellium-api-0.2.0/corellium_api/
--rw-r--r--   0 sam       (1000) sam       (1000)     7074 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/__init__.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-02-24 02:27:47.894491 corellium-api-0.2.0/corellium_api/api/
--rw-r--r--   0 sam       (1000) sam       (1000)      144 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/api/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)   828519 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/api/corellium_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)    27763 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/api_client.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16373 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/configuration.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5079 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/exceptions.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-02-24 02:27:47.926490 corellium-api-0.2.0/corellium_api/models/
--rw-r--r--   0 sam       (1000) sam       (1000)     6533 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7297 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/address.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7554 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_app.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3858 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_app_ready_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4355 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_app_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4440 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_apps_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4530 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_apps_status_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5938 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3598 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_icons.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3650 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_install_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3923 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_profiles_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3685 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_system_adb_auth.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3950 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_system_get_prop_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3664 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agent_value_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3805 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/agreed_ack.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5803 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/api_conflict_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5470 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/api_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5774 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/api_internal_consistency_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6109 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/api_not_found_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3838 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/api_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3057 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/bit.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3706 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/btrace_enable_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3371 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/button.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5900 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/coupon_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3763 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/create_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5546 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/created_by.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4799 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/credentials.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4663 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/domain_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8137 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16319 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/features.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5473 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/file_changes.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13230 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/firmware.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4980 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/gpio_state_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4900 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/gpios_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3714 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/grant_trial_request_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9583 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/hook.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9942 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/image.py
--rw-r--r--   0 sam       (1000) sam       (1000)    22126 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4241 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_agent_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8957 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_boot_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3481 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_boot_options_additional_tag.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3684 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_console_endpoint.py
--rw-r--r--   0 sam       (1000) sam       (1000)    14753 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_create_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5709 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4939 2023-02-24 01:35:13.000000 corellium-api-0.2.0/corellium_api/models/instance_netmon_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4551 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/instance_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3602 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/instance_services.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3719 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/instance_start_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3342 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/instance_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3681 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/instance_stop_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4524 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/instance_upgrade_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5005 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/invitation.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3610 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/invite_revoke_params.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3015 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/invite_revoke_params_ids.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4189 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/kcrange.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5589 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/kernel_task.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4975 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/kernel_thread.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4294 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/media_play_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9969 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/model.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6961 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/model_software.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5833 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/password_change_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5846 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/password_reset_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6233 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/patch_instance_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9480 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/peripherals_data.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5136 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/plan.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5173 2023-02-24 02:21:07.000000 corellium-api-0.2.0/corellium_api/models/plan_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6360 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/project.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8535 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/project_key.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4882 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/project_quota.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5104 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/project_settings.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5463 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/project_usage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5035 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/rate_info.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3887 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/reset_link_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5641 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/role.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4299 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/rotate_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8026 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/snapshot.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3875 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/snapshot_creation_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4256 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/snapshot_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13443 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/subscriber_invite.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5073 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3566 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/team_create.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3574 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/text_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4461 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/touch_curve_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3716 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/touch_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3831 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/trial.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5947 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/trial_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7580 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/trial_request_metadata.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7300 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/trial_request_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3799 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/update_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6885 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/user.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5657 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/user_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6963 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/v1_create_hook_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4010 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/v1_load_extension_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3783 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/v1_set_state_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5759 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/validation_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5176 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/volume_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4355 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/vpn_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7965 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/web_player_create_session_request.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5869 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/models/web_player_session.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9862 2023-02-24 01:35:14.000000 corellium-api-0.2.0/corellium_api/rest.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-02-24 02:27:47.894491 corellium-api-0.2.0/corellium_api.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-02-24 02:27:47.000000 corellium-api-0.2.0/corellium_api.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     7293 2023-02-24 02:27:47.000000 corellium-api-0.2.0/corellium_api.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-02-24 02:27:47.000000 corellium-api-0.2.0/corellium_api.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       57 2023-02-24 02:27:47.000000 corellium-api-0.2.0/corellium_api.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       14 2023-02-24 02:27:47.000000 corellium-api-0.2.0/corellium_api.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       69 2023-02-24 02:27:47.954489 corellium-api-0.2.0/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)     1056 2023-02-24 01:35:14.000000 corellium-api-0.2.0/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-02-24 02:27:47.954489 corellium-api-0.2.0/test/
--rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_address.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1520 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_app.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1460 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_app_ready_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1386 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_app_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1793 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_apps_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1616 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_apps_status_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1454 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1306 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_icons.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1370 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_install_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1526 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_profiles_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1399 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_system_adb_auth.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1477 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_system_get_prop_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1371 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agent_value_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1376 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_agreed_ack.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1510 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_api_conflict_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1410 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_api_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1623 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_api_internal_consistency_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_api_not_found_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1317 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_api_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1197 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_bit.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1501 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_btrace_enable_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1230 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_button.py
--rw-r--r--   0 sam       (1000) sam       (1000)    21247 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_corellium_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1500 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_coupon_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1329 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_create_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1383 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_created_by.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1409 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_credentials.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1586 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_domain_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1534 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1936 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_features.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1404 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_file_changes.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1882 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_firmware.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1693 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_gpio_state_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2099 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_gpios_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1471 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_grant_trial_request_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1505 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_hook.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1708 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_image.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3538 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1420 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_agent_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1688 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_boot_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_boot_options_additional_tag.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1446 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_console_endpoint.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3031 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_create_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)      842 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1464 2023-02-24 01:35:13.000000 corellium-api-0.2.0/test/test_instance_netmon_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1430 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_instance_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1594 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_instance_services.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1418 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_instance_start_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1309 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_instance_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1405 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_instance_stop_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1457 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_instance_upgrade_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1369 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_invitation.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1393 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_invite_revoke_params.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1401 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_invite_revoke_params_ids.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1340 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_kcrange.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1657 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_kernel_task.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1429 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_kernel_thread.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1368 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_media_play_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1645 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_model.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2368 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_model_software.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1561 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_password_change_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1548 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_password_reset_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1925 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_patch_instance_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1829 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_peripherals_data.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1348 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_plan.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-02-24 02:21:07.000000 corellium-api-0.2.0/test/test_plan_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1933 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_project.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1704 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_project_key.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1394 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_project_quota.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1434 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_project_settings.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1424 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_project_usage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1337 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_rate_info.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1366 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_reset_link_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1387 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_role.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1341 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_rotate_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1609 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_snapshot.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1474 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_snapshot_creation_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1379 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_snapshot_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2291 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_subscriber_invite.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1608 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1300 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_team_create.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1291 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_text_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1382 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1391 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_touch_curve_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1308 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_touch_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1286 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_trial.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1452 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_trial_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1574 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_trial_request_metadata.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2083 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_trial_request_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1362 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_update_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1465 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_user.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1430 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_user_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1664 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_v1_create_hook_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1506 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_v1_load_extension_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1383 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_v1_set_state_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1508 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_validation_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1458 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_volume_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1461 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_vpn_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3402 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_web_player_create_session_request.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1539 2023-02-24 01:35:14.000000 corellium-api-0.2.0/test/test_web_player_session.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.987334 corellium-api-0.3.0/
+-rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-19 23:37:42.987334 corellium-api-0.3.0/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)    28293 2023-04-19 23:26:46.000000 corellium-api-0.3.0/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.891338 corellium-api-0.3.0/corellium_api/
+-rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/__init__.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.891338 corellium-api-0.3.0/corellium_api/api/
+-rw-r--r--   0 sam       (1000) sam       (1000)      144 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/api/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)   856205 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/api/corellium_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    27761 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/api_client.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16369 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/configuration.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5077 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/exceptions.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.951335 corellium-api-0.3.0/corellium_api/models/
+-rw-r--r--   0 sam       (1000) sam       (1000)     6757 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/models/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7295 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/address.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7552 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_app.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3856 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_app_ready_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_app_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4438 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_apps_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4528 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_apps_status_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5936 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3596 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_icons.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3648 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_install_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3921 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_profiles_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3683 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_system_adb_auth.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3948 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_system_get_prop_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3662 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agent_value_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3803 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/agreed_ack.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5801 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_conflict_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5468 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5772 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_internal_consistency_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6107 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_not_found_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3836 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/api_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3055 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/bit.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3704 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/btrace_enable_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3369 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/button.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5898 2023-04-19 23:26:43.000000 corellium-api-0.3.0/corellium_api/models/coupon_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3761 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/create_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5544 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/created_by.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4797 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/credentials.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4661 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/domain_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8135 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16317 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/features.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5471 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/file_changes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13228 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/firmware.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4978 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/gpio_state_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4898 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/gpios_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3712 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/grant_trial_request_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9581 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/hook.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9950 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/image.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    22906 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4239 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_agent_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8955 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_boot_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3479 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_boot_options_additional_tag.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3682 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_console_endpoint.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    14845 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_create_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5707 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5049 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_netmon_proc_map_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4937 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_netmon_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4549 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3600 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_services.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4511 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_start_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3340 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3679 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_stop_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4522 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/instance_upgrade_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5003 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/invitation.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3608 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/invite_revoke_params.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3013 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/invite_revoke_params_ids.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4187 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/kcrange.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5587 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/kernel_task.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4973 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/kernel_thread.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4292 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/media_play_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9967 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/model.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6959 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/model_software.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7408 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/net_mon_proc_map_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5831 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/password_change_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5844 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/password_reset_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6273 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/patch_instance_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9478 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/peripherals_data.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4162 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/plan.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5173 2023-02-24 02:21:07.000000 corellium-api-0.3.0/corellium_api/models/plan_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6358 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8533 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_key.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4880 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_quota.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5102 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_settings.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5461 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/project_usage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6326 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/proxy_config.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5033 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/rate_info.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3885 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/reset_link_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5639 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/role.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4297 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/rotate_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8024 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/snapshot.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3873 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/snapshot_creation_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4254 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/snapshot_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13441 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/subscriber_invite.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5071 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3564 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/team_create.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3572 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/text_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4459 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4351 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/touch_curve_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3714 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/touch_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3829 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5945 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7578 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial_request_metadata.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/trial_request_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3797 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/update_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6883 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/user.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5655 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/user_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6961 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/v1_create_hook_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4008 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/v1_load_extension_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3781 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/v1_set_state_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5757 2023-04-19 23:26:44.000000 corellium-api-0.3.0/corellium_api/models/validation_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5174 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/volume_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/vpn_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7963 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/web_player_create_session_request.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5867 2023-04-19 23:26:45.000000 corellium-api-0.3.0/corellium_api/models/web_player_session.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9860 2023-04-19 23:26:46.000000 corellium-api-0.3.0/corellium_api/rest.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.891338 corellium-api-0.3.0/corellium_api.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     7540 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       57 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       14 2023-04-19 23:37:42.000000 corellium-api-0.3.0/corellium_api.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       69 2023-04-19 23:37:42.987334 corellium-api-0.3.0/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)     1054 2023-04-19 23:26:46.000000 corellium-api-0.3.0/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-19 23:37:42.987334 corellium-api-0.3.0/test/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1424 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_address.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1518 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_app.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1458 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_app_ready_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1384 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_app_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1791 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_apps_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1614 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_apps_status_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1452 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1304 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_icons.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1368 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_install_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_profiles_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1397 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_system_adb_auth.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1475 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_system_get_prop_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1369 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agent_value_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1374 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_agreed_ack.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1508 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_conflict_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1408 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1621 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_internal_consistency_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_not_found_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1315 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_api_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1195 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_bit.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1499 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_btrace_enable_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1228 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_button.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    21773 2023-04-19 23:26:46.000000 corellium-api-0.3.0/test/test_corellium_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1498 2023-04-19 23:26:43.000000 corellium-api-0.3.0/test/test_coupon_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1327 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_create_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_created_by.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1407 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_credentials.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1584 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_domain_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1532 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1934 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_features.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1402 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_file_changes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1880 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_firmware.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1691 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_gpio_state_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2097 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_gpios_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1469 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_grant_trial_request_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1503 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_hook.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1706 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_image.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3752 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1418 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_agent_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1686 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_boot_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_boot_options_additional_tag.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1444 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_console_endpoint.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3029 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_create_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      840 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1543 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_netmon_proc_map_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1462 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_netmon_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_services.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1449 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_start_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1307 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1403 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_stop_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1455 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_instance_upgrade_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1367 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_invitation.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1391 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_invite_revoke_params.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1399 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_invite_revoke_params_ids.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1338 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_kcrange.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1655 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_kernel_task.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1427 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_kernel_thread.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1366 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_media_play_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1643 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_model.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2366 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_model_software.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1837 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_net_mon_proc_map_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1559 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_password_change_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1546 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_password_reset_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_patch_instance_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1827 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_peripherals_data.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1263 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_plan.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-02-24 02:21:07.000000 corellium-api-0.3.0/test/test_plan_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1931 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1702 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_key.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1392 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_quota.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_settings.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1422 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_project_usage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_proxy_config.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1335 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_rate_info.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1364 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_reset_link_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1385 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_role.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1339 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_rotate_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1607 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_snapshot.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1472 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_snapshot_creation_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1377 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_snapshot_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2289 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_subscriber_invite.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1606 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1298 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_team_create.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1289 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_text_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1380 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1389 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_touch_curve_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1306 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_touch_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1284 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1450 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1572 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial_request_metadata.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2081 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_trial_request_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1360 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_update_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1463 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_user.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_user_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1662 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_v1_create_hook_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1504 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_v1_load_extension_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-19 23:26:44.000000 corellium-api-0.3.0/test/test_v1_set_state_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1506 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_validation_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1456 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_volume_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1459 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_vpn_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3400 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_web_player_create_session_request.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1537 2023-04-19 23:26:45.000000 corellium-api-0.3.0/test/test_web_player_session.py
```

### Comparing `corellium-api-0.2.0/README.md` & `corellium-api-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # corellium-api
 REST API to manage your virtual devices.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 4.2.0-6a4b86f
-- Package version: 0.2.0
+- API version: 4.5.0-16740
+- Package version: 0.3.0
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -132,101 +132,105 @@
 *CorelliumApi* | [**v1_create_hook**](docs/CorelliumApi.md#v1_create_hook) | **POST** /v1/instances/{instanceId}/hooks | Create hypervisor hook for Instance
 *CorelliumApi* | [**v1_create_image**](docs/CorelliumApi.md#v1_create_image) | **POST** /v1/images | Create a new Image
 *CorelliumApi* | [**v1_create_instance**](docs/CorelliumApi.md#v1_create_instance) | **POST** /v1/instances | Create Instance
 *CorelliumApi* | [**v1_create_project**](docs/CorelliumApi.md#v1_create_project) | **POST** /v1/projects | Create a Project
 *CorelliumApi* | [**v1_create_snapshot**](docs/CorelliumApi.md#v1_create_snapshot) | **POST** /v1/instances/{instanceId}/snapshots | Create Instance Snapshot
 *CorelliumApi* | [**v1_create_subscriber_invite**](docs/CorelliumApi.md#v1_create_subscriber_invite) | **POST** /v1/billing/invites | Create Subscriber Invite
 *CorelliumApi* | [**v1_create_user**](docs/CorelliumApi.md#v1_create_user) | **POST** /v1/users | Create User
+*CorelliumApi* | [**v1_delete_extension**](docs/CorelliumApi.md#v1_delete_extension) | **DELETE** /v1/extensions/{extensionId} | Delete an existing extension
 *CorelliumApi* | [**v1_delete_hook**](docs/CorelliumApi.md#v1_delete_hook) | **DELETE** /v1/hooks/{hookId} | Delete an existing hypervisor hook
 *CorelliumApi* | [**v1_delete_image**](docs/CorelliumApi.md#v1_delete_image) | **DELETE** /v2/images/{imageId} | Delete Image
 *CorelliumApi* | [**v1_delete_instance**](docs/CorelliumApi.md#v1_delete_instance) | **DELETE** /v1/instances/{instanceId} | Remove Instance
 *CorelliumApi* | [**v1_delete_instance_snapshot**](docs/CorelliumApi.md#v1_delete_instance_snapshot) | **DELETE** /v1/instances/{instanceId}/snapshots/{snapshotId} | Delete a Snapshot
 *CorelliumApi* | [**v1_delete_project**](docs/CorelliumApi.md#v1_delete_project) | **DELETE** /v1/projects/{projectId} | Delete a Project
 *CorelliumApi* | [**v1_delete_snapshot**](docs/CorelliumApi.md#v1_delete_snapshot) | **DELETE** /v1/snapshots/{snapshotId} | Delete a Snapshot
 *CorelliumApi* | [**v1_delete_user**](docs/CorelliumApi.md#v1_delete_user) | **DELETE** /v1/users/{userId} | Delete User
 *CorelliumApi* | [**v1_disable_expose_port**](docs/CorelliumApi.md#v1_disable_expose_port) | **POST** /v1/instances/{instanceId}/exposeport/disable | Disable an exposed port on an instance for device access.
 *CorelliumApi* | [**v1_enable_expose_port**](docs/CorelliumApi.md#v1_enable_expose_port) | **POST** /v1/instances/{instanceId}/exposeport/enable | Enable an exposed port on an instance for device access.
 *CorelliumApi* | [**v1_execute_hyper_trace_hooks**](docs/CorelliumApi.md#v1_execute_hyper_trace_hooks) | **POST** /v1/instances/{instanceId}/hooks/execute | Execute Hooks on an instance
+*CorelliumApi* | [**v1_get_extension_by_id**](docs/CorelliumApi.md#v1_get_extension_by_id) | **GET** /v1/extensions/{extensionId} | Get extension by id
+*CorelliumApi* | [**v1_get_extensions**](docs/CorelliumApi.md#v1_get_extensions) | **GET** /v1/extensions | Get all extensions
 *CorelliumApi* | [**v1_get_hook_by_id**](docs/CorelliumApi.md#v1_get_hook_by_id) | **GET** /v1/hooks/{hookId} | Get hypervisor hook by id
 *CorelliumApi* | [**v1_get_hooks**](docs/CorelliumApi.md#v1_get_hooks) | **GET** /v1/instances/{instanceId}/hooks | Get all hypervisor hooks for Instance
 *CorelliumApi* | [**v1_get_image**](docs/CorelliumApi.md#v1_get_image) | **GET** /v1/images/{imageId} | Get Image Metadata
 *CorelliumApi* | [**v1_get_images**](docs/CorelliumApi.md#v1_get_images) | **GET** /v1/images | Get all Images Metadata
 *CorelliumApi* | [**v1_get_instance**](docs/CorelliumApi.md#v1_get_instance) | **GET** /v1/instances/{instanceId} | Get Instance
 *CorelliumApi* | [**v1_get_instance_console**](docs/CorelliumApi.md#v1_get_instance_console) | **GET** /v1/instances/{instanceId}/console | Get console websocket URL
 *CorelliumApi* | [**v1_get_instance_console_log**](docs/CorelliumApi.md#v1_get_instance_console_log) | **GET** /v1/instances/{instanceId}/consoleLog | Get Console Log
 *CorelliumApi* | [**v1_get_instance_gpios**](docs/CorelliumApi.md#v1_get_instance_gpios) | **GET** /v1/instances/{instanceId}/gpios | Get Instance GPIOs
 *CorelliumApi* | [**v1_get_instance_panics**](docs/CorelliumApi.md#v1_get_instance_panics) | **GET** /v1/instances/{instanceId}/panics | Get Panics
 *CorelliumApi* | [**v1_get_instance_peripherals**](docs/CorelliumApi.md#v1_get_instance_peripherals) | **GET** /v1/instances/{instanceId}/peripherals | Get Instance Peripherals
-*CorelliumApi* | [**v1_get_instance_quick_connect_command**](docs/CorelliumApi.md#v1_get_instance_quick_connect_command) | **GET** /v1/instances/{instanceId}/quickConnectCommand | Recommended SSH Command for Quick Connect
 *CorelliumApi* | [**v1_get_instance_rate**](docs/CorelliumApi.md#v1_get_instance_rate) | **GET** /v1/instances/{instanceId}/rate | Get rate information
 *CorelliumApi* | [**v1_get_instance_screenshot**](docs/CorelliumApi.md#v1_get_instance_screenshot) | **GET** /v1/instances/{instanceId}/screenshot.{format} | Get Instance Screenshot
 *CorelliumApi* | [**v1_get_instance_snapshot**](docs/CorelliumApi.md#v1_get_instance_snapshot) | **GET** /v1/instances/{instanceId}/snapshots/{snapshotId} | Get Instance Snapshot
 *CorelliumApi* | [**v1_get_instance_snapshots**](docs/CorelliumApi.md#v1_get_instance_snapshots) | **GET** /v1/instances/{instanceId}/snapshots | Get Instance Snapshots
-*CorelliumApi* | [**v1_get_instance_state**](docs/CorelliumApi.md#v1_get_instance_state) | **GET** /v1/instances/{instanceId}/state | Get state of Instance
 *CorelliumApi* | [**v1_get_instances**](docs/CorelliumApi.md#v1_get_instances) | **GET** /v1/instances | Get Instances
 *CorelliumApi* | [**v1_get_model_software**](docs/CorelliumApi.md#v1_get_model_software) | **GET** /v1/models/{model}/software | Get Software for Model
 *CorelliumApi* | [**v1_get_models**](docs/CorelliumApi.md#v1_get_models) | **GET** /v1/models | Get Supported Models
 *CorelliumApi* | [**v1_get_project**](docs/CorelliumApi.md#v1_get_project) | **GET** /v1/projects/{projectId} | Get a Project
 *CorelliumApi* | [**v1_get_project_instances**](docs/CorelliumApi.md#v1_get_project_instances) | **GET** /v1/projects/{projectId}/instances | Get Instances in Project
 *CorelliumApi* | [**v1_get_project_keys**](docs/CorelliumApi.md#v1_get_project_keys) | **GET** /v1/projects/{projectId}/keys | Get Project Authorized Keys
 *CorelliumApi* | [**v1_get_project_vpn_config**](docs/CorelliumApi.md#v1_get_project_vpn_config) | **GET** /v1/projects/{projectId}/vpnconfig/{format} | Get Project VPN Configuration
 *CorelliumApi* | [**v1_get_projects**](docs/CorelliumApi.md#v1_get_projects) | **GET** /v1/projects | Get Projects
 *CorelliumApi* | [**v1_get_reset_link_info**](docs/CorelliumApi.md#v1_get_reset_link_info) | **GET** /v1/users/reset-link-info | Send Password Reset Link Info
 *CorelliumApi* | [**v1_get_snapshot**](docs/CorelliumApi.md#v1_get_snapshot) | **GET** /v1/snapshots/{snapshotId} | Get Snapshot
 *CorelliumApi* | [**v1_instances_instance_id_message_post**](docs/CorelliumApi.md#v1_instances_instance_id_message_post) | **POST** /v1/instances/{instanceId}/message | Receive a message on an iOS vm
 *CorelliumApi* | [**v1_kcrange**](docs/CorelliumApi.md#v1_kcrange) | **GET** /v1/instances/{instanceId}/btrace-kcrange | Get Kernel extension ranges
 *CorelliumApi* | [**v1_list_threads**](docs/CorelliumApi.md#v1_list_threads) | **GET** /v1/instances/{instanceId}/strace/thread-list | Get Running Threads (CoreTrace)
+*CorelliumApi* | [**v1_load_extension**](docs/CorelliumApi.md#v1_load_extension) | **POST** /v1/extensions | Load an extension
 *CorelliumApi* | [**v1_media_play**](docs/CorelliumApi.md#v1_media_play) | **POST** /v1/instances/{instanceId}/media/play | Start playing media
 *CorelliumApi* | [**v1_media_stop**](docs/CorelliumApi.md#v1_media_stop) | **POST** /v1/instances/{instanceId}/media/stop | Stop playing media
+*CorelliumApi* | [**v1_parse_extension_json**](docs/CorelliumApi.md#v1_parse_extension_json) | **POST** /v1/extensions/parse/extension.json | Validates extension.json
 *CorelliumApi* | [**v1_patch_instance**](docs/CorelliumApi.md#v1_patch_instance) | **PATCH** /v1/instances/{instanceId} | Update Instance
 *CorelliumApi* | [**v1_pause_instance**](docs/CorelliumApi.md#v1_pause_instance) | **POST** /v1/instances/{instanceId}/pause | Pause an Instance
 *CorelliumApi* | [**v1_post_instance_input**](docs/CorelliumApi.md#v1_post_instance_input) | **POST** /v1/instances/{instanceId}/input | Provide Instance Input
 *CorelliumApi* | [**v1_ready**](docs/CorelliumApi.md#v1_ready) | **GET** /v1/ready | API Status
 *CorelliumApi* | [**v1_reboot_instance**](docs/CorelliumApi.md#v1_reboot_instance) | **POST** /v1/instances/{instanceId}/reboot | Reboot an Instance
 *CorelliumApi* | [**v1_remove_project_key**](docs/CorelliumApi.md#v1_remove_project_key) | **DELETE** /v1/projects/{projectId}/keys/{keyId} | Delete Project Authorized Key
 *CorelliumApi* | [**v1_remove_team_role_from_project**](docs/CorelliumApi.md#v1_remove_team_role_from_project) | **DELETE** /v1/roles/projects/{projectId}/teams/{teamId}/roles/{roleId} | Remove team role from project
 *CorelliumApi* | [**v1_remove_user_from_team**](docs/CorelliumApi.md#v1_remove_user_from_team) | **DELETE** /v1/teams/{teamId}/users/{userId} | Remove user from team
 *CorelliumApi* | [**v1_remove_user_role_from_project**](docs/CorelliumApi.md#v1_remove_user_role_from_project) | **DELETE** /v1/roles/projects/{projectId}/users/{userId}/roles/{roleId} | Remove user role from project
 *CorelliumApi* | [**v1_rename_instance_snapshot**](docs/CorelliumApi.md#v1_rename_instance_snapshot) | **PATCH** /v1/instances/{instanceId}/snapshots/{snapshotId} | Rename a Snapshot
 *CorelliumApi* | [**v1_reset_user_password**](docs/CorelliumApi.md#v1_reset_user_password) | **POST** /v1/users/reset-password | Reset User Password
+*CorelliumApi* | [**v1_restore_backup**](docs/CorelliumApi.md#v1_restore_backup) | **POST** /v1/instances/{instanceId}/restoreBackup | Restore backup
 *CorelliumApi* | [**v1_restore_instance_snapshot**](docs/CorelliumApi.md#v1_restore_instance_snapshot) | **POST** /v1/instances/{instanceId}/snapshots/{snapshotId}/restore | Restore a Snapshot
 *CorelliumApi* | [**v1_roles**](docs/CorelliumApi.md#v1_roles) | **GET** /v1/roles | Get all roles
 *CorelliumApi* | [**v1_rotate_instance**](docs/CorelliumApi.md#v1_rotate_instance) | **POST** /v1/instances/{instanceId}/rotate | Rotate device to specified orientation
 *CorelliumApi* | [**v1_send_user_reset_link**](docs/CorelliumApi.md#v1_send_user_reset_link) | **POST** /v1/users/send-reset-link | Send Password Reset Link
 *CorelliumApi* | [**v1_set_instance_gpios**](docs/CorelliumApi.md#v1_set_instance_gpios) | **PUT** /v1/instances/{instanceId}/gpios | Set Instance GPIOs
 *CorelliumApi* | [**v1_set_instance_peripherals**](docs/CorelliumApi.md#v1_set_instance_peripherals) | **PUT** /v1/instances/{instanceId}/peripherals | Set Instance Peripherals
 *CorelliumApi* | [**v1_set_instance_state**](docs/CorelliumApi.md#v1_set_instance_state) | **PUT** /v1/instances/{instanceId}/state | Set state of Instance
 *CorelliumApi* | [**v1_snapshot_rename**](docs/CorelliumApi.md#v1_snapshot_rename) | **PATCH** /v1/snapshots/{snapshotId} | Rename a Snapshot
 *CorelliumApi* | [**v1_start_core_trace**](docs/CorelliumApi.md#v1_start_core_trace) | **POST** /v1/instances/{instanceId}/strace/enable | Start CoreTrace on an instance
 *CorelliumApi* | [**v1_start_hyper_trace**](docs/CorelliumApi.md#v1_start_hyper_trace) | **POST** /v1/instances/{instanceId}/btrace/enable | Start HyperTrace on an instance
 *CorelliumApi* | [**v1_start_instance**](docs/CorelliumApi.md#v1_start_instance) | **POST** /v1/instances/{instanceId}/start | Start an Instance
+*CorelliumApi* | [**v1_start_net_mon_proc_map**](docs/CorelliumApi.md#v1_start_net_mon_proc_map) | **POST** /v1/instances/{instanceId}/netmonprocmap/enable | Start Enhanced Network Monitor on an instance.
 *CorelliumApi* | [**v1_start_network_monitor**](docs/CorelliumApi.md#v1_start_network_monitor) | **POST** /v1/instances/{instanceId}/sslsplit/enable | Start Network Monitor on an instance.
 *CorelliumApi* | [**v1_stop_core_trace**](docs/CorelliumApi.md#v1_stop_core_trace) | **POST** /v1/instances/{instanceId}/strace/disable | Stop CoreTrace on an instance.
 *CorelliumApi* | [**v1_stop_hyper_trace**](docs/CorelliumApi.md#v1_stop_hyper_trace) | **POST** /v1/instances/{instanceId}/btrace/disable | Stop HyperTrace on an instance.
 *CorelliumApi* | [**v1_stop_instance**](docs/CorelliumApi.md#v1_stop_instance) | **POST** /v1/instances/{instanceId}/stop | Stop an Instance
+*CorelliumApi* | [**v1_stop_net_mon_proc_map**](docs/CorelliumApi.md#v1_stop_net_mon_proc_map) | **POST** /v1/instances/{instanceId}/netmonprocmap/disable | Stop Enhanced Network Monitor on an instance.
 *CorelliumApi* | [**v1_stop_network_monitor**](docs/CorelliumApi.md#v1_stop_network_monitor) | **POST** /v1/instances/{instanceId}/sslsplit/disable | Stop Network Monitor on an instance.
 *CorelliumApi* | [**v1_team_change**](docs/CorelliumApi.md#v1_team_change) | **PATCH** /v1/teams/{teamId} | Update team
 *CorelliumApi* | [**v1_team_create**](docs/CorelliumApi.md#v1_team_create) | **POST** /v1/teams | Create team
 *CorelliumApi* | [**v1_team_delete**](docs/CorelliumApi.md#v1_team_delete) | **DELETE** /v1/teams/{teamId} | Delete team
 *CorelliumApi* | [**v1_teams**](docs/CorelliumApi.md#v1_teams) | **GET** /v1/teams | Get teams
 *CorelliumApi* | [**v1_unpause_instance**](docs/CorelliumApi.md#v1_unpause_instance) | **POST** /v1/instances/{instanceId}/unpause | Unpause an Instance
+*CorelliumApi* | [**v1_update_extension**](docs/CorelliumApi.md#v1_update_extension) | **PUT** /v1/extensions/{extensionId} | Update an existing extension
 *CorelliumApi* | [**v1_update_hook**](docs/CorelliumApi.md#v1_update_hook) | **PUT** /v1/hooks/{hookId} | Update an existing hypervisor hook
 *CorelliumApi* | [**v1_update_project**](docs/CorelliumApi.md#v1_update_project) | **PATCH** /v1/projects/{projectId} | Update a Project
 *CorelliumApi* | [**v1_update_project_settings**](docs/CorelliumApi.md#v1_update_project_settings) | **PATCH** /v1/projects/{projectId}/settings | Change Project Settings
 *CorelliumApi* | [**v1_update_user**](docs/CorelliumApi.md#v1_update_user) | **PATCH** /v1/users/{userId} | Update User
 *CorelliumApi* | [**v1_upgrade_instance**](docs/CorelliumApi.md#v1_upgrade_instance) | **POST** /v1/instances/{instanceId}/upgrade | Upgrade iOS version
 *CorelliumApi* | [**v1_upload_image_data**](docs/CorelliumApi.md#v1_upload_image_data) | **POST** /v1/images/{imageId} | Upload Image Data
 *CorelliumApi* | [**v1_user_agree_terms**](docs/CorelliumApi.md#v1_user_agree_terms) | **POST** /v1/users/agree | Consent to the current terms and conditions
 *CorelliumApi* | [**v1_users_change_password_post**](docs/CorelliumApi.md#v1_users_change_password_post) | **POST** /v1/users/change-password | Change User Password
 *CorelliumApi* | [**v1_users_login**](docs/CorelliumApi.md#v1_users_login) | **POST** /v1/users/login | Log In
-*CorelliumApi* | [**v1_web_player_allowed_domains**](docs/CorelliumApi.md#v1_web_player_allowed_domains) | **GET** /v1/webplayer/allowedDomains | Retrieve the list of allowed domains for all Webplayer sessions
-*CorelliumApi* | [**v1_web_player_create_session**](docs/CorelliumApi.md#v1_web_player_create_session) | **POST** /v1/webplayer | Create a new Webplayer Session
-*CorelliumApi* | [**v1_web_player_destroy_session**](docs/CorelliumApi.md#v1_web_player_destroy_session) | **DELETE** /v1/webplayer/{sessionId} | Tear down a Webplayer Session
-*CorelliumApi* | [**v1_web_player_list_sessions**](docs/CorelliumApi.md#v1_web_player_list_sessions) | **GET** /v1/webplayer | List all Webplayer sessions
-*CorelliumApi* | [**v1_web_player_session_info**](docs/CorelliumApi.md#v1_web_player_session_info) | **GET** /v1/webplayer/{sessionId} | Retrieve Webplayer Session Information
+*CorelliumApi* | [**v2_get_instance_quick_connect_command**](docs/CorelliumApi.md#v2_get_instance_quick_connect_command) | **GET** /v2/instances/{instanceId}/quickConnectCommand | Recommended SSH Command for Quick Connect
+*CorelliumApi* | [**v2_get_instance_state**](docs/CorelliumApi.md#v2_get_instance_state) | **GET** /v2/instances/{instanceId}/state | Get state of Instance
 
 
 ## Documentation For Models
 
  - [Address](docs/Address.md)
  - [AgentApp](docs/AgentApp.md)
  - [AgentAppReadyResponse](docs/AgentAppReadyResponse.md)
@@ -266,14 +270,15 @@
  - [Instance](docs/Instance.md)
  - [InstanceAgentState](docs/InstanceAgentState.md)
  - [InstanceBootOptions](docs/InstanceBootOptions.md)
  - [InstanceBootOptionsAdditionalTag](docs/InstanceBootOptionsAdditionalTag.md)
  - [InstanceConsoleEndpoint](docs/InstanceConsoleEndpoint.md)
  - [InstanceCreateOptions](docs/InstanceCreateOptions.md)
  - [InstanceInput](docs/InstanceInput.md)
+ - [InstanceNetmonProcMapState](docs/InstanceNetmonProcMapState.md)
  - [InstanceNetmonState](docs/InstanceNetmonState.md)
  - [InstanceReturn](docs/InstanceReturn.md)
  - [InstanceServices](docs/InstanceServices.md)
  - [InstanceStartOptions](docs/InstanceStartOptions.md)
  - [InstanceState](docs/InstanceState.md)
  - [InstanceStopOptions](docs/InstanceStopOptions.md)
  - [InstanceUpgradeBody](docs/InstanceUpgradeBody.md)
@@ -282,24 +287,26 @@
  - [InviteRevokeParamsIds](docs/InviteRevokeParamsIds.md)
  - [Kcrange](docs/Kcrange.md)
  - [KernelTask](docs/KernelTask.md)
  - [KernelThread](docs/KernelThread.md)
  - [MediaPlayBody](docs/MediaPlayBody.md)
  - [Model](docs/Model.md)
  - [ModelSoftware](docs/ModelSoftware.md)
+ - [NetMonProcMapFilter](docs/NetMonProcMapFilter.md)
  - [PasswordChangeBody](docs/PasswordChangeBody.md)
  - [PasswordResetBody](docs/PasswordResetBody.md)
  - [PatchInstanceOptions](docs/PatchInstanceOptions.md)
  - [PeripheralsData](docs/PeripheralsData.md)
  - [Plan](docs/Plan.md)
  - [Project](docs/Project.md)
  - [ProjectKey](docs/ProjectKey.md)
  - [ProjectQuota](docs/ProjectQuota.md)
  - [ProjectSettings](docs/ProjectSettings.md)
  - [ProjectUsage](docs/ProjectUsage.md)
+ - [ProxyConfig](docs/ProxyConfig.md)
  - [RateInfo](docs/RateInfo.md)
  - [ResetLinkBody](docs/ResetLinkBody.md)
  - [Role](docs/Role.md)
  - [RotateBody](docs/RotateBody.md)
  - [Snapshot](docs/Snapshot.md)
  - [SnapshotCreationOptions](docs/SnapshotCreationOptions.md)
  - [SnapshotStatus](docs/SnapshotStatus.md)
```

### Comparing `corellium-api-0.2.0/corellium_api/__init__.py` & `corellium-api-0.3.0/corellium_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 # import apis into sdk package
 from corellium_api.api.corellium_api import CorelliumApi
 
 # import ApiClient
 from corellium_api.api_client import ApiClient
 from corellium_api.configuration import Configuration
@@ -68,14 +68,15 @@
 from corellium_api.models.instance import Instance
 from corellium_api.models.instance_agent_state import InstanceAgentState
 from corellium_api.models.instance_boot_options import InstanceBootOptions
 from corellium_api.models.instance_boot_options_additional_tag import InstanceBootOptionsAdditionalTag
 from corellium_api.models.instance_console_endpoint import InstanceConsoleEndpoint
 from corellium_api.models.instance_create_options import InstanceCreateOptions
 from corellium_api.models.instance_input import InstanceInput
+from corellium_api.models.instance_netmon_proc_map_state import InstanceNetmonProcMapState
 from corellium_api.models.instance_netmon_state import InstanceNetmonState
 from corellium_api.models.instance_return import InstanceReturn
 from corellium_api.models.instance_services import InstanceServices
 from corellium_api.models.instance_start_options import InstanceStartOptions
 from corellium_api.models.instance_state import InstanceState
 from corellium_api.models.instance_stop_options import InstanceStopOptions
 from corellium_api.models.instance_upgrade_body import InstanceUpgradeBody
@@ -84,24 +85,26 @@
 from corellium_api.models.invite_revoke_params_ids import InviteRevokeParamsIds
 from corellium_api.models.kcrange import Kcrange
 from corellium_api.models.kernel_task import KernelTask
 from corellium_api.models.kernel_thread import KernelThread
 from corellium_api.models.media_play_body import MediaPlayBody
 from corellium_api.models.model import Model
 from corellium_api.models.model_software import ModelSoftware
+from corellium_api.models.net_mon_proc_map_filter import NetMonProcMapFilter
 from corellium_api.models.password_change_body import PasswordChangeBody
 from corellium_api.models.password_reset_body import PasswordResetBody
 from corellium_api.models.patch_instance_options import PatchInstanceOptions
 from corellium_api.models.peripherals_data import PeripheralsData
 from corellium_api.models.plan import Plan
 from corellium_api.models.project import Project
 from corellium_api.models.project_key import ProjectKey
 from corellium_api.models.project_quota import ProjectQuota
 from corellium_api.models.project_settings import ProjectSettings
 from corellium_api.models.project_usage import ProjectUsage
+from corellium_api.models.proxy_config import ProxyConfig
 from corellium_api.models.rate_info import RateInfo
 from corellium_api.models.reset_link_body import ResetLinkBody
 from corellium_api.models.role import Role
 from corellium_api.models.rotate_body import RotateBody
 from corellium_api.models.snapshot import Snapshot
 from corellium_api.models.snapshot_creation_options import SnapshotCreationOptions
 from corellium_api.models.snapshot_status import SnapshotStatus
```

### Comparing `corellium-api-0.2.0/corellium_api/api/corellium_api.py` & `corellium-api-0.3.0/corellium_api/api/corellium_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -6013,14 +6013,148 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_delete_extension(self, extension_id, **kwargs):  # noqa: E501
+        """Delete an existing extension  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_delete_extension(extension_id, async_req=True)
+        >>> result = thread.get()
+
+        :param extension_id: Extension ID (required)
+        :type extension_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_delete_extension_with_http_info(extension_id, **kwargs)  # noqa: E501
+
+    def v1_delete_extension_with_http_info(self, extension_id, **kwargs):  # noqa: E501
+        """Delete an existing extension  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_delete_extension_with_http_info(extension_id, async_req=True)
+        >>> result = thread.get()
+
+        :param extension_id: Extension ID (required)
+        :type extension_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'extension_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_delete_extension" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'extension_id' is set
+        if self.api_client.client_side_validation and ('extension_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['extension_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `extension_id` when calling `v1_delete_extension`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'extension_id' in local_var_params:
+            path_params['extensionId'] = local_var_params['extension_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {}
+
+        return self.api_client.call_api(
+            '/v1/extensions/{extensionId}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_delete_hook(self, hook_id, **kwargs):  # noqa: E501
         """Delete an existing hypervisor hook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_delete_hook(hook_id, async_req=True)
@@ -7367,14 +7501,301 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_get_extension_by_id(self, extension_id, **kwargs):  # noqa: E501
+        """Get extension by id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_extension_by_id(extension_id, async_req=True)
+        >>> result = thread.get()
+
+        :param extension_id: Extension Id (required)
+        :type extension_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Extension
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_get_extension_by_id_with_http_info(extension_id, **kwargs)  # noqa: E501
+
+    def v1_get_extension_by_id_with_http_info(self, extension_id, **kwargs):  # noqa: E501
+        """Get extension by id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_extension_by_id_with_http_info(extension_id, async_req=True)
+        >>> result = thread.get()
+
+        :param extension_id: Extension Id (required)
+        :type extension_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(Extension, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'extension_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_get_extension_by_id" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'extension_id' is set
+        if self.api_client.client_side_validation and ('extension_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['extension_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `extension_id` when calling `v1_get_extension_by_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'extension_id' in local_var_params:
+            path_params['extensionId'] = local_var_params['extension_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {
+            200: "Extension",
+            400: "UserError",
+            403: "ApiError",
+        }
+
+        return self.api_client.call_api(
+            '/v1/extensions/{extensionId}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
+    def v1_get_extensions(self, **kwargs):  # noqa: E501
+        """Get all extensions  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_extensions(async_req=True)
+        >>> result = thread.get()
+
+        :param limit: limit for pagination results, defaults to 20
+        :type limit: float
+        :param offset: offset for pagination results, defaults to 0
+        :type offset: float
+        :param if_none_match: sha256sum of the last response with the same parameters (optional)
+        :type if_none_match: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: list[Extension]
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_get_extensions_with_http_info(**kwargs)  # noqa: E501
+
+    def v1_get_extensions_with_http_info(self, **kwargs):  # noqa: E501
+        """Get all extensions  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_extensions_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param limit: limit for pagination results, defaults to 20
+        :type limit: float
+        :param offset: offset for pagination results, defaults to 0
+        :type offset: float
+        :param if_none_match: sha256sum of the last response with the same parameters (optional)
+        :type if_none_match: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(list[Extension], status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'limit',
+            'offset',
+            'if_none_match'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_get_extensions" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
+            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
+        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
+            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
+
+        header_params = dict(local_var_params.get('_headers', {}))
+        if 'if_none_match' in local_var_params:
+            header_params['if-none-match'] = local_var_params['if_none_match']  # noqa: E501
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {
+            200: "list[Extension]",
+            304: None,
+            400: "UserError",
+            403: "ApiError",
+        }
+
+        return self.api_client.call_api(
+            '/v1/extensions', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_get_hook_by_id(self, hook_id, **kwargs):  # noqa: E501
         """Get hypervisor hook by id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_get_hook_by_id(hook_id, async_req=True)
@@ -8768,152 +9189,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_get_instance_quick_connect_command(self, instance_id, **kwargs):  # noqa: E501
-        """Recommended SSH Command for Quick Connect  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_instance_quick_connect_command(instance_id, async_req=True)
-        >>> result = thread.get()
-
-        :param instance_id: Instance ID - uuid (required)
-        :type instance_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: str
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_get_instance_quick_connect_command_with_http_info(instance_id, **kwargs)  # noqa: E501
-
-    def v1_get_instance_quick_connect_command_with_http_info(self, instance_id, **kwargs):  # noqa: E501
-        """Recommended SSH Command for Quick Connect  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_instance_quick_connect_command_with_http_info(instance_id, async_req=True)
-        >>> result = thread.get()
-
-        :param instance_id: Instance ID - uuid (required)
-        :type instance_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'instance_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_get_instance_quick_connect_command" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'instance_id' is set
-        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['instance_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_get_instance_quick_connect_command`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'instance_id' in local_var_params:
-            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "str",
-            400: "UserError",
-            403: "ApiError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/instances/{instanceId}/quickConnectCommand', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def v1_get_instance_rate(self, instance_id, **kwargs):  # noqa: E501
         """Get rate information  # noqa: E501
 
         Returns the cost, in microcents, for the instance in the on and off state. Instances are charged $0.25 / day for storage (off) and $0.25 per core per hour (on).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -9487,152 +9770,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_get_instance_state(self, instance_id, **kwargs):  # noqa: E501
-        """Get state of Instance  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_instance_state(instance_id, async_req=True)
-        >>> result = thread.get()
-
-        :param instance_id: Instance ID - uuid (required)
-        :type instance_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: InstanceState
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_get_instance_state_with_http_info(instance_id, **kwargs)  # noqa: E501
-
-    def v1_get_instance_state_with_http_info(self, instance_id, **kwargs):  # noqa: E501
-        """Get state of Instance  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_get_instance_state_with_http_info(instance_id, async_req=True)
-        >>> result = thread.get()
-
-        :param instance_id: Instance ID - uuid (required)
-        :type instance_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(InstanceState, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'instance_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_get_instance_state" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'instance_id' is set
-        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['instance_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_get_instance_state`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'instance_id' in local_var_params:
-            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "InstanceState",
-            403: "ApiError",
-            404: "UserError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/instances/{instanceId}/state', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def v1_get_instances(self, **kwargs):  # noqa: E501
         """Get Instances  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_get_instances(async_req=True)
@@ -11427,14 +11572,158 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_load_extension(self, v1_load_extension_parameters, **kwargs):  # noqa: E501
+        """Load an extension  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_load_extension(v1_load_extension_parameters, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_load_extension_parameters: application/json (required)
+        :type v1_load_extension_parameters: V1LoadExtensionParameters
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Extension
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_load_extension_with_http_info(v1_load_extension_parameters, **kwargs)  # noqa: E501
+
+    def v1_load_extension_with_http_info(self, v1_load_extension_parameters, **kwargs):  # noqa: E501
+        """Load an extension  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_load_extension_with_http_info(v1_load_extension_parameters, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_load_extension_parameters: application/json (required)
+        :type v1_load_extension_parameters: V1LoadExtensionParameters
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(Extension, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'v1_load_extension_parameters'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_load_extension" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'v1_load_extension_parameters' is set
+        if self.api_client.client_side_validation and ('v1_load_extension_parameters' not in local_var_params or  # noqa: E501
+                                                        local_var_params['v1_load_extension_parameters'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `v1_load_extension_parameters` when calling `v1_load_extension`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'v1_load_extension_parameters' in local_var_params:
+            body_params = local_var_params['v1_load_extension_parameters']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = local_var_params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json'],
+                'POST', body_params))  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {
+            200: "Extension",
+            400: "UserError",
+            403: "ApiError",
+        }
+
+        return self.api_client.call_api(
+            '/v1/extensions', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_media_play(self, instance_id, media_play_body, **kwargs):  # noqa: E501
         """Start playing media  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_media_play(instance_id, media_play_body, async_req=True)
@@ -11712,14 +12001,157 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_parse_extension_json(self, extension, **kwargs):  # noqa: E501
+        """Validates extension.json  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_parse_extension_json(extension, async_req=True)
+        >>> result = thread.get()
+
+        :param extension: extension.json contents (required)
+        :type extension: Extension
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_parse_extension_json_with_http_info(extension, **kwargs)  # noqa: E501
+
+    def v1_parse_extension_json_with_http_info(self, extension, **kwargs):  # noqa: E501
+        """Validates extension.json  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_parse_extension_json_with_http_info(extension, async_req=True)
+        >>> result = thread.get()
+
+        :param extension: extension.json contents (required)
+        :type extension: Extension
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'extension'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_parse_extension_json" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'extension' is set
+        if self.api_client.client_side_validation and ('extension' not in local_var_params or  # noqa: E501
+                                                        local_var_params['extension'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `extension` when calling `v1_parse_extension_json`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'extension' in local_var_params:
+            body_params = local_var_params['extension']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = local_var_params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json'],
+                'POST', body_params))  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {
+            200: "object",
+            400: "UserError",
+        }
+
+        return self.api_client.call_api(
+            '/v1/extensions/parse/extension.json', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_patch_instance(self, instance_id, patch_instance_options, **kwargs):  # noqa: E501
         """Update Instance  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_patch_instance(instance_id, patch_instance_options, async_req=True)
@@ -13331,14 +13763,148 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_restore_backup(self, instance_id, **kwargs):  # noqa: E501
+        """Restore backup  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_restore_backup(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_restore_backup_with_http_info(instance_id, **kwargs)  # noqa: E501
+
+    def v1_restore_backup_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Restore backup  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_restore_backup_with_http_info(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'instance_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_restore_backup" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_restore_backup`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {}
+
+        return self.api_client.call_api(
+            '/v1/instances/{instanceId}/restoreBackup', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_restore_instance_snapshot(self, instance_id, snapshot_id, **kwargs):  # noqa: E501
         """Restore a Snapshot  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_restore_instance_snapshot(instance_id, snapshot_id, async_req=True)
@@ -14946,14 +15512,161 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_start_net_mon_proc_map(self, instance_id, **kwargs):  # noqa: E501
+        """Start Enhanced Network Monitor on an instance.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_start_net_mon_proc_map(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param net_mon_proc_map_filter: 
+        :type net_mon_proc_map_filter: NetMonProcMapFilter
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_start_net_mon_proc_map_with_http_info(instance_id, **kwargs)  # noqa: E501
+
+    def v1_start_net_mon_proc_map_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Start Enhanced Network Monitor on an instance.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_start_net_mon_proc_map_with_http_info(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param net_mon_proc_map_filter: 
+        :type net_mon_proc_map_filter: NetMonProcMapFilter
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'instance_id',
+            'net_mon_proc_map_filter'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_start_net_mon_proc_map" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_start_net_mon_proc_map`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'net_mon_proc_map_filter' in local_var_params:
+            body_params = local_var_params['net_mon_proc_map_filter']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = local_var_params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json'],
+                'POST', body_params))  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {}
+
+        return self.api_client.call_api(
+            '/v1/instances/{instanceId}/netmonprocmap/enable', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_start_network_monitor(self, instance_id, **kwargs):  # noqa: E501
         """Start Network Monitor on an instance.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_start_network_monitor(instance_id, async_req=True)
@@ -15495,14 +16208,148 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_stop_net_mon_proc_map(self, instance_id, **kwargs):  # noqa: E501
+        """Stop Enhanced Network Monitor on an instance.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_stop_net_mon_proc_map(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_stop_net_mon_proc_map_with_http_info(instance_id, **kwargs)  # noqa: E501
+
+    def v1_stop_net_mon_proc_map_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Stop Enhanced Network Monitor on an instance.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_stop_net_mon_proc_map_with_http_info(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'instance_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_stop_net_mon_proc_map" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_stop_net_mon_proc_map`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {}
+
+        return self.api_client.call_api(
+            '/v1/instances/{instanceId}/netmonprocmap/disable', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_stop_network_monitor(self, instance_id, **kwargs):  # noqa: E501
         """Stop Network Monitor on an instance.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_stop_network_monitor(instance_id, async_req=True)
@@ -16326,14 +17173,165 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def v1_update_extension(self, extension_id, update_extension, **kwargs):  # noqa: E501
+        """Update an existing extension  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_update_extension(extension_id, update_extension, async_req=True)
+        >>> result = thread.get()
+
+        :param extension_id: Extension ID (required)
+        :type extension_id: str
+        :param update_extension: application/json (required)
+        :type update_extension: UpdateExtension
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_update_extension_with_http_info(extension_id, update_extension, **kwargs)  # noqa: E501
+
+    def v1_update_extension_with_http_info(self, extension_id, update_extension, **kwargs):  # noqa: E501
+        """Update an existing extension  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_update_extension_with_http_info(extension_id, update_extension, async_req=True)
+        >>> result = thread.get()
+
+        :param extension_id: Extension ID (required)
+        :type extension_id: str
+        :param update_extension: application/json (required)
+        :type update_extension: UpdateExtension
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'extension_id',
+            'update_extension'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_update_extension" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'extension_id' is set
+        if self.api_client.client_side_validation and ('extension_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['extension_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `extension_id` when calling `v1_update_extension`")  # noqa: E501
+        # verify the required parameter 'update_extension' is set
+        if self.api_client.client_side_validation and ('update_extension' not in local_var_params or  # noqa: E501
+                                                        local_var_params['update_extension'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `update_extension` when calling `v1_update_extension`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'extension_id' in local_var_params:
+            path_params['extensionId'] = local_var_params['extension_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'update_extension' in local_var_params:
+            body_params = local_var_params['update_extension']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = local_var_params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json'],
+                'PUT', body_params))  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {}
+
+        return self.api_client.call_api(
+            '/v1/extensions/{extensionId}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def v1_update_hook(self, hook_id, v1_create_hook_parameters, **kwargs):  # noqa: E501
         """Update an existing hypervisor hook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_update_hook(hook_id, v1_create_hook_parameters, async_req=True)
@@ -17659,455 +18657,54 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_web_player_allowed_domains(self, **kwargs):  # noqa: E501
-        """Retrieve the list of allowed domains for all Webplayer sessions  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_web_player_allowed_domains(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: WebPlayerSession
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_web_player_allowed_domains_with_http_info(**kwargs)  # noqa: E501
-
-    def v1_web_player_allowed_domains_with_http_info(self, **kwargs):  # noqa: E501
-        """Retrieve the list of allowed domains for all Webplayer sessions  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_web_player_allowed_domains_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(WebPlayerSession, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_web_player_allowed_domains" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "WebPlayerSession",
-            400: "UserError",
-            403: "ApiError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/webplayer/allowedDomains', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
-    def v1_web_player_create_session(self, web_player_create_session_request, **kwargs):  # noqa: E501
-        """Create a new Webplayer Session  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_web_player_create_session(web_player_create_session_request, async_req=True)
-        >>> result = thread.get()
-
-        :param web_player_create_session_request: Request Data (required)
-        :type web_player_create_session_request: WebPlayerCreateSessionRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: WebPlayerSession
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_web_player_create_session_with_http_info(web_player_create_session_request, **kwargs)  # noqa: E501
-
-    def v1_web_player_create_session_with_http_info(self, web_player_create_session_request, **kwargs):  # noqa: E501
-        """Create a new Webplayer Session  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_web_player_create_session_with_http_info(web_player_create_session_request, async_req=True)
-        >>> result = thread.get()
-
-        :param web_player_create_session_request: Request Data (required)
-        :type web_player_create_session_request: WebPlayerCreateSessionRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(WebPlayerSession, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'web_player_create_session_request'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_web_player_create_session" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'web_player_create_session_request' is set
-        if self.api_client.client_side_validation and ('web_player_create_session_request' not in local_var_params or  # noqa: E501
-                                                        local_var_params['web_player_create_session_request'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `web_player_create_session_request` when calling `v1_web_player_create_session`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'web_player_create_session_request' in local_var_params:
-            body_params = local_var_params['web_player_create_session_request']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = local_var_params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json'],
-                'POST', body_params))  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {
-            200: "WebPlayerSession",
-            400: "UserError",
-            403: "ApiError",
-        }
-
-        return self.api_client.call_api(
-            '/v1/webplayer', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
-    def v1_web_player_destroy_session(self, session_id, **kwargs):  # noqa: E501
-        """Tear down a Webplayer Session  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_web_player_destroy_session(session_id, async_req=True)
-        >>> result = thread.get()
-
-        :param session_id: Webplayer Session identifier (required)
-        :type session_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.v1_web_player_destroy_session_with_http_info(session_id, **kwargs)  # noqa: E501
-
-    def v1_web_player_destroy_session_with_http_info(self, session_id, **kwargs):  # noqa: E501
-        """Tear down a Webplayer Session  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1_web_player_destroy_session_with_http_info(session_id, async_req=True)
-        >>> result = thread.get()
-
-        :param session_id: Webplayer Session identifier (required)
-        :type session_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'session_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method v1_web_player_destroy_session" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'session_id' is set
-        if self.api_client.client_side_validation and ('session_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['session_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `session_id` when calling `v1_web_player_destroy_session`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'session_id' in local_var_params:
-            path_params['sessionId'] = local_var_params['session_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['BearerAuth']  # noqa: E501
-
-        response_types_map = {}
-
-        return self.api_client.call_api(
-            '/v1/webplayer/{sessionId}', 'DELETE',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
-    def v1_web_player_list_sessions(self, **kwargs):  # noqa: E501
-        """List all Webplayer sessions  # noqa: E501
+    def v2_get_instance_quick_connect_command(self, instance_id, **kwargs):  # noqa: E501
+        """Recommended SSH Command for Quick Connect  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_web_player_list_sessions(async_req=True)
+        >>> thread = api.v2_get_instance_quick_connect_command(instance_id, async_req=True)
         >>> result = thread.get()
 
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[WebPlayerSession]
+        :rtype: str
         """
         kwargs['_return_http_data_only'] = True
-        return self.v1_web_player_list_sessions_with_http_info(**kwargs)  # noqa: E501
+        return self.v2_get_instance_quick_connect_command_with_http_info(instance_id, **kwargs)  # noqa: E501
 
-    def v1_web_player_list_sessions_with_http_info(self, **kwargs):  # noqa: E501
-        """List all Webplayer sessions  # noqa: E501
+    def v2_get_instance_quick_connect_command_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Recommended SSH Command for Quick Connect  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_web_player_list_sessions_with_http_info(async_req=True)
+        >>> thread = api.v2_get_instance_quick_connect_command_with_http_info(instance_id, async_req=True)
         >>> result = thread.get()
 
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -18121,20 +18718,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(list[WebPlayerSession], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
+            'instance_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -18144,22 +18742,28 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1_web_player_list_sessions" % key
+                    " to method v2_get_instance_quick_connect_command" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v2_get_instance_quick_connect_command`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
 
         query_params = []
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
@@ -18169,21 +18773,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         response_types_map = {
-            200: "list[WebPlayerSession]",
+            200: "str",
             400: "UserError",
             403: "ApiError",
         }
 
         return self.api_client.call_api(
-            '/v1/webplayer', 'GET',
+            '/v2/instances/{instanceId}/quickConnectCommand', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -18191,54 +18795,58 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def v1_web_player_session_info(self, session_id, **kwargs):  # noqa: E501
-        """Retrieve Webplayer Session Information  # noqa: E501
+    def v2_get_instance_state(self, instance_id, **kwargs):  # noqa: E501
+        """Get state of Instance  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_web_player_session_info(session_id, async_req=True)
+        >>> thread = api.v2_get_instance_state(instance_id, async_req=True)
         >>> result = thread.get()
 
-        :param session_id: Webplayer Session identifier (required)
-        :type session_id: str
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param return_attr: The attributes to return.
+        :type return_attr: list[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: WebPlayerSession
+        :rtype: InstanceState
         """
         kwargs['_return_http_data_only'] = True
-        return self.v1_web_player_session_info_with_http_info(session_id, **kwargs)  # noqa: E501
+        return self.v2_get_instance_state_with_http_info(instance_id, **kwargs)  # noqa: E501
 
-    def v1_web_player_session_info_with_http_info(self, session_id, **kwargs):  # noqa: E501
-        """Retrieve Webplayer Session Information  # noqa: E501
+    def v2_get_instance_state_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Get state of Instance  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_web_player_session_info_with_http_info(session_id, async_req=True)
+        >>> thread = api.v2_get_instance_state_with_http_info(instance_id, async_req=True)
         >>> result = thread.get()
 
-        :param session_id: Webplayer Session identifier (required)
-        :type session_id: str
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param return_attr: The attributes to return.
+        :type return_attr: list[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -18252,21 +18860,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(WebPlayerSession, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(InstanceState, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'session_id'
+            'instance_id',
+            'return_attr'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -18276,30 +18885,33 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1_web_player_session_info" % key
+                    " to method v2_get_instance_state" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'session_id' is set
-        if self.api_client.client_side_validation and ('session_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['session_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `session_id` when calling `v1_web_player_session_info`")  # noqa: E501
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v2_get_instance_state`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'session_id' in local_var_params:
-            path_params['sessionId'] = local_var_params['session_id']  # noqa: E501
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
 
         query_params = []
+        if 'return_attr' in local_var_params and local_var_params['return_attr'] is not None:  # noqa: E501
+            query_params.append(('returnAttr', local_var_params['return_attr']))  # noqa: E501
+            collection_formats['returnAttr'] = 'multi'  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -18307,22 +18919,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         response_types_map = {
-            200: "WebPlayerSession",
-            400: "UserError",
+            200: "InstanceState",
             403: "ApiError",
             404: "UserError",
         }
 
         return self.api_client.call_api(
-            '/v1/webplayer/{sessionId}', 'GET',
+            '/v2/instances/{instanceId}/state', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
```

### Comparing `corellium-api-0.2.0/corellium_api/api_client.py` & `corellium-api-0.3.0/corellium_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.2.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.3.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `corellium-api-0.2.0/corellium_api/configuration.py` & `corellium-api-0.3.0/corellium_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -381,16 +381,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.2.0-6a4b86f\n"\
-               "SDK Package Version: 0.2.0".\
+               "Version of the API: 4.5.0-16740\n"\
+               "SDK Package Version: 0.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `corellium-api-0.2.0/corellium_api/exceptions.py` & `corellium-api-0.3.0/corellium_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `corellium-api-0.2.0/corellium_api/models/__init__.py` & `corellium-api-0.3.0/corellium_api/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -53,14 +53,15 @@
 from corellium_api.models.instance import Instance
 from corellium_api.models.instance_agent_state import InstanceAgentState
 from corellium_api.models.instance_boot_options import InstanceBootOptions
 from corellium_api.models.instance_boot_options_additional_tag import InstanceBootOptionsAdditionalTag
 from corellium_api.models.instance_console_endpoint import InstanceConsoleEndpoint
 from corellium_api.models.instance_create_options import InstanceCreateOptions
 from corellium_api.models.instance_input import InstanceInput
+from corellium_api.models.instance_netmon_proc_map_state import InstanceNetmonProcMapState
 from corellium_api.models.instance_netmon_state import InstanceNetmonState
 from corellium_api.models.instance_return import InstanceReturn
 from corellium_api.models.instance_services import InstanceServices
 from corellium_api.models.instance_start_options import InstanceStartOptions
 from corellium_api.models.instance_state import InstanceState
 from corellium_api.models.instance_stop_options import InstanceStopOptions
 from corellium_api.models.instance_upgrade_body import InstanceUpgradeBody
@@ -69,24 +70,26 @@
 from corellium_api.models.invite_revoke_params_ids import InviteRevokeParamsIds
 from corellium_api.models.kcrange import Kcrange
 from corellium_api.models.kernel_task import KernelTask
 from corellium_api.models.kernel_thread import KernelThread
 from corellium_api.models.media_play_body import MediaPlayBody
 from corellium_api.models.model import Model
 from corellium_api.models.model_software import ModelSoftware
+from corellium_api.models.net_mon_proc_map_filter import NetMonProcMapFilter
 from corellium_api.models.password_change_body import PasswordChangeBody
 from corellium_api.models.password_reset_body import PasswordResetBody
 from corellium_api.models.patch_instance_options import PatchInstanceOptions
 from corellium_api.models.peripherals_data import PeripheralsData
 from corellium_api.models.plan import Plan
 from corellium_api.models.project import Project
 from corellium_api.models.project_key import ProjectKey
 from corellium_api.models.project_quota import ProjectQuota
 from corellium_api.models.project_settings import ProjectSettings
 from corellium_api.models.project_usage import ProjectUsage
+from corellium_api.models.proxy_config import ProxyConfig
 from corellium_api.models.rate_info import RateInfo
 from corellium_api.models.reset_link_body import ResetLinkBody
 from corellium_api.models.role import Role
 from corellium_api.models.rotate_body import RotateBody
 from corellium_api.models.snapshot import Snapshot
 from corellium_api.models.snapshot_creation_options import SnapshotCreationOptions
 from corellium_api.models.snapshot_status import SnapshotStatus
```

### Comparing `corellium-api-0.2.0/corellium_api/models/address.py` & `corellium-api-0.3.0/corellium_api/models/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_app.py` & `corellium-api-0.3.0/corellium_api/models/agent_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_app_ready_response.py` & `corellium-api-0.3.0/corellium_api/models/agent_app_ready_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_app_status.py` & `corellium-api-0.3.0/corellium_api/models/agent_app_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_apps_list.py` & `corellium-api-0.3.0/corellium_api/models/agent_apps_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_apps_status_list.py` & `corellium-api-0.3.0/corellium_api/models/agent_apps_status_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_error.py` & `corellium-api-0.3.0/corellium_api/models/agent_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_icons.py` & `corellium-api-0.3.0/corellium_api/models/agent_icons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_install_body.py` & `corellium-api-0.3.0/corellium_api/models/agent_install_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_profiles_return.py` & `corellium-api-0.3.0/corellium_api/models/agent_profiles_return.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_system_adb_auth.py` & `corellium-api-0.3.0/corellium_api/models/agent_system_adb_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_system_get_prop_body.py` & `corellium-api-0.3.0/corellium_api/models/agent_system_get_prop_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agent_value_return.py` & `corellium-api-0.3.0/corellium_api/models/agent_value_return.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/agreed_ack.py` & `corellium-api-0.3.0/corellium_api/models/agreed_ack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/api_conflict_error.py` & `corellium-api-0.3.0/corellium_api/models/api_conflict_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/api_error.py` & `corellium-api-0.3.0/corellium_api/models/api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/api_internal_consistency_error.py` & `corellium-api-0.3.0/corellium_api/models/api_internal_consistency_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/api_not_found_error.py` & `corellium-api-0.3.0/corellium_api/models/api_not_found_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/api_token.py` & `corellium-api-0.3.0/corellium_api/models/api_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/bit.py` & `corellium-api-0.3.0/corellium_api/models/bit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/btrace_enable_options.py` & `corellium-api-0.3.0/corellium_api/models/btrace_enable_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/button.py` & `corellium-api-0.3.0/corellium_api/models/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/coupon_options.py` & `corellium-api-0.3.0/corellium_api/models/coupon_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/create_team.py` & `corellium-api-0.3.0/corellium_api/models/create_team.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/created_by.py` & `corellium-api-0.3.0/corellium_api/models/created_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/credentials.py` & `corellium-api-0.3.0/corellium_api/models/credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/domain_options.py` & `corellium-api-0.3.0/corellium_api/models/domain_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/extension.py` & `corellium-api-0.3.0/corellium_api/models/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/features.py` & `corellium-api-0.3.0/corellium_api/models/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/file_changes.py` & `corellium-api-0.3.0/corellium_api/models/file_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/firmware.py` & `corellium-api-0.3.0/corellium_api/models/firmware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/gpio_state_definition.py` & `corellium-api-0.3.0/corellium_api/models/gpio_state_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/gpios_state.py` & `corellium-api-0.3.0/corellium_api/models/gpios_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/grant_trial_request_response.py` & `corellium-api-0.3.0/corellium_api/models/grant_trial_request_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/hook.py` & `corellium-api-0.3.0/corellium_api/models/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/image.py` & `corellium-api-0.3.0/corellium_api/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -177,15 +177,15 @@
         """Sets the type of this Image.
 
         Type of image  # noqa: E501
 
         :param type: The type of this Image.  # noqa: E501
         :type type: str
         """
-        allowed_values = [None,"fwbinary", "kernel", "devicetree", "ramdisk", "loaderfile", "sepfw", "seprom", "bootrom", "llb", "iboot", "ibootdata", "fwpackage", "partition"]  # noqa: E501
+        allowed_values = [None,"fwbinary", "kernel", "devicetree", "ramdisk", "loaderfile", "sepfw", "seprom", "bootrom", "llb", "iboot", "ibootdata", "fwpackage", "partition", "backup"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance.py` & `corellium-api-0.3.0/corellium_api/models/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -56,14 +56,15 @@
         'panicked': 'bool',
         'created': 'datetime',
         'model': 'str',
         'fwpackage': 'str',
         'os': 'str',
         'agent': 'InstanceAgentState',
         'netmon': 'InstanceNetmonState',
+        'netmonprocmap': 'InstanceNetmonProcMapState',
         'expose_port': 'str',
         'fault': 'bool',
         'patches': 'list[str]',
         'created_by': 'CreatedBy'
     }
 
     attribute_map = {
@@ -87,21 +88,22 @@
         'panicked': 'panicked',
         'created': 'created',
         'model': 'model',
         'fwpackage': 'fwpackage',
         'os': 'os',
         'agent': 'agent',
         'netmon': 'netmon',
+        'netmonprocmap': 'netmonprocmap',
         'expose_port': 'exposePort',
         'fault': 'fault',
         'patches': 'patches',
         'created_by': 'createdBy'
     }
 
-    def __init__(self, id=None, name=None, key=None, flavor=None, type=None, project=None, state=None, state_changed=None, started_at=None, user_task=None, task_state=None, error=None, boot_options=None, service_ip=None, wifi_ip=None, secondary_ip=None, services=None, panicked=None, created=None, model=None, fwpackage=None, os=None, agent=None, netmon=None, expose_port=None, fault=None, patches=None, created_by=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, key=None, flavor=None, type=None, project=None, state=None, state_changed=None, started_at=None, user_task=None, task_state=None, error=None, boot_options=None, service_ip=None, wifi_ip=None, secondary_ip=None, services=None, panicked=None, created=None, model=None, fwpackage=None, os=None, agent=None, netmon=None, netmonprocmap=None, expose_port=None, fault=None, patches=None, created_by=None, local_vars_configuration=None):  # noqa: E501
         """Instance - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
@@ -123,14 +125,15 @@
         self._panicked = None
         self._created = None
         self._model = None
         self._fwpackage = None
         self._os = None
         self._agent = None
         self._netmon = None
+        self._netmonprocmap = None
         self._expose_port = None
         self._fault = None
         self._patches = None
         self._created_by = None
         self.discriminator = None
 
         self.id = id
@@ -156,14 +159,15 @@
         self.panicked = panicked
         self.created = created
         self.model = model
         self.fwpackage = fwpackage
         self.os = os
         self.agent = agent
         self.netmon = netmon
+        self.netmonprocmap = netmonprocmap
         self.expose_port = expose_port
         self.fault = fault
         self.patches = patches
         if created_by is not None:
             self.created_by = created_by
 
     @property
@@ -705,14 +709,35 @@
         :param netmon: The netmon of this Instance.  # noqa: E501
         :type netmon: InstanceNetmonState
         """
 
         self._netmon = netmon
 
     @property
+    def netmonprocmap(self):
+        """Gets the netmonprocmap of this Instance.  # noqa: E501
+
+
+        :return: The netmonprocmap of this Instance.  # noqa: E501
+        :rtype: InstanceNetmonProcMapState
+        """
+        return self._netmonprocmap
+
+    @netmonprocmap.setter
+    def netmonprocmap(self, netmonprocmap):
+        """Sets the netmonprocmap of this Instance.
+
+
+        :param netmonprocmap: The netmonprocmap of this Instance.  # noqa: E501
+        :type netmonprocmap: InstanceNetmonProcMapState
+        """
+
+        self._netmonprocmap = netmonprocmap
+
+    @property
     def expose_port(self):
         """Gets the expose_port of this Instance.  # noqa: E501
 
           # noqa: E501
 
         :return: The expose_port of this Instance.  # noqa: E501
         :rtype: str
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_agent_state.py` & `corellium-api-0.3.0/corellium_api/models/instance_agent_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_boot_options.py` & `corellium-api-0.3.0/corellium_api/models/instance_boot_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_boot_options_additional_tag.py` & `corellium-api-0.3.0/corellium_api/models/instance_boot_options_additional_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_console_endpoint.py` & `corellium-api-0.3.0/corellium_api/models/instance_console_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_create_options.py` & `corellium-api-0.3.0/corellium_api/models/instance_create_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -393,26 +393,26 @@
 
         self._volume = volume
 
     @property
     def snapshot(self):
         """Gets the snapshot of this InstanceCreateOptions.  # noqa: E501
 
-        Snapshot ID  # noqa: E501
+        Snapshot ID for this instance to be cloned from if defined  # noqa: E501
 
         :return: The snapshot of this InstanceCreateOptions.  # noqa: E501
         :rtype: str
         """
         return self._snapshot
 
     @snapshot.setter
     def snapshot(self, snapshot):
         """Sets the snapshot of this InstanceCreateOptions.
 
-        Snapshot ID  # noqa: E501
+        Snapshot ID for this instance to be cloned from if defined  # noqa: E501
 
         :param snapshot: The snapshot of this InstanceCreateOptions.  # noqa: E501
         :type snapshot: str
         """
 
         self._snapshot = snapshot
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_input.py` & `corellium-api-0.3.0/corellium_api/models/instance_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_netmon_state.py` & `corellium-api-0.3.0/corellium_api/models/instance_netmon_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_return.py` & `corellium-api-0.3.0/corellium_api/models/instance_return.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_services.py` & `corellium-api-0.3.0/corellium_api/models/instance_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_start_options.py` & `corellium-api-0.3.0/corellium_api/models/text_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,69 +17,69 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class InstanceStartOptions(object):
+class TextInput(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'paused': 'bool'
+        'text': 'str'
     }
 
     attribute_map = {
-        'paused': 'paused'
+        'text': 'text'
     }
 
-    def __init__(self, paused=None, local_vars_configuration=None):  # noqa: E501
-        """InstanceStartOptions - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, text=None, local_vars_configuration=None):  # noqa: E501
+        """TextInput - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._paused = None
+        self._text = None
         self.discriminator = None
 
-        self.paused = paused
+        self.text = text
 
     @property
-    def paused(self):
-        """Gets the paused of this InstanceStartOptions.  # noqa: E501
+    def text(self):
+        """Gets the text of this TextInput.  # noqa: E501
 
-        Start device paused  # noqa: E501
+        text to type  # noqa: E501
 
-        :return: The paused of this InstanceStartOptions.  # noqa: E501
-        :rtype: bool
+        :return: The text of this TextInput.  # noqa: E501
+        :rtype: str
         """
-        return self._paused
+        return self._text
 
-    @paused.setter
-    def paused(self, paused):
-        """Sets the paused of this InstanceStartOptions.
+    @text.setter
+    def text(self, text):
+        """Sets the text of this TextInput.
 
-        Start device paused  # noqa: E501
+        text to type  # noqa: E501
 
-        :param paused: The paused of this InstanceStartOptions.  # noqa: E501
-        :type paused: bool
+        :param text: The text of this TextInput.  # noqa: E501
+        :type text: str
         """
 
-        self._paused = paused
+        self._text = text
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -115,18 +115,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InstanceStartOptions):
+        if not isinstance(other, TextInput):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InstanceStartOptions):
+        if not isinstance(other, TextInput):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_state.py` & `corellium-api-0.3.0/corellium_api/models/instance_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_stop_options.py` & `corellium-api-0.3.0/corellium_api/models/instance_stop_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/instance_upgrade_body.py` & `corellium-api-0.3.0/corellium_api/models/instance_upgrade_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/invitation.py` & `corellium-api-0.3.0/corellium_api/models/invitation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/invite_revoke_params.py` & `corellium-api-0.3.0/corellium_api/models/invite_revoke_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/invite_revoke_params_ids.py` & `corellium-api-0.3.0/corellium_api/models/invite_revoke_params_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/kcrange.py` & `corellium-api-0.3.0/corellium_api/models/kcrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/kernel_task.py` & `corellium-api-0.3.0/corellium_api/models/kernel_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/kernel_thread.py` & `corellium-api-0.3.0/corellium_api/models/kernel_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/media_play_body.py` & `corellium-api-0.3.0/corellium_api/models/media_play_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/model.py` & `corellium-api-0.3.0/corellium_api/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/model_software.py` & `corellium-api-0.3.0/corellium_api/models/model_software.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/password_change_body.py` & `corellium-api-0.3.0/corellium_api/models/password_change_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/password_reset_body.py` & `corellium-api-0.3.0/corellium_api/models/password_reset_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/patch_instance_options.py` & `corellium-api-0.3.0/corellium_api/models/patch_instance_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -35,15 +35,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'name': 'str',
         'state': 'str',
         'boot_options': 'InstanceBootOptions',
-        'proxy': 'str'
+        'proxy': 'list[ProxyConfig]'
     }
 
     attribute_map = {
         'name': 'name',
         'state': 'state',
         'boot_options': 'bootOptions',
         'proxy': 'proxy'
@@ -143,26 +143,26 @@
     @property
     def proxy(self):
         """Gets the proxy of this PatchInstanceOptions.  # noqa: E501
 
           # noqa: E501
 
         :return: The proxy of this PatchInstanceOptions.  # noqa: E501
-        :rtype: str
+        :rtype: list[ProxyConfig]
         """
         return self._proxy
 
     @proxy.setter
     def proxy(self, proxy):
         """Sets the proxy of this PatchInstanceOptions.
 
           # noqa: E501
 
         :param proxy: The proxy of this PatchInstanceOptions.  # noqa: E501
-        :type proxy: str
+        :type proxy: list[ProxyConfig]
         """
 
         self._proxy = proxy
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `corellium-api-0.2.0/corellium_api/models/peripherals_data.py` & `corellium-api-0.3.0/corellium_api/models/peripherals_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/plan.py` & `corellium-api-0.3.0/corellium_api/models/plan_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 3.11.0-13738
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class Plan(object):
+class PlanOptions(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -42,44 +42,42 @@
 
     attribute_map = {
         'license_type': 'licenseType',
         'cores': 'cores'
     }
 
     def __init__(self, license_type=None, cores=None, local_vars_configuration=None):  # noqa: E501
-        """Plan - a model defined in OpenAPI"""  # noqa: E501
+        """PlanOptions - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._license_type = None
         self._cores = None
         self.discriminator = None
 
         self.license_type = license_type
         self.cores = cores
 
     @property
     def license_type(self):
-        """Gets the license_type of this Plan.  # noqa: E501
+        """Gets the license_type of this PlanOptions.  # noqa: E501
 
-          # noqa: E501
 
-        :return: The license_type of this Plan.  # noqa: E501
+        :return: The license_type of this PlanOptions.  # noqa: E501
         :rtype: str
         """
         return self._license_type
 
     @license_type.setter
     def license_type(self, license_type):
-        """Sets the license_type of this Plan.
+        """Sets the license_type of this PlanOptions.
 
-          # noqa: E501
 
-        :param license_type: The license_type of this Plan.  # noqa: E501
+        :param license_type: The license_type of this PlanOptions.  # noqa: E501
         :type license_type: str
         """
         if self.local_vars_configuration.client_side_validation and license_type is None:  # noqa: E501
             raise ValueError("Invalid value for `license_type`, must not be `None`")  # noqa: E501
         allowed_values = ["premium", "individual", "standard", "enterprise", "individual-usage", "enterprise-usage", "unrestricted"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and license_type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -87,30 +85,30 @@
                 .format(license_type, allowed_values)
             )
 
         self._license_type = license_type
 
     @property
     def cores(self):
-        """Gets the cores of this Plan.  # noqa: E501
+        """Gets the cores of this PlanOptions.  # noqa: E501
 
         Number of CPU cores  # noqa: E501
 
-        :return: The cores of this Plan.  # noqa: E501
+        :return: The cores of this PlanOptions.  # noqa: E501
         :rtype: int
         """
         return self._cores
 
     @cores.setter
     def cores(self, cores):
-        """Sets the cores of this Plan.
+        """Sets the cores of this PlanOptions.
 
         Number of CPU cores  # noqa: E501
 
-        :param cores: The cores of this Plan.  # noqa: E501
+        :param cores: The cores of this PlanOptions.  # noqa: E501
         :type cores: int
         """
         if self.local_vars_configuration.client_side_validation and cores is None:  # noqa: E501
             raise ValueError("Invalid value for `cores`, must not be `None`")  # noqa: E501
 
         self._cores = cores
 
@@ -152,18 +150,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Plan):
+        if not isinstance(other, PlanOptions):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Plan):
+        if not isinstance(other, PlanOptions):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/models/plan_options.py` & `corellium-api-0.3.0/corellium_api/models/trial_extension.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 3.11.0-13738
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,104 +17,150 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class PlanOptions(object):
+class TrialExtension(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'license_type': 'str',
-        'cores': 'int'
+        'duration': 'float',
+        'reason': 'str',
+        'denied': 'bool',
+        'denied_reason': 'str'
     }
 
     attribute_map = {
-        'license_type': 'licenseType',
-        'cores': 'cores'
+        'duration': 'duration',
+        'reason': 'reason',
+        'denied': 'denied',
+        'denied_reason': 'deniedReason'
     }
 
-    def __init__(self, license_type=None, cores=None, local_vars_configuration=None):  # noqa: E501
-        """PlanOptions - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, duration=None, reason=None, denied=None, denied_reason=None, local_vars_configuration=None):  # noqa: E501
+        """TrialExtension - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._license_type = None
-        self._cores = None
+        self._duration = None
+        self._reason = None
+        self._denied = None
+        self._denied_reason = None
         self.discriminator = None
 
-        self.license_type = license_type
-        self.cores = cores
+        self.duration = duration
+        self.reason = reason
+        self.denied = denied
+        self.denied_reason = denied_reason
 
     @property
-    def license_type(self):
-        """Gets the license_type of this PlanOptions.  # noqa: E501
+    def duration(self):
+        """Gets the duration of this TrialExtension.  # noqa: E501
 
+        how many additional days?  # noqa: E501
 
-        :return: The license_type of this PlanOptions.  # noqa: E501
+        :return: The duration of this TrialExtension.  # noqa: E501
+        :rtype: float
+        """
+        return self._duration
+
+    @duration.setter
+    def duration(self, duration):
+        """Sets the duration of this TrialExtension.
+
+        how many additional days?  # noqa: E501
+
+        :param duration: The duration of this TrialExtension.  # noqa: E501
+        :type duration: float
+        """
+
+        self._duration = duration
+
+    @property
+    def reason(self):
+        """Gets the reason of this TrialExtension.  # noqa: E501
+
+        why does the user want more time?  # noqa: E501
+
+        :return: The reason of this TrialExtension.  # noqa: E501
         :rtype: str
         """
-        return self._license_type
+        return self._reason
+
+    @reason.setter
+    def reason(self, reason):
+        """Sets the reason of this TrialExtension.
+
+        why does the user want more time?  # noqa: E501
+
+        :param reason: The reason of this TrialExtension.  # noqa: E501
+        :type reason: str
+        """
+
+        self._reason = reason
+
+    @property
+    def denied(self):
+        """Gets the denied of this TrialExtension.  # noqa: E501
+
+          # noqa: E501
+
+        :return: The denied of this TrialExtension.  # noqa: E501
+        :rtype: bool
+        """
+        return self._denied
+
+    @denied.setter
+    def denied(self, denied):
+        """Sets the denied of this TrialExtension.
 
-    @license_type.setter
-    def license_type(self, license_type):
-        """Sets the license_type of this PlanOptions.
-
-
-        :param license_type: The license_type of this PlanOptions.  # noqa: E501
-        :type license_type: str
-        """
-        if self.local_vars_configuration.client_side_validation and license_type is None:  # noqa: E501
-            raise ValueError("Invalid value for `license_type`, must not be `None`")  # noqa: E501
-        allowed_values = ["premium", "individual", "standard", "enterprise", "individual-usage", "enterprise-usage", "unrestricted"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and license_type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `license_type` ({0}), must be one of {1}"  # noqa: E501
-                .format(license_type, allowed_values)
-            )
+          # noqa: E501
 
-        self._license_type = license_type
+        :param denied: The denied of this TrialExtension.  # noqa: E501
+        :type denied: bool
+        """
+
+        self._denied = denied
 
     @property
-    def cores(self):
-        """Gets the cores of this PlanOptions.  # noqa: E501
+    def denied_reason(self):
+        """Gets the denied_reason of this TrialExtension.  # noqa: E501
 
-        Number of CPU cores  # noqa: E501
+        explanation for why the request was denied  # noqa: E501
 
-        :return: The cores of this PlanOptions.  # noqa: E501
-        :rtype: int
+        :return: The denied_reason of this TrialExtension.  # noqa: E501
+        :rtype: str
         """
-        return self._cores
+        return self._denied_reason
 
-    @cores.setter
-    def cores(self, cores):
-        """Sets the cores of this PlanOptions.
+    @denied_reason.setter
+    def denied_reason(self, denied_reason):
+        """Sets the denied_reason of this TrialExtension.
 
-        Number of CPU cores  # noqa: E501
+        explanation for why the request was denied  # noqa: E501
 
-        :param cores: The cores of this PlanOptions.  # noqa: E501
-        :type cores: int
+        :param denied_reason: The denied_reason of this TrialExtension.  # noqa: E501
+        :type denied_reason: str
         """
-        if self.local_vars_configuration.client_side_validation and cores is None:  # noqa: E501
-            raise ValueError("Invalid value for `cores`, must not be `None`")  # noqa: E501
 
-        self._cores = cores
+        self._denied_reason = denied_reason
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -150,18 +196,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PlanOptions):
+        if not isinstance(other, TrialExtension):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PlanOptions):
+        if not isinstance(other, TrialExtension):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/models/project.py` & `corellium-api-0.3.0/corellium_api/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/project_key.py` & `corellium-api-0.3.0/corellium_api/models/project_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/project_quota.py` & `corellium-api-0.3.0/corellium_api/models/project_quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/project_settings.py` & `corellium-api-0.3.0/corellium_api/models/project_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/project_usage.py` & `corellium-api-0.3.0/corellium_api/models/project_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/rate_info.py` & `corellium-api-0.3.0/corellium_api/models/rate_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/reset_link_body.py` & `corellium-api-0.3.0/corellium_api/models/reset_link_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/role.py` & `corellium-api-0.3.0/corellium_api/models/role.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/rotate_body.py` & `corellium-api-0.3.0/corellium_api/models/rotate_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/snapshot.py` & `corellium-api-0.3.0/corellium_api/models/snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/snapshot_creation_options.py` & `corellium-api-0.3.0/corellium_api/models/snapshot_creation_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/snapshot_status.py` & `corellium-api-0.3.0/corellium_api/models/snapshot_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/subscriber_invite.py` & `corellium-api-0.3.0/corellium_api/models/subscriber_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/team.py` & `corellium-api-0.3.0/corellium_api/models/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/team_create.py` & `corellium-api-0.3.0/corellium_api/models/team_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/text_input.py` & `corellium-api-0.3.0/corellium_api/models/v1_set_state_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,69 +17,69 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class TextInput(object):
+class V1SetStateBody(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'text': 'str'
+        'state': 'InstanceState'
     }
 
     attribute_map = {
-        'text': 'text'
+        'state': 'state'
     }
 
-    def __init__(self, text=None, local_vars_configuration=None):  # noqa: E501
-        """TextInput - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, state=None, local_vars_configuration=None):  # noqa: E501
+        """V1SetStateBody - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._text = None
+        self._state = None
         self.discriminator = None
 
-        self.text = text
+        self.state = state
 
     @property
-    def text(self):
-        """Gets the text of this TextInput.  # noqa: E501
+    def state(self):
+        """Gets the state of this V1SetStateBody.  # noqa: E501
 
-        text to type  # noqa: E501
 
-        :return: The text of this TextInput.  # noqa: E501
-        :rtype: str
+        :return: The state of this V1SetStateBody.  # noqa: E501
+        :rtype: InstanceState
         """
-        return self._text
+        return self._state
 
-    @text.setter
-    def text(self, text):
-        """Sets the text of this TextInput.
+    @state.setter
+    def state(self, state):
+        """Sets the state of this V1SetStateBody.
 
-        text to type  # noqa: E501
 
-        :param text: The text of this TextInput.  # noqa: E501
-        :type text: str
+        :param state: The state of this V1SetStateBody.  # noqa: E501
+        :type state: InstanceState
         """
+        if self.local_vars_configuration.client_side_validation and state is None:  # noqa: E501
+            raise ValueError("Invalid value for `state`, must not be `None`")  # noqa: E501
 
-        self._text = text
+        self._state = state
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -115,18 +115,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TextInput):
+        if not isinstance(other, V1SetStateBody):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TextInput):
+        if not isinstance(other, V1SetStateBody):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/models/token.py` & `corellium-api-0.3.0/corellium_api/models/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/touch_curve_input.py` & `corellium-api-0.3.0/corellium_api/models/touch_curve_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/touch_input.py` & `corellium-api-0.3.0/corellium_api/models/touch_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/trial.py` & `corellium-api-0.3.0/corellium_api/models/trial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/trial_extension.py` & `corellium-api-0.3.0/corellium_api/models/web_player_session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,150 +17,129 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class TrialExtension(object):
+class WebPlayerSession(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'duration': 'float',
-        'reason': 'str',
-        'denied': 'bool',
-        'denied_reason': 'str'
+        'identifier': 'str',
+        'token': 'str',
+        'expiration': 'float'
     }
 
     attribute_map = {
-        'duration': 'duration',
-        'reason': 'reason',
-        'denied': 'denied',
-        'denied_reason': 'deniedReason'
+        'identifier': 'identifier',
+        'token': 'token',
+        'expiration': 'expiration'
     }
 
-    def __init__(self, duration=None, reason=None, denied=None, denied_reason=None, local_vars_configuration=None):  # noqa: E501
-        """TrialExtension - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, identifier=None, token=None, expiration=None, local_vars_configuration=None):  # noqa: E501
+        """WebPlayerSession - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._duration = None
-        self._reason = None
-        self._denied = None
-        self._denied_reason = None
+        self._identifier = None
+        self._token = None
+        self._expiration = None
         self.discriminator = None
 
-        self.duration = duration
-        self.reason = reason
-        self.denied = denied
-        self.denied_reason = denied_reason
+        self.identifier = identifier
+        self.token = token
+        self.expiration = expiration
 
     @property
-    def duration(self):
-        """Gets the duration of this TrialExtension.  # noqa: E501
+    def identifier(self):
+        """Gets the identifier of this WebPlayerSession.  # noqa: E501
 
-        how many additional days?  # noqa: E501
+        New Session Identifier  # noqa: E501
 
-        :return: The duration of this TrialExtension.  # noqa: E501
-        :rtype: float
-        """
-        return self._duration
-
-    @duration.setter
-    def duration(self, duration):
-        """Sets the duration of this TrialExtension.
-
-        how many additional days?  # noqa: E501
-
-        :param duration: The duration of this TrialExtension.  # noqa: E501
-        :type duration: float
-        """
-
-        self._duration = duration
-
-    @property
-    def reason(self):
-        """Gets the reason of this TrialExtension.  # noqa: E501
-
-        why does the user want more time?  # noqa: E501
-
-        :return: The reason of this TrialExtension.  # noqa: E501
+        :return: The identifier of this WebPlayerSession.  # noqa: E501
         :rtype: str
         """
-        return self._reason
+        return self._identifier
 
-    @reason.setter
-    def reason(self, reason):
-        """Sets the reason of this TrialExtension.
+    @identifier.setter
+    def identifier(self, identifier):
+        """Sets the identifier of this WebPlayerSession.
 
-        why does the user want more time?  # noqa: E501
+        New Session Identifier  # noqa: E501
 
-        :param reason: The reason of this TrialExtension.  # noqa: E501
-        :type reason: str
+        :param identifier: The identifier of this WebPlayerSession.  # noqa: E501
+        :type identifier: str
         """
+        if self.local_vars_configuration.client_side_validation and identifier is None:  # noqa: E501
+            raise ValueError("Invalid value for `identifier`, must not be `None`")  # noqa: E501
 
-        self._reason = reason
+        self._identifier = identifier
 
     @property
-    def denied(self):
-        """Gets the denied of this TrialExtension.  # noqa: E501
+    def token(self):
+        """Gets the token of this WebPlayerSession.  # noqa: E501
 
-          # noqa: E501
+        Session Token  # noqa: E501
 
-        :return: The denied of this TrialExtension.  # noqa: E501
-        :rtype: bool
+        :return: The token of this WebPlayerSession.  # noqa: E501
+        :rtype: str
         """
-        return self._denied
+        return self._token
 
-    @denied.setter
-    def denied(self, denied):
-        """Sets the denied of this TrialExtension.
+    @token.setter
+    def token(self, token):
+        """Sets the token of this WebPlayerSession.
 
-          # noqa: E501
+        Session Token  # noqa: E501
 
-        :param denied: The denied of this TrialExtension.  # noqa: E501
-        :type denied: bool
+        :param token: The token of this WebPlayerSession.  # noqa: E501
+        :type token: str
         """
+        if self.local_vars_configuration.client_side_validation and token is None:  # noqa: E501
+            raise ValueError("Invalid value for `token`, must not be `None`")  # noqa: E501
 
-        self._denied = denied
+        self._token = token
 
     @property
-    def denied_reason(self):
-        """Gets the denied_reason of this TrialExtension.  # noqa: E501
+    def expiration(self):
+        """Gets the expiration of this WebPlayerSession.  # noqa: E501
 
-        explanation for why the request was denied  # noqa: E501
+        Expiration in ISO-8601 format e.g. 2022-05-06T02:39:23.000Z  # noqa: E501
 
-        :return: The denied_reason of this TrialExtension.  # noqa: E501
-        :rtype: str
+        :return: The expiration of this WebPlayerSession.  # noqa: E501
+        :rtype: float
         """
-        return self._denied_reason
+        return self._expiration
 
-    @denied_reason.setter
-    def denied_reason(self, denied_reason):
-        """Sets the denied_reason of this TrialExtension.
+    @expiration.setter
+    def expiration(self, expiration):
+        """Sets the expiration of this WebPlayerSession.
 
-        explanation for why the request was denied  # noqa: E501
+        Expiration in ISO-8601 format e.g. 2022-05-06T02:39:23.000Z  # noqa: E501
 
-        :param denied_reason: The denied_reason of this TrialExtension.  # noqa: E501
-        :type denied_reason: str
+        :param expiration: The expiration of this WebPlayerSession.  # noqa: E501
+        :type expiration: float
         """
+        if self.local_vars_configuration.client_side_validation and expiration is None:  # noqa: E501
+            raise ValueError("Invalid value for `expiration`, must not be `None`")  # noqa: E501
 
-        self._denied_reason = denied_reason
+        self._expiration = expiration
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -196,18 +175,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TrialExtension):
+        if not isinstance(other, WebPlayerSession):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TrialExtension):
+        if not isinstance(other, WebPlayerSession):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/models/trial_request_metadata.py` & `corellium-api-0.3.0/corellium_api/models/trial_request_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/trial_request_options.py` & `corellium-api-0.3.0/corellium_api/models/trial_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/update_extension.py` & `corellium-api-0.3.0/corellium_api/models/update_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/user.py` & `corellium-api-0.3.0/corellium_api/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/user_error.py` & `corellium-api-0.3.0/corellium_api/models/user_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/v1_create_hook_parameters.py` & `corellium-api-0.3.0/corellium_api/models/v1_create_hook_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/v1_load_extension_parameters.py` & `corellium-api-0.3.0/corellium_api/models/v1_load_extension_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/v1_set_state_body.py` & `corellium-api-0.3.0/corellium_api/models/plan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,69 +17,96 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class V1SetStateBody(object):
+class Plan(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'state': 'InstanceState'
+        'plan_id': 'str',
+        'name': 'str'
     }
 
     attribute_map = {
-        'state': 'state'
+        'plan_id': 'planId',
+        'name': 'name'
     }
 
-    def __init__(self, state=None, local_vars_configuration=None):  # noqa: E501
-        """V1SetStateBody - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, plan_id=None, name=None, local_vars_configuration=None):  # noqa: E501
+        """Plan - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._state = None
+        self._plan_id = None
+        self._name = None
         self.discriminator = None
 
-        self.state = state
+        self.plan_id = plan_id
+        self.name = name
 
     @property
-    def state(self):
-        """Gets the state of this V1SetStateBody.  # noqa: E501
+    def plan_id(self):
+        """Gets the plan_id of this Plan.  # noqa: E501
 
+        Plan ID  # noqa: E501
 
-        :return: The state of this V1SetStateBody.  # noqa: E501
-        :rtype: InstanceState
+        :return: The plan_id of this Plan.  # noqa: E501
+        :rtype: str
         """
-        return self._state
+        return self._plan_id
 
-    @state.setter
-    def state(self, state):
-        """Sets the state of this V1SetStateBody.
+    @plan_id.setter
+    def plan_id(self, plan_id):
+        """Sets the plan_id of this Plan.
 
+        Plan ID  # noqa: E501
 
-        :param state: The state of this V1SetStateBody.  # noqa: E501
-        :type state: InstanceState
+        :param plan_id: The plan_id of this Plan.  # noqa: E501
+        :type plan_id: str
         """
-        if self.local_vars_configuration.client_side_validation and state is None:  # noqa: E501
-            raise ValueError("Invalid value for `state`, must not be `None`")  # noqa: E501
 
-        self._state = state
+        self._plan_id = plan_id
+
+    @property
+    def name(self):
+        """Gets the name of this Plan.  # noqa: E501
+
+        Plan Name  # noqa: E501
+
+        :return: The name of this Plan.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this Plan.
+
+        Plan Name  # noqa: E501
+
+        :param name: The name of this Plan.  # noqa: E501
+        :type name: str
+        """
+
+        self._name = name
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -115,18 +142,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1SetStateBody):
+        if not isinstance(other, Plan):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1SetStateBody):
+        if not isinstance(other, Plan):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/models/validation_error.py` & `corellium-api-0.3.0/corellium_api/models/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/volume_options.py` & `corellium-api-0.3.0/corellium_api/models/volume_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/vpn_definition.py` & `corellium-api-0.3.0/corellium_api/models/vpn_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/web_player_create_session_request.py` & `corellium-api-0.3.0/corellium_api/models/web_player_create_session_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.2.0/corellium_api/models/web_player_session.py` & `corellium-api-0.3.0/corellium_api/models/instance_netmon_proc_map_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -17,129 +17,123 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from corellium_api.configuration import Configuration
 
 
-class WebPlayerSession(object):
+class InstanceNetmonProcMapState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'identifier': 'str',
-        'token': 'str',
-        'expiration': 'float'
+        'hash': 'str',
+        'info': 'str',
+        'enabled': 'bool'
     }
 
     attribute_map = {
-        'identifier': 'identifier',
-        'token': 'token',
-        'expiration': 'expiration'
+        'hash': 'hash',
+        'info': 'info',
+        'enabled': 'enabled'
     }
 
-    def __init__(self, identifier=None, token=None, expiration=None, local_vars_configuration=None):  # noqa: E501
-        """WebPlayerSession - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, hash=None, info=None, enabled=None, local_vars_configuration=None):  # noqa: E501
+        """InstanceNetmonProcMapState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._identifier = None
-        self._token = None
-        self._expiration = None
+        self._hash = None
+        self._info = None
+        self._enabled = None
         self.discriminator = None
 
-        self.identifier = identifier
-        self.token = token
-        self.expiration = expiration
+        self.hash = hash
+        self.info = info
+        self.enabled = enabled
 
     @property
-    def identifier(self):
-        """Gets the identifier of this WebPlayerSession.  # noqa: E501
+    def hash(self):
+        """Gets the hash of this InstanceNetmonProcMapState.  # noqa: E501
 
-        New Session Identifier  # noqa: E501
+          # noqa: E501
 
-        :return: The identifier of this WebPlayerSession.  # noqa: E501
+        :return: The hash of this InstanceNetmonProcMapState.  # noqa: E501
         :rtype: str
         """
-        return self._identifier
+        return self._hash
 
-    @identifier.setter
-    def identifier(self, identifier):
-        """Sets the identifier of this WebPlayerSession.
+    @hash.setter
+    def hash(self, hash):
+        """Sets the hash of this InstanceNetmonProcMapState.
 
-        New Session Identifier  # noqa: E501
+          # noqa: E501
 
-        :param identifier: The identifier of this WebPlayerSession.  # noqa: E501
-        :type identifier: str
+        :param hash: The hash of this InstanceNetmonProcMapState.  # noqa: E501
+        :type hash: str
         """
-        if self.local_vars_configuration.client_side_validation and identifier is None:  # noqa: E501
-            raise ValueError("Invalid value for `identifier`, must not be `None`")  # noqa: E501
 
-        self._identifier = identifier
+        self._hash = hash
 
     @property
-    def token(self):
-        """Gets the token of this WebPlayerSession.  # noqa: E501
+    def info(self):
+        """Gets the info of this InstanceNetmonProcMapState.  # noqa: E501
 
-        Session Token  # noqa: E501
+          # noqa: E501
 
-        :return: The token of this WebPlayerSession.  # noqa: E501
+        :return: The info of this InstanceNetmonProcMapState.  # noqa: E501
         :rtype: str
         """
-        return self._token
+        return self._info
 
-    @token.setter
-    def token(self, token):
-        """Sets the token of this WebPlayerSession.
+    @info.setter
+    def info(self, info):
+        """Sets the info of this InstanceNetmonProcMapState.
 
-        Session Token  # noqa: E501
+          # noqa: E501
 
-        :param token: The token of this WebPlayerSession.  # noqa: E501
-        :type token: str
+        :param info: The info of this InstanceNetmonProcMapState.  # noqa: E501
+        :type info: str
         """
-        if self.local_vars_configuration.client_side_validation and token is None:  # noqa: E501
-            raise ValueError("Invalid value for `token`, must not be `None`")  # noqa: E501
 
-        self._token = token
+        self._info = info
 
     @property
-    def expiration(self):
-        """Gets the expiration of this WebPlayerSession.  # noqa: E501
+    def enabled(self):
+        """Gets the enabled of this InstanceNetmonProcMapState.  # noqa: E501
 
-        Expiration in ISO-8601 format e.g. 2022-05-06T02:39:23.000Z  # noqa: E501
+          # noqa: E501
 
-        :return: The expiration of this WebPlayerSession.  # noqa: E501
-        :rtype: float
+        :return: The enabled of this InstanceNetmonProcMapState.  # noqa: E501
+        :rtype: bool
         """
-        return self._expiration
+        return self._enabled
 
-    @expiration.setter
-    def expiration(self, expiration):
-        """Sets the expiration of this WebPlayerSession.
+    @enabled.setter
+    def enabled(self, enabled):
+        """Sets the enabled of this InstanceNetmonProcMapState.
 
-        Expiration in ISO-8601 format e.g. 2022-05-06T02:39:23.000Z  # noqa: E501
+          # noqa: E501
 
-        :param expiration: The expiration of this WebPlayerSession.  # noqa: E501
-        :type expiration: float
+        :param enabled: The enabled of this InstanceNetmonProcMapState.  # noqa: E501
+        :type enabled: bool
         """
-        if self.local_vars_configuration.client_side_validation and expiration is None:  # noqa: E501
-            raise ValueError("Invalid value for `expiration`, must not be `None`")  # noqa: E501
 
-        self._expiration = expiration
+        self._enabled = enabled
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -175,18 +169,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WebPlayerSession):
+        if not isinstance(other, InstanceNetmonProcMapState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, WebPlayerSession):
+        if not isinstance(other, InstanceNetmonProcMapState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `corellium-api-0.2.0/corellium_api/rest.py` & `corellium-api-0.3.0/corellium_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `corellium-api-0.2.0/corellium_api.egg-info/SOURCES.txt` & `corellium-api-0.3.0/corellium_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 corellium_api/models/instance.py
 corellium_api/models/instance_agent_state.py
 corellium_api/models/instance_boot_options.py
 corellium_api/models/instance_boot_options_additional_tag.py
 corellium_api/models/instance_console_endpoint.py
 corellium_api/models/instance_create_options.py
 corellium_api/models/instance_input.py
+corellium_api/models/instance_netmon_proc_map_state.py
 corellium_api/models/instance_netmon_state.py
 corellium_api/models/instance_return.py
 corellium_api/models/instance_services.py
 corellium_api/models/instance_start_options.py
 corellium_api/models/instance_state.py
 corellium_api/models/instance_stop_options.py
 corellium_api/models/instance_upgrade_body.py
@@ -69,25 +70,27 @@
 corellium_api/models/invite_revoke_params_ids.py
 corellium_api/models/kcrange.py
 corellium_api/models/kernel_task.py
 corellium_api/models/kernel_thread.py
 corellium_api/models/media_play_body.py
 corellium_api/models/model.py
 corellium_api/models/model_software.py
+corellium_api/models/net_mon_proc_map_filter.py
 corellium_api/models/password_change_body.py
 corellium_api/models/password_reset_body.py
 corellium_api/models/patch_instance_options.py
 corellium_api/models/peripherals_data.py
 corellium_api/models/plan.py
 corellium_api/models/plan_options.py
 corellium_api/models/project.py
 corellium_api/models/project_key.py
 corellium_api/models/project_quota.py
 corellium_api/models/project_settings.py
 corellium_api/models/project_usage.py
+corellium_api/models/proxy_config.py
 corellium_api/models/rate_info.py
 corellium_api/models/reset_link_body.py
 corellium_api/models/role.py
 corellium_api/models/rotate_body.py
 corellium_api/models/snapshot.py
 corellium_api/models/snapshot_creation_options.py
 corellium_api/models/snapshot_status.py
@@ -153,14 +156,15 @@
 test/test_instance.py
 test/test_instance_agent_state.py
 test/test_instance_boot_options.py
 test/test_instance_boot_options_additional_tag.py
 test/test_instance_console_endpoint.py
 test/test_instance_create_options.py
 test/test_instance_input.py
+test/test_instance_netmon_proc_map_state.py
 test/test_instance_netmon_state.py
 test/test_instance_return.py
 test/test_instance_services.py
 test/test_instance_start_options.py
 test/test_instance_state.py
 test/test_instance_stop_options.py
 test/test_instance_upgrade_body.py
@@ -169,25 +173,27 @@
 test/test_invite_revoke_params_ids.py
 test/test_kcrange.py
 test/test_kernel_task.py
 test/test_kernel_thread.py
 test/test_media_play_body.py
 test/test_model.py
 test/test_model_software.py
+test/test_net_mon_proc_map_filter.py
 test/test_password_change_body.py
 test/test_password_reset_body.py
 test/test_patch_instance_options.py
 test/test_peripherals_data.py
 test/test_plan.py
 test/test_plan_options.py
 test/test_project.py
 test/test_project_key.py
 test/test_project_quota.py
 test/test_project_settings.py
 test/test_project_usage.py
+test/test_proxy_config.py
 test/test_rate_info.py
 test/test_reset_link_body.py
 test/test_role.py
 test/test_rotate_body.py
 test/test_snapshot.py
 test/test_snapshot_creation_options.py
 test/test_snapshot_status.py
```

### Comparing `corellium-api-0.2.0/setup.py` & `corellium-api-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "corellium-api"
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `corellium-api-0.2.0/test/test_address.py` & `corellium-api-0.3.0/test/test_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_app.py` & `corellium-api-0.3.0/test/test_agent_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_app_ready_response.py` & `corellium-api-0.3.0/test/test_agent_app_ready_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_app_status.py` & `corellium-api-0.3.0/test/test_agent_app_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_apps_list.py` & `corellium-api-0.3.0/test/test_agent_apps_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_apps_status_list.py` & `corellium-api-0.3.0/test/test_agent_apps_status_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_error.py` & `corellium-api-0.3.0/test/test_agent_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_icons.py` & `corellium-api-0.3.0/test/test_agent_icons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_install_body.py` & `corellium-api-0.3.0/test/test_agent_install_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_profiles_return.py` & `corellium-api-0.3.0/test/test_agent_profiles_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_system_adb_auth.py` & `corellium-api-0.3.0/test/test_agent_system_adb_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_system_get_prop_body.py` & `corellium-api-0.3.0/test/test_agent_system_get_prop_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agent_value_return.py` & `corellium-api-0.3.0/test/test_agent_value_return.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_agreed_ack.py` & `corellium-api-0.3.0/test/test_agreed_ack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_api_conflict_error.py` & `corellium-api-0.3.0/test/test_api_conflict_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_api_error.py` & `corellium-api-0.3.0/test/test_api_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_api_internal_consistency_error.py` & `corellium-api-0.3.0/test/test_api_internal_consistency_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_api_not_found_error.py` & `corellium-api-0.3.0/test/test_api_not_found_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_api_token.py` & `corellium-api-0.3.0/test/test_api_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_bit.py` & `corellium-api-0.3.0/test/test_bit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_btrace_enable_options.py` & `corellium-api-0.3.0/test/test_btrace_enable_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_button.py` & `corellium-api-0.3.0/test/test_button.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_corellium_api.py` & `corellium-api-0.3.0/test/test_corellium_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -311,14 +311,21 @@
     def test_v1_create_user(self):
         """Test case for v1_create_user
 
         Create User  # noqa: E501
         """
         pass
 
+    def test_v1_delete_extension(self):
+        """Test case for v1_delete_extension
+
+        Delete an existing extension  # noqa: E501
+        """
+        pass
+
     def test_v1_delete_hook(self):
         """Test case for v1_delete_hook
 
         Delete an existing hypervisor hook  # noqa: E501
         """
         pass
 
@@ -381,14 +388,28 @@
     def test_v1_execute_hyper_trace_hooks(self):
         """Test case for v1_execute_hyper_trace_hooks
 
         Execute Hooks on an instance  # noqa: E501
         """
         pass
 
+    def test_v1_get_extension_by_id(self):
+        """Test case for v1_get_extension_by_id
+
+        Get extension by id  # noqa: E501
+        """
+        pass
+
+    def test_v1_get_extensions(self):
+        """Test case for v1_get_extensions
+
+        Get all extensions  # noqa: E501
+        """
+        pass
+
     def test_v1_get_hook_by_id(self):
         """Test case for v1_get_hook_by_id
 
         Get hypervisor hook by id  # noqa: E501
         """
         pass
 
@@ -451,21 +472,14 @@
     def test_v1_get_instance_peripherals(self):
         """Test case for v1_get_instance_peripherals
 
         Get Instance Peripherals  # noqa: E501
         """
         pass
 
-    def test_v1_get_instance_quick_connect_command(self):
-        """Test case for v1_get_instance_quick_connect_command
-
-        Recommended SSH Command for Quick Connect  # noqa: E501
-        """
-        pass
-
     def test_v1_get_instance_rate(self):
         """Test case for v1_get_instance_rate
 
         Get rate information  # noqa: E501
         """
         pass
 
@@ -486,21 +500,14 @@
     def test_v1_get_instance_snapshots(self):
         """Test case for v1_get_instance_snapshots
 
         Get Instance Snapshots  # noqa: E501
         """
         pass
 
-    def test_v1_get_instance_state(self):
-        """Test case for v1_get_instance_state
-
-        Get state of Instance  # noqa: E501
-        """
-        pass
-
     def test_v1_get_instances(self):
         """Test case for v1_get_instances
 
         Get Instances  # noqa: E501
         """
         pass
 
@@ -584,28 +591,42 @@
     def test_v1_list_threads(self):
         """Test case for v1_list_threads
 
         Get Running Threads (CoreTrace)  # noqa: E501
         """
         pass
 
+    def test_v1_load_extension(self):
+        """Test case for v1_load_extension
+
+        Load an extension  # noqa: E501
+        """
+        pass
+
     def test_v1_media_play(self):
         """Test case for v1_media_play
 
         Start playing media  # noqa: E501
         """
         pass
 
     def test_v1_media_stop(self):
         """Test case for v1_media_stop
 
         Stop playing media  # noqa: E501
         """
         pass
 
+    def test_v1_parse_extension_json(self):
+        """Test case for v1_parse_extension_json
+
+        Validates extension.json  # noqa: E501
+        """
+        pass
+
     def test_v1_patch_instance(self):
         """Test case for v1_patch_instance
 
         Update Instance  # noqa: E501
         """
         pass
 
@@ -675,14 +696,21 @@
     def test_v1_reset_user_password(self):
         """Test case for v1_reset_user_password
 
         Reset User Password  # noqa: E501
         """
         pass
 
+    def test_v1_restore_backup(self):
+        """Test case for v1_restore_backup
+
+        Restore backup  # noqa: E501
+        """
+        pass
+
     def test_v1_restore_instance_snapshot(self):
         """Test case for v1_restore_instance_snapshot
 
         Restore a Snapshot  # noqa: E501
         """
         pass
 
@@ -752,14 +780,21 @@
     def test_v1_start_instance(self):
         """Test case for v1_start_instance
 
         Start an Instance  # noqa: E501
         """
         pass
 
+    def test_v1_start_net_mon_proc_map(self):
+        """Test case for v1_start_net_mon_proc_map
+
+        Start Enhanced Network Monitor on an instance.  # noqa: E501
+        """
+        pass
+
     def test_v1_start_network_monitor(self):
         """Test case for v1_start_network_monitor
 
         Start Network Monitor on an instance.  # noqa: E501
         """
         pass
 
@@ -780,14 +815,21 @@
     def test_v1_stop_instance(self):
         """Test case for v1_stop_instance
 
         Stop an Instance  # noqa: E501
         """
         pass
 
+    def test_v1_stop_net_mon_proc_map(self):
+        """Test case for v1_stop_net_mon_proc_map
+
+        Stop Enhanced Network Monitor on an instance.  # noqa: E501
+        """
+        pass
+
     def test_v1_stop_network_monitor(self):
         """Test case for v1_stop_network_monitor
 
         Stop Network Monitor on an instance.  # noqa: E501
         """
         pass
 
@@ -822,14 +864,21 @@
     def test_v1_unpause_instance(self):
         """Test case for v1_unpause_instance
 
         Unpause an Instance  # noqa: E501
         """
         pass
 
+    def test_v1_update_extension(self):
+        """Test case for v1_update_extension
+
+        Update an existing extension  # noqa: E501
+        """
+        pass
+
     def test_v1_update_hook(self):
         """Test case for v1_update_hook
 
         Update an existing hypervisor hook  # noqa: E501
         """
         pass
 
@@ -885,45 +934,24 @@
     def test_v1_users_login(self):
         """Test case for v1_users_login
 
         Log In  # noqa: E501
         """
         pass
 
-    def test_v1_web_player_allowed_domains(self):
-        """Test case for v1_web_player_allowed_domains
-
-        Retrieve the list of allowed domains for all Webplayer sessions  # noqa: E501
-        """
-        pass
-
-    def test_v1_web_player_create_session(self):
-        """Test case for v1_web_player_create_session
-
-        Create a new Webplayer Session  # noqa: E501
-        """
-        pass
+    def test_v2_get_instance_quick_connect_command(self):
+        """Test case for v2_get_instance_quick_connect_command
 
-    def test_v1_web_player_destroy_session(self):
-        """Test case for v1_web_player_destroy_session
-
-        Tear down a Webplayer Session  # noqa: E501
-        """
-        pass
-
-    def test_v1_web_player_list_sessions(self):
-        """Test case for v1_web_player_list_sessions
-
-        List all Webplayer sessions  # noqa: E501
+        Recommended SSH Command for Quick Connect  # noqa: E501
         """
         pass
 
-    def test_v1_web_player_session_info(self):
-        """Test case for v1_web_player_session_info
+    def test_v2_get_instance_state(self):
+        """Test case for v2_get_instance_state
 
-        Retrieve Webplayer Session Information  # noqa: E501
+        Get state of Instance  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `corellium-api-0.2.0/test/test_coupon_options.py` & `corellium-api-0.3.0/test/test_coupon_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_create_team.py` & `corellium-api-0.3.0/test/test_create_team.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_created_by.py` & `corellium-api-0.3.0/test/test_created_by.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_credentials.py` & `corellium-api-0.3.0/test/test_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_domain_options.py` & `corellium-api-0.3.0/test/test_domain_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_extension.py` & `corellium-api-0.3.0/test/test_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_features.py` & `corellium-api-0.3.0/test/test_features.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_file_changes.py` & `corellium-api-0.3.0/test/test_file_changes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_firmware.py` & `corellium-api-0.3.0/test/test_firmware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_gpio_state_definition.py` & `corellium-api-0.3.0/test/test_gpio_state_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_gpios_state.py` & `corellium-api-0.3.0/test/test_gpios_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_grant_trial_request_response.py` & `corellium-api-0.3.0/test/test_grant_trial_request_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_hook.py` & `corellium-api-0.3.0/test/test_hook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_image.py` & `corellium-api-0.3.0/test/test_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance.py` & `corellium-api-0.3.0/test/test_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -78,14 +78,18 @@
                 agent = corellium_api.models.instance_agent_state.InstanceAgentState(
                     hash = '', 
                     info = '', ), 
                 netmon = corellium_api.models.instance_netmon_state.InstanceNetmonState(
                     hash = '', 
                     info = '', 
                     enabled = True, ), 
+                netmonprocmap = corellium_api.models.instance_netmon_proc_map_state.InstanceNetmonProcMapState(
+                    hash = '', 
+                    info = '', 
+                    enabled = True, ), 
                 expose_port = '', 
                 fault = True, 
                 patches = [
                     ''
                     ], 
                 created_by = corellium_api.models.created_by.createdBy(
                     id = '',
```

### Comparing `corellium-api-0.2.0/test/test_instance_agent_state.py` & `corellium-api-0.3.0/test/test_instance_agent_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_boot_options.py` & `corellium-api-0.3.0/test/test_instance_boot_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_boot_options_additional_tag.py` & `corellium-api-0.3.0/test/test_instance_boot_options_additional_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_console_endpoint.py` & `corellium-api-0.3.0/test/test_instance_console_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_create_options.py` & `corellium-api-0.3.0/test/test_instance_create_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_input.py` & `corellium-api-0.3.0/test/test_instance_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_netmon_state.py` & `corellium-api-0.3.0/test/test_instance_netmon_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_return.py` & `corellium-api-0.3.0/test/test_instance_return.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_services.py` & `corellium-api-0.3.0/test/test_instance_services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_start_options.py` & `corellium-api-0.3.0/test/test_instance_start_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -32,15 +32,16 @@
         """Test InstanceStartOptions
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = corellium_api.models.instance_start_options.InstanceStartOptions()  # noqa: E501
         if include_optional :
             return InstanceStartOptions(
-                paused = True
+                paused = True, 
+                sockcap = True
             )
         else :
             return InstanceStartOptions(
         )
 
     def testInstanceStartOptions(self):
         """Test InstanceStartOptions"""
```

### Comparing `corellium-api-0.2.0/test/test_instance_state.py` & `corellium-api-0.3.0/test/test_instance_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_stop_options.py` & `corellium-api-0.3.0/test/test_instance_stop_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_instance_upgrade_body.py` & `corellium-api-0.3.0/test/test_instance_upgrade_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_invitation.py` & `corellium-api-0.3.0/test/test_invitation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_invite_revoke_params.py` & `corellium-api-0.3.0/test/test_invite_revoke_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_invite_revoke_params_ids.py` & `corellium-api-0.3.0/test/test_invite_revoke_params_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_kcrange.py` & `corellium-api-0.3.0/test/test_kcrange.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_kernel_task.py` & `corellium-api-0.3.0/test/test_kernel_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_kernel_thread.py` & `corellium-api-0.3.0/test/test_kernel_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_media_play_body.py` & `corellium-api-0.3.0/test/test_media_play_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_model.py` & `corellium-api-0.3.0/test/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_model_software.py` & `corellium-api-0.3.0/test/test_model_software.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_password_change_body.py` & `corellium-api-0.3.0/test/test_password_change_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_password_reset_body.py` & `corellium-api-0.3.0/test/test_password_reset_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_patch_instance_options.py` & `corellium-api-0.3.0/test/test_patch_instance_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -45,15 +45,21 @@
                     ecid = '', 
                     random_seed = '', 
                     pac = True, 
                     aprr = True, 
                     additional_tags = [
                         'kalloc'
                         ], ), 
-                proxy = ''
+                proxy = [
+                    corellium_api.models.proxy_config.ProxyConfig(
+                        device_port = 1.337, 
+                        first_available = True, 
+                        expose = True, 
+                        router_port = 1.337, )
+                    ]
             )
         else :
             return PatchInstanceOptions(
         )
 
     def testPatchInstanceOptions(self):
         """Test PatchInstanceOptions"""
```

### Comparing `corellium-api-0.2.0/test/test_peripherals_data.py` & `corellium-api-0.3.0/test/test_peripherals_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_plan.py` & `corellium-api-0.3.0/test/test_plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -32,21 +32,19 @@
         """Test Plan
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = corellium_api.models.plan.Plan()  # noqa: E501
         if include_optional :
             return Plan(
-                license_type = 'premium', 
-                cores = 56
+                plan_id = '', 
+                name = ''
             )
         else :
             return Plan(
-                license_type = 'premium',
-                cores = 56,
         )
 
     def testPlan(self):
         """Test Plan"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `corellium-api-0.2.0/test/test_plan_options.py` & `corellium-api-0.3.0/test/test_plan_options.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.2.0/test/test_project.py` & `corellium-api-0.3.0/test/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_project_key.py` & `corellium-api-0.3.0/test/test_project_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_project_quota.py` & `corellium-api-0.3.0/test/test_project_quota.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_project_settings.py` & `corellium-api-0.3.0/test/test_project_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_project_usage.py` & `corellium-api-0.3.0/test/test_project_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_rate_info.py` & `corellium-api-0.3.0/test/test_rate_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_reset_link_body.py` & `corellium-api-0.3.0/test/test_reset_link_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_role.py` & `corellium-api-0.3.0/test/test_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_rotate_body.py` & `corellium-api-0.3.0/test/test_rotate_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_snapshot.py` & `corellium-api-0.3.0/test/test_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_snapshot_creation_options.py` & `corellium-api-0.3.0/test/test_snapshot_creation_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_snapshot_status.py` & `corellium-api-0.3.0/test/test_snapshot_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_subscriber_invite.py` & `corellium-api-0.3.0/test/test_subscriber_invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_team.py` & `corellium-api-0.3.0/test/test_team.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_team_create.py` & `corellium-api-0.3.0/test/test_team_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_text_input.py` & `corellium-api-0.3.0/test/test_text_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_token.py` & `corellium-api-0.3.0/test/test_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_touch_curve_input.py` & `corellium-api-0.3.0/test/test_touch_curve_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_touch_input.py` & `corellium-api-0.3.0/test/test_touch_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_trial.py` & `corellium-api-0.3.0/test/test_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_trial_extension.py` & `corellium-api-0.3.0/test/test_trial_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_trial_request_metadata.py` & `corellium-api-0.3.0/test/test_trial_request_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_trial_request_options.py` & `corellium-api-0.3.0/test/test_trial_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_update_extension.py` & `corellium-api-0.3.0/test/test_update_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_user.py` & `corellium-api-0.3.0/test/test_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_user_error.py` & `corellium-api-0.3.0/test/test_user_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_v1_create_hook_parameters.py` & `corellium-api-0.3.0/test/test_v1_create_hook_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_v1_load_extension_parameters.py` & `corellium-api-0.3.0/test/test_v1_load_extension_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_v1_set_state_body.py` & `corellium-api-0.3.0/test/test_v1_set_state_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_validation_error.py` & `corellium-api-0.3.0/test/test_validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_volume_options.py` & `corellium-api-0.3.0/test/test_volume_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_vpn_definition.py` & `corellium-api-0.3.0/test/test_vpn_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_web_player_create_session_request.py` & `corellium-api-0.3.0/test/test_web_player_create_session_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.2.0/test/test_web_player_session.py` & `corellium-api-0.3.0/test/test_web_player_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.2.0-6a4b86f
+    The version of the OpenAPI document: 4.5.0-16740
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

