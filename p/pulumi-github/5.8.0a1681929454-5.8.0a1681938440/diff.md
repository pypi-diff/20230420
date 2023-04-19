# Comparing `tmp/pulumi_github-5.8.0a1681929454.tar.gz` & `tmp/pulumi_github-5.8.0a1681938440.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_github-5.8.0a1681929454.tar", last modified: Wed Apr 19 19:04:18 2023, max compression
+gzip compressed data, was "pulumi_github-5.8.0a1681938440.tar", last modified: Wed Apr 19 21:17:44 2023, max compression
```

## Comparing `pulumi_github-5.8.0a1681929454.tar` & `pulumi_github-5.8.0a1681938440.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:18.292962 pulumi_github-5.8.0a1681929454/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-19 19:04:18.288962 pulumi_github-5.8.0a1681929454/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:18.288962 pulumi_github-5.8.0a1681929454/pulumi_github/
--rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19178 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_environment_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_repository_access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_repository_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_runner_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/actions_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/app_installation_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/app_installation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/branch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    44058 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/branch_protection_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:18.288962 pulumi_github-5.8.0a1681929454/pulumi_github/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/dependabot_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/dependabot_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/dependabot_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/emu_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14476 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/enterprise_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_environment_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_external_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_github_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_ip_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_team_sync_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_pull_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/issue_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/organization_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/organization_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/organization_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    79808 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/organization_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/organization_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   102405 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/project_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/project_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/release.py
--rw-r--r--   0 runner    (1001) docker     (123)   107291 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_autolink_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_collaborator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    28682 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/repository_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/team_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/team_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/team_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/team_sync_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/user_invitation_accepter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:18.288962 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:04:18.292962 pulumi_github-5.8.0a1681929454/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-19 19:04:18.000000 pulumi_github-5.8.0a1681929454/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:44.597778 pulumi_github-5.8.0a1681938440/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-19 21:17:44.597778 pulumi_github-5.8.0a1681938440/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:44.593778 pulumi_github-5.8.0a1681938440/pulumi_github/
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19178 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_environment_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_repository_access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_repository_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_runner_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/actions_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/app_installation_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/app_installation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/branch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44058 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/branch_protection_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:44.597778 pulumi_github-5.8.0a1681938440/pulumi_github/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/dependabot_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/dependabot_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/dependabot_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/emu_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14476 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/enterprise_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_environment_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_external_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_github_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_issue_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_ip_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_team_sync_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_pull_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/issue_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/organization_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/organization_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/organization_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79808 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/organization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/organization_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103800 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/project_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/project_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107291 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_autolink_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28682 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/repository_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/team_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/team_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/team_sync_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/user_invitation_accepter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:44.597778 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:17:44.597778 pulumi_github-5.8.0a1681938440/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-19 21:17:44.000000 pulumi_github-5.8.0a1681938440/setup.py
```

### Comparing `pulumi_github-5.8.0a1681929454/PKG-INFO` & `pulumi_github-5.8.0a1681938440/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_github
-Version: 5.8.0a1681929454
+Version: 5.8.0a1681938440
 Summary: A Pulumi package for creating and managing github cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi github
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Build Status](https://travis-ci.com/pulumi/pulumi-github.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-ci.com/pulumi/pulumi-github)
 
 # GitHub provider
 
 The GitHub resource provider for Pulumi lets you use GitHub resources in your infrastructure programs.
```

### Comparing `pulumi_github-5.8.0a1681929454/README.md` & `pulumi_github-5.8.0a1681938440/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/__init__.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from .get_dependabot_organization_secrets import *
 from .get_dependabot_public_key import *
 from .get_dependabot_secrets import *
 from .get_enterprise import *
 from .get_external_groups import *
 from .get_github_app import *
 from .get_ip_ranges import *
+from .get_issue_labels import *
 from .get_membership import *
 from .get_organization import *
 from .get_organization_ip_allow_list import *
 from .get_organization_team_sync_groups import *
 from .get_organization_teams import *
 from .get_organization_webhooks import *
 from .get_ref import *
```

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/_inputs.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/_utilities.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_environment_secret.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_environment_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_environment_variable.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_permissions.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_secret.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_secret_repositories.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_secret_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_organization_variable.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_organization_variable.py`

 * *Files 11% similar despite different names*

```diff
@@ -198,14 +198,38 @@
                  variable_name: Optional[pulumi.Input[str]] = None,
                  visibility: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub organization.
         You must have write access to a repository to use this resource.
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_github as github
+
+        example_variable = github.ActionsOrganizationVariable("exampleVariable",
+            value="example_variable_value",
+            variable_name="example_variable_name",
+            visibility="private")
+        ```
+
+        ```python
+        import pulumi
+        import pulumi_github as github
+
+        repo = github.get_repository(full_name="my-org/repo")
+        example_variable = github.ActionsOrganizationVariable("exampleVariable",
+            variable_name="example_variable_name",
+            visibility="selected",
+            value="example_variable_value",
+            selected_repository_ids=[repo.repo_id])
+        ```
+
         ## Import
 
         This resource can be imported using an ID made up of the variable name
 
         ```sh
          $ pulumi import github:index/actionsOrganizationVariable:ActionsOrganizationVariable test_variable test_variable_name
         ```
@@ -224,14 +248,38 @@
                  resource_name: str,
                  args: ActionsOrganizationVariableArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub organization.
         You must have write access to a repository to use this resource.
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_github as github
+
+        example_variable = github.ActionsOrganizationVariable("exampleVariable",
+            value="example_variable_value",
+            variable_name="example_variable_name",
+            visibility="private")
+        ```
+
+        ```python
+        import pulumi
+        import pulumi_github as github
+
+        repo = github.get_repository(full_name="my-org/repo")
+        example_variable = github.ActionsOrganizationVariable("exampleVariable",
+            variable_name="example_variable_name",
+            visibility="selected",
+            value="example_variable_value",
+            selected_repository_ids=[repo.repo_id])
+        ```
+
         ## Import
 
         This resource can be imported using an ID made up of the variable name
 
         ```sh
          $ pulumi import github:index/actionsOrganizationVariable:ActionsOrganizationVariable test_variable test_variable_name
         ```
```

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_repository_access_level.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_repository_access_level.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_repository_permissions.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_repository_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_runner_group.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_runner_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_secret.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/actions_variable.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/actions_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/app_installation_repositories.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/app_installation_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/app_installation_repository.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/app_installation_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/branch.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/branch_default.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/branch_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/branch_protection.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/branch_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/branch_protection_v3.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/branch_protection_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/config/outputs.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/config/vars.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/dependabot_organization_secret.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/dependabot_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/dependabot_organization_secret_repositories.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/dependabot_organization_secret_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/dependabot_secret.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/dependabot_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/emu_group_mapping.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/emu_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/enterprise_organization.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/enterprise_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_environment_secrets.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_environment_variables.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_environment_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_public_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_registration_token.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_registration_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_secrets.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_organization_variables.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_organization_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_public_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_registration_token.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_registration_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_secrets.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_actions_variables.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_actions_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_branch.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_collaborators.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_collaborators.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_organization_public_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_organization_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_organization_secrets.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_organization_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_public_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_dependabot_secrets.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_dependabot_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_enterprise.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_external_groups.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_external_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_github_app.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_github_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_ip_ranges.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_membership.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_organization.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_ip_allow_list.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_ip_allow_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_team_sync_groups.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_team_sync_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_teams.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_organization_webhooks.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_organization_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_ref.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_ref.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,24 @@
 ]
 
 @pulumi.output_type
 class GetRefResult:
     """
     A collection of values returned by getRef.
     """
-    def __init__(__self__, etag=None, id=None, ref=None, repository=None, sha=None):
+    def __init__(__self__, etag=None, id=None, owner=None, ref=None, repository=None, sha=None):
         if etag and not isinstance(etag, str):
             raise TypeError("Expected argument 'etag' to be a str")
         pulumi.set(__self__, "etag", etag)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if owner and not isinstance(owner, str):
+            raise TypeError("Expected argument 'owner' to be a str")
+        pulumi.set(__self__, "owner", owner)
         if ref and not isinstance(ref, str):
             raise TypeError("Expected argument 'ref' to be a str")
         pulumi.set(__self__, "ref", ref)
         if repository and not isinstance(repository, str):
             raise TypeError("Expected argument 'repository' to be a str")
         pulumi.set(__self__, "repository", repository)
         if sha and not isinstance(sha, str):
@@ -52,14 +55,19 @@
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def owner(self) -> Optional[str]:
+        return pulumi.get(self, "owner")
+
+    @property
+    @pulumi.getter
     def ref(self) -> str:
         return pulumi.get(self, "ref")
 
     @property
     @pulumi.getter
     def repository(self) -> str:
         return pulumi.get(self, "repository")
@@ -77,68 +85,77 @@
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetRefResult(
             etag=self.etag,
             id=self.id,
+            owner=self.owner,
             ref=self.ref,
             repository=self.repository,
             sha=self.sha)
 
 
-def get_ref(ref: Optional[str] = None,
+def get_ref(owner: Optional[str] = None,
+            ref: Optional[str] = None,
             repository: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRefResult:
     """
     Use this data source to retrieve information about a repository ref.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_github as github
 
-    development = github.get_ref(ref="heads/development",
+    development = github.get_ref(owner="example",
+        ref="heads/development",
         repository="example")
     ```
 
 
+    :param str owner: Owner of the repository.
     :param str ref: The repository ref to look up. Must be formatted `heads/<ref>` for branches, and `tags/<ref>` for tags.
     :param str repository: The GitHub repository name.
     """
     __args__ = dict()
+    __args__['owner'] = owner
     __args__['ref'] = ref
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getRef:getRef', __args__, opts=opts, typ=GetRefResult).value
 
     return AwaitableGetRefResult(
         etag=__ret__.etag,
         id=__ret__.id,
+        owner=__ret__.owner,
         ref=__ret__.ref,
         repository=__ret__.repository,
         sha=__ret__.sha)
 
 
 @_utilities.lift_output_func(get_ref)
-def get_ref_output(ref: Optional[pulumi.Input[str]] = None,
+def get_ref_output(owner: Optional[pulumi.Input[Optional[str]]] = None,
+                   ref: Optional[pulumi.Input[str]] = None,
                    repository: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRefResult]:
     """
     Use this data source to retrieve information about a repository ref.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_github as github
 
-    development = github.get_ref(ref="heads/development",
+    development = github.get_ref(owner="example",
+        ref="heads/development",
         repository="example")
     ```
 
 
+    :param str owner: Owner of the repository.
     :param str ref: The repository ref to look up. Must be formatted `heads/<ref>` for branches, and `tags/<ref>` for tags.
     :param str repository: The GitHub repository name.
     """
     ...
```

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_release.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_release.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repositories.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetRepositoryResult:
     """
     A collection of values returned by getRepository.
     """
-    def __init__(__self__, allow_auto_merge=None, allow_merge_commit=None, allow_rebase_merge=None, allow_squash_merge=None, archived=None, default_branch=None, description=None, full_name=None, git_clone_url=None, has_discussions=None, has_downloads=None, has_issues=None, has_projects=None, has_wiki=None, homepage_url=None, html_url=None, http_clone_url=None, id=None, is_template=None, merge_commit_message=None, merge_commit_title=None, name=None, node_id=None, pages=None, private=None, repo_id=None, squash_merge_commit_message=None, squash_merge_commit_title=None, ssh_clone_url=None, svn_url=None, template=None, topics=None, visibility=None):
+    def __init__(__self__, allow_auto_merge=None, allow_merge_commit=None, allow_rebase_merge=None, allow_squash_merge=None, archived=None, default_branch=None, description=None, fork=None, full_name=None, git_clone_url=None, has_discussions=None, has_downloads=None, has_issues=None, has_projects=None, has_wiki=None, homepage_url=None, html_url=None, http_clone_url=None, id=None, is_template=None, merge_commit_message=None, merge_commit_title=None, name=None, node_id=None, pages=None, private=None, repo_id=None, squash_merge_commit_message=None, squash_merge_commit_title=None, ssh_clone_url=None, svn_url=None, template=None, topics=None, visibility=None):
         if allow_auto_merge and not isinstance(allow_auto_merge, bool):
             raise TypeError("Expected argument 'allow_auto_merge' to be a bool")
         pulumi.set(__self__, "allow_auto_merge", allow_auto_merge)
         if allow_merge_commit and not isinstance(allow_merge_commit, bool):
             raise TypeError("Expected argument 'allow_merge_commit' to be a bool")
         pulumi.set(__self__, "allow_merge_commit", allow_merge_commit)
         if allow_rebase_merge and not isinstance(allow_rebase_merge, bool):
@@ -40,14 +40,17 @@
         pulumi.set(__self__, "archived", archived)
         if default_branch and not isinstance(default_branch, str):
             raise TypeError("Expected argument 'default_branch' to be a str")
         pulumi.set(__self__, "default_branch", default_branch)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
+        if fork and not isinstance(fork, bool):
+            raise TypeError("Expected argument 'fork' to be a bool")
+        pulumi.set(__self__, "fork", fork)
         if full_name and not isinstance(full_name, str):
             raise TypeError("Expected argument 'full_name' to be a str")
         pulumi.set(__self__, "full_name", full_name)
         if git_clone_url and not isinstance(git_clone_url, str):
             raise TypeError("Expected argument 'git_clone_url' to be a str")
         pulumi.set(__self__, "git_clone_url", git_clone_url)
         if has_discussions and not isinstance(has_discussions, bool):
@@ -176,14 +179,22 @@
     def description(self) -> Optional[str]:
         """
         A description of the repository.
         """
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter
+    def fork(self) -> bool:
+        """
+        Whether the repository is a fork.
+        """
+        return pulumi.get(self, "fork")
+
+    @property
     @pulumi.getter(name="fullName")
     def full_name(self) -> str:
         return pulumi.get(self, "full_name")
 
     @property
     @pulumi.getter(name="gitCloneUrl")
     def git_clone_url(self) -> str:
@@ -391,14 +402,15 @@
             allow_auto_merge=self.allow_auto_merge,
             allow_merge_commit=self.allow_merge_commit,
             allow_rebase_merge=self.allow_rebase_merge,
             allow_squash_merge=self.allow_squash_merge,
             archived=self.archived,
             default_branch=self.default_branch,
             description=self.description,
+            fork=self.fork,
             full_name=self.full_name,
             git_clone_url=self.git_clone_url,
             has_discussions=self.has_discussions,
             has_downloads=self.has_downloads,
             has_issues=self.has_issues,
             has_projects=self.has_projects,
             has_wiki=self.has_wiki,
@@ -458,14 +470,15 @@
         allow_auto_merge=__ret__.allow_auto_merge,
         allow_merge_commit=__ret__.allow_merge_commit,
         allow_rebase_merge=__ret__.allow_rebase_merge,
         allow_squash_merge=__ret__.allow_squash_merge,
         archived=__ret__.archived,
         default_branch=__ret__.default_branch,
         description=__ret__.description,
+        fork=__ret__.fork,
         full_name=__ret__.full_name,
         git_clone_url=__ret__.git_clone_url,
         has_discussions=__ret__.has_discussions,
         has_downloads=__ret__.has_downloads,
         has_issues=__ret__.has_issues,
         has_projects=__ret__.has_projects,
         has_wiki=__ret__.has_wiki,
```

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_branches.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_deploy_keys.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_file.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_milestone.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_pull_request.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_pull_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_pull_requests.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_teams.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_repository_webhooks.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_repository_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_ssh_keys.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_team.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_tree.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_user.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/get_users.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/issue.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/issue_label.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/issue_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/membership.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/organization_block.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/organization_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/organization_project.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/organization_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/organization_security_manager.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/organization_security_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/organization_settings.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/organization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/organization_webhook.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/organization_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/outputs.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     'GetActionsOrganizationVariablesVariableResult',
     'GetActionsSecretsSecretResult',
     'GetActionsVariablesVariableResult',
     'GetCollaboratorsCollaboratorResult',
     'GetDependabotOrganizationSecretsSecretResult',
     'GetDependabotSecretsSecretResult',
     'GetExternalGroupsExternalGroupResult',
+    'GetIssueLabelsLabelResult',
     'GetOrganizationIpAllowListIpAllowListResult',
     'GetOrganizationTeamSyncGroupsGroupResult',
     'GetOrganizationTeamsTeamResult',
     'GetOrganizationWebhooksWebhookResult',
     'GetReleaseAssetResult',
     'GetRepositoryBranchesBranchResult',
     'GetRepositoryDeployKeysKeyResult',
@@ -1996,14 +1997,65 @@
         """
         the date the group was last updated.
         """
         return pulumi.get(self, "updated_at")
 
 
 @pulumi.output_type
+class GetIssueLabelsLabelResult(dict):
+    def __init__(__self__, *,
+                 color: str,
+                 description: str,
+                 name: str,
+                 url: str):
+        """
+        :param str color: The hexadecimal color code for the label, without the leading #.
+        :param str description: A short description of the label.
+        :param str name: The name of the label.
+        :param str url: The URL of the label.
+        """
+        pulumi.set(__self__, "color", color)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter
+    def color(self) -> str:
+        """
+        The hexadecimal color code for the label, without the leading #.
+        """
+        return pulumi.get(self, "color")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        A short description of the label.
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the label.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        The URL of the label.
+        """
+        return pulumi.get(self, "url")
+
+
+@pulumi.output_type
 class GetOrganizationIpAllowListIpAllowListResult(dict):
     def __init__(__self__, *,
                  allow_list_value: str,
                  created_at: str,
                  id: str,
                  is_active: bool,
                  name: str,
```

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/project_card.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/project_card.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/project_column.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/project_column.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/provider.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/release.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/release.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_autolink_reference.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_autolink_reference.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_collaborator.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_collaborator.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_collaborators.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_collaborators.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_deploy_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_deploy_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_environment.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_file.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_milestone.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_project.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_pull_request.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_pull_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_tag_protection.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/repository_webhook.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/repository_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/team.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/team_members.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/team_membership.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/team_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/team_repository.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/team_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/team_settings.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/team_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/team_sync_group_mapping.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/team_sync_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/user_gpg_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/user_invitation_accepter.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/user_invitation_accepter.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github/user_ssh_key.py` & `pulumi_github-5.8.0a1681938440/pulumi_github/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/PKG-INFO` & `pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-github
-Version: 5.8.0a1681929454
+Version: 5.8.0a1681938440
 Summary: A Pulumi package for creating and managing github cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi github
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Build Status](https://travis-ci.com/pulumi/pulumi-github.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-ci.com/pulumi/pulumi-github)
 
 # GitHub provider
 
 The GitHub resource provider for Pulumi lets you use GitHub resources in your infrastructure programs.
```

### Comparing `pulumi_github-5.8.0a1681929454/pulumi_github.egg-info/SOURCES.txt` & `pulumi_github-5.8.0a1681938440/pulumi_github.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 pulumi_github/get_dependabot_organization_secrets.py
 pulumi_github/get_dependabot_public_key.py
 pulumi_github/get_dependabot_secrets.py
 pulumi_github/get_enterprise.py
 pulumi_github/get_external_groups.py
 pulumi_github/get_github_app.py
 pulumi_github/get_ip_ranges.py
+pulumi_github/get_issue_labels.py
 pulumi_github/get_membership.py
 pulumi_github/get_organization.py
 pulumi_github/get_organization_ip_allow_list.py
 pulumi_github/get_organization_team_sync_groups.py
 pulumi_github/get_organization_teams.py
 pulumi_github/get_organization_webhooks.py
 pulumi_github/get_ref.py
```

### Comparing `pulumi_github-5.8.0a1681929454/setup.py` & `pulumi_github-5.8.0a1681938440/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.8.0a1681929454"
-PLUGIN_VERSION = "5.8.0-alpha.1681929454+1fce4957"
+VERSION = "5.8.0a1681938440"
+PLUGIN_VERSION = "5.8.0-alpha.1681938440+ddf6c005"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'github', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "github Pulumi Package - Development Version"
 
 
 setup(name='pulumi_github',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing github cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

