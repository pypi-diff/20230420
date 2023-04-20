# Comparing `tmp/orchestrator-core-1.0.1rc3.tar.gz` & `tmp/orchestrator-core-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator-core-1.0.1rc3.tar", last modified: Wed Apr 12 12:55:40 2023, max compression
+gzip compressed data, was "orchestrator-core-1.0.2rc1.tar", last modified: Thu Apr 20 12:20:29 2023, max compression
```

## Comparing `orchestrator-core-1.0.1rc3.tar` & `orchestrator-core-1.0.2rc1.tar`

### file list

```diff
@@ -1,295 +1,295 @@
--rw-r--r--   0        0        0      346 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.coveragerc
--rw-r--r--   0        0        0     2620 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0      385 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1156 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2099 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1782 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.gitignore
--rw-r--r--   0        0        0     2043 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    29641 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-04-12 12:55:35.543482 orchestrator-core-1.0.1rc3/Dockerfile
--rw-r--r--   0        0        0    11409 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/LICENSE
--rw-r--r--   0        0        0      150 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/NOTICE
--rw-r--r--   0        0        0     4813 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/README.md
--rw-r--r--   0        0        0       79 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/codecov.yml
--rw-r--r--   0        0        0       45 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0     4347 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     5641 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/index.md
--rw-r--r--   0        0        0     3897 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/js/termynal.js
--rw-r--r--   0        0        0     5605 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0      771 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     3489 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/mutmut_config.py
--rw-r--r--   0        0        0     1098 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2871 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2856 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    16207 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5211 2023-04-12 12:55:35.547483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11510 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      996 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/api/models.py
--rw-r--r--   0        0        0     7394 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      871 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      734 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2920 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/db/database.py
--rw-r--r--   0        0        0    23116 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/db/models.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16769 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2554 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2528 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3315 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62310 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2659 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/forms/validators.py
--rw-r--r--   0        0        0       39 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-04-12 12:55:35.551483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2576 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1056 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1516 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3141 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/celery.py
--rw-r--r--   0        0        0    21239 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24204 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     4802 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1706 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3431 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/settings.py
--rw-r--r--   0        0        0      731 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/targets.py
--rw-r--r--   0        0        0     9605 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     8354 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3403 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3194 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33573 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9204 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0     8839 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4689 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/pyproject.toml
--rw-r--r--   0        0        0     2385 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/setup.cfg
--rw-r--r--   0        0        0      665 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/setup.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/test/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.555483 orchestrator-core-1.0.1rc3/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     7152 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/conftest.py
--rw-r--r--   0        0        0     5786 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    19583 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    16019 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37733 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2394 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      422 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/config.py
--rw-r--r--   0        0        0    20724 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50075 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.559483 orchestrator-core-1.0.1rc3/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26441 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12022 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-04-12 12:55:35.563484 orchestrator-core-1.0.1rc3/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5411 1970-01-01 00:00:00.000000 orchestrator-core-1.0.1rc3/PKG-INFO
+-rw-r--r--   0        0        0      346 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0      385 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1156 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2099 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1782 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.gitignore
+-rw-r--r--   0        0        0     2043 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29641 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/LICENSE
+-rw-r--r--   0        0        0      150 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/NOTICE
+-rw-r--r--   0        0        0     4813 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/README.md
+-rw-r--r--   0        0        0       79 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/codecov.yml
+-rw-r--r--   0        0        0       45 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0     4347 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     5641 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0     2080 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/js/termynal.js
+-rw-r--r--   0        0        0     5605 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-04-20 12:20:17.903835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0      771 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     3489 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/mutmut_config.py
+-rw-r--r--   0        0        0     1098 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2871 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2856 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    16350 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5211 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11510 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      996 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11705 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5636 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7278 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13831 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6853 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10653 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9423 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24095 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1439 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      871 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20183 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8943 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4113 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2920 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10288 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/db/database.py
+-rw-r--r--   0        0        0    23116 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/db/models.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16855 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2554 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2528 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3315 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62310 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2659 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2977 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5434 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0       39 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40397 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-04-20 12:20:17.907835 orchestrator-core-1.0.2rc1/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2576 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1056 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3390 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1516 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    21514 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1530 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3879 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24204 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     4802 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1706 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3581 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/settings.py
+-rw-r--r--   0        0        0      731 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/targets.py
+-rw-r--r--   0        0        0     9605 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6207 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     3839 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     8354 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3403 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13148 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7231 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1323 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3194 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33580 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9204 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8335 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0     8839 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4500 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2385 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/setup.cfg
+-rw-r--r--   0        0        0      665 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/setup.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1529 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     7530 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/conftest.py
+-rw-r--r--   0        0        0     5786 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-04-20 12:20:17.911835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    20143 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    16019 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37733 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2394 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      422 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/config.py
+-rw-r--r--   0        0        0    20724 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50075 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2824 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12048 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1871 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12492 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-04-20 12:20:17.915835 orchestrator-core-1.0.2rc1/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 orchestrator-core-1.0.2rc1/PKG-INFO
```

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/README.md` & `orchestrator-core-1.0.2rc1/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/build-push-container.yml` & `orchestrator-core-1.0.2rc1/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/codeql-analysis.yml` & `orchestrator-core-1.0.2rc1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/publish-package.yml` & `orchestrator-core-1.0.2rc1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/run-linting-tests.yml` & `orchestrator-core-1.0.2rc1/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/run-unit-tests.yml` & `orchestrator-core-1.0.2rc1/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.github/workflows/scheduled-build.yml` & `orchestrator-core-1.0.2rc1/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.gitignore` & `orchestrator-core-1.0.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/.pre-commit-config.yaml` & `orchestrator-core-1.0.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/CHANGELOG.md` & `orchestrator-core-1.0.2rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/LICENSE` & `orchestrator-core-1.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/README.md` & `orchestrator-core-1.0.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/cli.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/domainmodels.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/forms.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/openapi.json` & `orchestrator-core-1.0.2rc1/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/scaling.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/tasks.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/websockets.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/application/workflow.md` & `orchestrator-core-1.0.2rc1/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/architecture/tldr.md` & `orchestrator-core-1.0.2rc1/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/contributing/guidelines.md` & `orchestrator-core-1.0.2rc1/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/contributing/testing.md` & `orchestrator-core-1.0.2rc1/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/css/termynal.css` & `orchestrator-core-1.0.2rc1/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/getting-started/base.md` & `orchestrator-core-1.0.2rc1/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/getting-started/development.md` & `orchestrator-core-1.0.2rc1/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/index.md` & `orchestrator-core-1.0.2rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/js/custom.js` & `orchestrator-core-1.0.2rc1/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/js/termynal.js` & `orchestrator-core-1.0.2rc1/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/create-user-group.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/create-user.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/database-migration.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/debian.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/docker.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/domain-models.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/explore.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/input-forms.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/macos.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/modify-user-group.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/modify-user.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/overview.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/register-workflows.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/scenario.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/start-applications.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/terminate-user-group.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/terminate-user.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/beginner/workflow-introduction.md` & `orchestrator-core-1.0.2rc1/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/docs/workshops/images/metadata_products.png` & `orchestrator-core-1.0.2rc1/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/examples/basic/basic_orchestrator.py` & `orchestrator-core-1.0.2rc1/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/mkdocs.yml` & `orchestrator-core-1.0.2rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/mutmut_config.py` & `orchestrator-core-1.0.2rc1/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.0.1rc3"
+__version__ = "1.0.2rc1"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/api.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,17 @@
 
     if process.last_status == ProcessStatus.COMPLETED:
         raise_status(HTTPStatus.CONFLICT, "Resuming a completed workflow is not possible")
 
     if process.last_status == ProcessStatus.RUNNING:
         raise_status(HTTPStatus.CONFLICT, "Resuming a running workflow is not possible")
 
+    if process.last_status == ProcessStatus.RESUMED:
+        raise_status(HTTPStatus.CONFLICT, "Resuming a resumed workflow is not possible")
+
     user_name = user.user_name if user else SYSTEM_USER
 
     broadcast_func = api_broadcast_process_data(request)
     resume_process(process, user=user_name, user_inputs=json_data, broadcast_func=broadcast_func)
 
 
 @router.put("/resume-all", response_model=ProcessResumeAllSchema)
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/error_handling.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/api/models.py` & `orchestrator-core-1.0.2rc1/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/app.py` & `orchestrator-core-1.0.2rc1/orchestrator/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from fastapi_etag.dependency import add_exception_handler
 from nwastdlib.logging import ClearStructlogContextASGIMiddleware, initialise_logging
 from opentelemetry import trace
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 from opentelemetry.instrumentation.psycopg2 import Psycopg2Instrumentor
 from opentelemetry.instrumentation.redis import RedisInstrumentor
-from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from sentry_sdk.integrations.fastapi import FastApiIntegration
 from sentry_sdk.integrations.redis import RedisIntegration
 from sentry_sdk.integrations.sqlalchemy import SqlalchemyIntegration
 from starlette.middleware.cors import CORSMiddleware
 from starlette.middleware.sessions import SessionMiddleware
 from starlette.responses import JSONResponse, Response
@@ -116,15 +115,14 @@
         def _index() -> str:
             return "Orchestrator orchestrator"
 
     def instrument_app(self) -> None:
         logger.info("Activating Opentelemetry tracing to app", app=self.title)
         trace.set_tracer_provider(tracer_provider)
         FastAPIInstrumentor.instrument_app(self)
-        RequestsInstrumentor().instrument()
         HTTPXClientInstrumentor().instrument()
         RedisInstrumentor().instrument()
         Psycopg2Instrumentor().instrument()
         SQLAlchemyInstrumentor().instrument(engine=db.engine, tracer_provider=tracer_provider)
 
     def add_sentry(
         self,
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/database.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/helpers/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/helpers/input_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/helpers/print_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/main.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/migrate_domain_models.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/migrate_workflows.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/migration_helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/cli/scheduler.py` & `orchestrator-core-1.0.2rc1/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/config/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/config/assignee.py` & `orchestrator-core-1.0.2rc1/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/db/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/db/database.py` & `orchestrator-core-1.0.2rc1/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/db/models.py` & `orchestrator-core-1.0.2rc1/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/devtools/populator.py` & `orchestrator-core-1.0.2rc1/orchestrator/devtools/populator.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,16 +250,16 @@
                     log = log.bind(func_name=func_name)
                     log.info("Calling custom function.")
                     value = getattr(self, func_name)(input_field)
                 except AttributeError:
                     log.warning("Unable to resolve custom function based on type.")
                     value = None
 
-            # If enum just pick the first
-            if value is None and "enum" in input_field:
+            # If enum just pick the first or leave empty if there are no options to select
+            if value is None and "enum" in input_field and input_field["enum"]:
                 value = input_field["enum"][0]
 
             if value is None and input_field.get("format") == "divider":
                 # Ignore divider elements
                 value = ""
 
             log.debug("Resolved input_field.", value=value)
@@ -364,15 +364,15 @@
         status = self.last_state["status"] if "status" in self.last_state else self.last_state["last_status"]
         if status == "completed":
             self.log.info("Process is complete.")
             self.done = True
             return False
         elif status == "suspended":
             return True
-        elif status == "running":
+        elif status in ('running', 'resumed'):
             return False
         elif status in ("failed", "waiting"):
             if self.retries < 1:
                 self.retries += 1
                 return True
 
             self.log.error("Cowardly quitting due to failed step.", reason=self.last_state["failed_reason"])
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/distlock/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/distlock/distlock_manager.py` & `orchestrator-core-1.0.2rc1/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/distlock/managers/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator-core-1.0.2rc1/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator-core-1.0.2rc1/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/domain/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/domain/base.py` & `orchestrator-core-1.0.2rc1/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/domain/lifecycle.py` & `orchestrator-core-1.0.2rc1/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/exception_handlers.py` & `orchestrator-core-1.0.2rc1/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/forms/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/forms/network_type_validators.py` & `orchestrator-core-1.0.2rc1/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/forms/validators.py` & `orchestrator-core-1.0.2rc1/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/alembic.ini` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/env.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/helpers.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/templates/env.py.j2` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator-core-1.0.2rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schedules/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schedules/resume_workflows.py` & `orchestrator-core-1.0.2rc1/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schedules/scheduling.py` & `orchestrator-core-1.0.2rc1/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schedules/task_vacuum.py` & `orchestrator-core-1.0.2rc1/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schedules/validate_products.py` & `orchestrator-core-1.0.2rc1/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schedules/validate_subscriptions.py` & `orchestrator-core-1.0.2rc1/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/base.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/engine_settings.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/fixed_input.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/problem_detail.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/process.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/product.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/product_block.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/resource_type.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/subscription.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/subscription_descriptions.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/schemas/workflow.py` & `orchestrator-core-1.0.2rc1/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/security.py` & `orchestrator-core-1.0.2rc1/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/celery.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/celery.py`

 * *Files 19% similar despite different names*

```diff
@@ -65,23 +65,39 @@
     pstat = load_process(process)
     workflow = pstat.workflow
 
     task_name = RESUME_TASK if workflow.target == Target.SYSTEM else RESUME_WORKFLOW
     trigger_task = get_celery_task(task_name)
     result = trigger_task.delay(pstat.pid, user_inputs, user)
 
+    _celery_set_process_status_resumed(process)
+
     # Enables "Sync celery tasks. This will let the app wait until celery completes"
     if app_settings.TESTING:
         pid = result.get()
         if not pid:
             raise RuntimeError("Celery worker has failed to resume process")
 
     return pstat.pid
 
 
+def _celery_set_process_status_resumed(process: ProcessTable) -> None:
+    """Set the process status to RESUMED to prevent re-adding to task queue.
+
+    Args:
+        process: Process from database
+    """
+    from orchestrator.db import db
+    from orchestrator.workflow import ProcessStatus
+
+    process.last_status = ProcessStatus.RESUMED
+    db.session.add(process)
+    db.session.commit()
+
+
 def _celery_validate(validation_workflow: str, json: Optional[List[State]]) -> None:
     _celery_start_process(validation_workflow, user_inputs=json)
 
 
 CELERY_EXECUTION_CONTEXT: Dict[str, Callable] = {
     "start": _celery_start_process,
     "resume": _celery_resume_process,
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/processes.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,14 +491,18 @@
             for _proc in processes:
                 try:
                     process = _get_process(_proc.pid)
                     if process.last_status == ProcessStatus.RUNNING:
                         # Process has been started by something else in the meantime
                         logger.info("Cannot resume a running process", pid=_proc.pid)
                         continue
+                    elif process.last_status == ProcessStatus.RESUMED:
+                        # Process has been resumed by something else in the meantime
+                        logger.info("Cannot resume a resumed process", pid=_proc.pid)
+                        continue
                     resume_process(process, user=user_name, broadcast_func=broadcast_func)
                 except Exception:
                     logger.exception("Failed to resume process", pid=_proc.pid)
             logger.info("Completed resuming processes")
         finally:
             distlock_manager.release_sync(lock)  # type: ignore
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/products.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/settings.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/subscriptions.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/tasks.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/services/translations.py` & `orchestrator-core-1.0.2rc1/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/settings.py` & `orchestrator-core-1.0.2rc1/orchestrator/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # limitations under the License.
 
 import secrets
 import string
 from pathlib import Path
 from typing import List, Optional
 
-from opentelemetry.exporter.jaeger.thrift import JaegerExporter
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
+from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from pydantic import BaseSettings
 
 from orchestrator.types import strEnum
 
 
@@ -64,14 +65,15 @@
     CC_NOC: int = 0
     SERVICE_NAME: str = "orchestrator-core"
     LOGGING_HOST: str = "localhost"
     LOG_LEVEL: str = "DEBUG"
     SLACK_ENGINE_SETTINGS_HOOK_ENABLED: bool = False
     SLACK_ENGINE_SETTINGS_HOOK_URL: str = ""
     TRACING_ENABLED: bool = False
+    TRACE_HOST: str = "http://localhost:4317"
     TRANSLATIONS_DIR: Optional[Path] = None
     WEBSOCKET_BROADCASTER_URL: str = "memory://"
     ENABLE_WEBSOCKETS: bool = True
     DISABLE_INSYNC_CHECK: bool = False
     DEFAULT_PRODUCT_WORKFLOWS: List[str] = ["modify_note"]
     SKIP_MODEL_FOR_MIGRATION_DB_DIFF: List[str] = []
 
@@ -85,11 +87,11 @@
     OPA_URL: str = "http://127.0.0.1:8181/v1/data/automation/authorization/allow"
 
 
 app_settings = AppSettings()
 oauth2_settings = Oauth2Settings()
 
 # Tracer settings
-tracer_provider = TracerProvider()
+tracer_provider = TracerProvider(resource=Resource.create({SERVICE_NAME: app_settings.SERVICE_NAME}))
 
-jaeger_exporter = JaegerExporter(agent_host_name=app_settings.LOGGING_HOST, udp_split_oversized_batches=True)
-tracer_provider.add_span_processor(BatchSpanProcessor(jaeger_exporter))
+otlp_exporter = OTLPSpanExporter(endpoint=app_settings.TRACE_HOST)
+tracer_provider.add_span_processor(BatchSpanProcessor(otlp_exporter))
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/targets.py` & `orchestrator-core-1.0.2rc1/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/types.py` & `orchestrator-core-1.0.2rc1/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/crypt.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/datetime.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/docs.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/errors.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/functional.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/json.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/redis.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/show_process.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/speed.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/state.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/strings.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/utils/vlans.py` & `orchestrator-core-1.0.2rc1/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/version.py` & `orchestrator-core-1.0.2rc1/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/websocket/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator-core-1.0.2rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator-core-1.0.2rc1/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/websocket/websocket_manager.py` & `orchestrator-core-1.0.2rc1/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflow.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
                     return Waiting(ex)
 
         return make_step_function(wrapper, name)
 
     return decorator
 
 
-def inputstep(name: str, assignee: Optional[Assignee] = None) -> Callable[[InputStepFunc], Step]:
+def inputstep(name: str, assignee: Assignee) -> Callable[[InputStepFunc], Step]:
     """Add user input step to workflow.
 
     IMPORTANT: In contrast to other workflow steps, the `@inputstep` wrapped function will not run in the
     workflow engine! This means that it should never do any changes in the database and external systems!
 
     Example::
 
@@ -409,14 +409,15 @@
     SUSPENDED = "suspended"
     WAITING = "waiting"
     ABORTED = "aborted"
     FAILED = "failed"
     API_UNAVAILABLE = "api_unavailable"
     INCONSISTENT_DATA = "inconsistent_data"
     COMPLETED = "completed"
+    RESUMED = "resumed"
 
 
 class StepStatus(strEnum):
     SUCCESS = "success"
     SKIPPED = "skipped"
     SUSPEND = "suspend"
     WAITING = "waiting"
```

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/modify_note.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/removed_workflow.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/steps.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/__init__.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/tasks/validate_products.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/translations/en-GB.json` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/orchestrator/workflows/utils.py` & `orchestrator-core-1.0.2rc1/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/pyproject.toml` & `orchestrator-core-1.0.2rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -41,24 +41,21 @@
     "click==8.0.3",
     "deepmerge==0.1.0",
     "fastapi~=0.91.0",
     "fastapi-etag==0.4.0",
     "more-itertools~=9.0.0",
     "itsdangerous==2.1.2",
     "Jinja2==3.1.2",
-    "opentelemetry-api==1.9.1",
-    "opentelemetry-exporter-jaeger==1.9.1",
-    "opentelemetry-instrumentation-httpx==0.28b1",
-    "opentelemetry-instrumentation-fastapi==0.28b1",
-    "opentelemetry-instrumentation-psycopg2==0.28b1",
-    "opentelemetry-instrumentation-redis==0.28b1",
-    "opentelemetry-instrumentation-requests==0.28b1",
-    "opentelemetry-instrumentation-sqlalchemy==0.28b1",
-    "opentelemetry-instrumentation-wsgi==0.28b1",
-    "opentelemetry-sdk==1.9.1",
+    "opentelemetry-distro",
+    "opentelemetry-exporter-otlp",
+    "opentelemetry-instrumentation-httpx",
+    "opentelemetry-instrumentation-fastapi",
+    "opentelemetry-instrumentation-psycopg2",
+    "opentelemetry-instrumentation-redis",
+    "opentelemetry-instrumentation-sqlalchemy",
     "orjson==3.8.0",
     "psycopg2-binary==2.9.5",
     "pydantic[email]==1.10.2",
     "python-dateutil==2.8.2",
     "python-rapidjson==1.9",
     "pytz==2022.7.1",
     "redis~=4.4.2",
```

### Comparing `orchestrator-core-1.0.1rc3/setup.cfg` & `orchestrator-core-1.0.2rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/setup.py` & `orchestrator-core-1.0.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/conftest.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/acceptance_tests/test_test_product.py` & `orchestrator-core-1.0.2rc1/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/conftest.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,17 +102,19 @@
         return pid
 
     return [
         mock_process(generic_subscription_1, "completed", first_datetime),
         mock_process(generic_subscription_1, "suspended", first_datetime + timedelta(days=1), assignee="NOC"),
         mock_process(generic_subscription_2, "completed", first_datetime + timedelta(days=2)),
         mock_process(generic_subscription_2, "failed", first_datetime + timedelta(days=3)),
+        mock_process(generic_subscription_1, "resumed", first_datetime + timedelta(days=5)),
         mock_process(generic_subscription_1, "suspended", first_datetime + timedelta(days=1), is_task=True),
         mock_process(generic_subscription_2, "completed", first_datetime + timedelta(days=2), is_task=True),
         mock_process(None, "running", first_datetime + timedelta(days=4), is_task=True),
+        mock_process(None, "resumed", first_datetime + timedelta(days=5), is_task=True),
     ]
 
 
 @pytest.fixture
 def mocked_processes_resumeall(test_workflow, generic_subscription_1, generic_subscription_2):
     first_datetime = datetime(2020, 1, 14, 9, 30, tzinfo=pytz.utc)
 
@@ -161,11 +163,13 @@
         mock_process(generic_subscription_1, "api_unavailable", first_datetime, is_task=True),
         mock_process(
             generic_subscription_1, "suspended", first_datetime + timedelta(days=1), assignee="NOC", is_task=True
         ),
         mock_process(generic_subscription_2, "completed", first_datetime + timedelta(days=2), is_task=True),
         mock_process(generic_subscription_2, "running", first_datetime + timedelta(days=2), is_task=True),
         mock_process(generic_subscription_2, "failed", first_datetime + timedelta(days=3), is_task=True),
+        mock_process(generic_subscription_1, "resumed", first_datetime + timedelta(days=5), is_task=True),
         mock_process(generic_subscription_1, "inconsistent_data", first_datetime + timedelta(days=1), is_task=True),
         mock_process(generic_subscription_2, "failed", first_datetime + timedelta(days=2), is_task=False),
         mock_process(None, "running", first_datetime + timedelta(days=4), is_task=True),
+        mock_process(None, "resumed", first_datetime + timedelta(days=5), is_task=True),
     ]
```

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_caching.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_health.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_helpers.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_models.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_processes.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,45 +361,59 @@
     process.failed_reason = ""
     db.session.commit()
 
     response = test_client.put(f"/api/processes/{started_process}/resume", json=[{}])
     assert 409 == response.status_code
 
 
+def test_try_resume_resumed_workflow(test_client, started_process):
+    process = ProcessTable.query.get(started_process)
+    # setup DB so it looks like this workflow has already been resumed
+    process.last_status = ProcessStatus.RESUMED
+    process.failed_reason = ""
+    db.session.add(process)
+    db.session.commit()
+
+    response = test_client.put(f"/api/processes/{started_process}/resume", json=[{}])
+    assert 409 == response.status_code
+
+
 def test_processes_filterable(test_client, mocked_processes, generic_subscription_2, generic_subscription_1):
     response = test_client.get("/api/processes/")
     assert HTTPStatus.OK == response.status_code
     processes = response.json()
 
-    assert 7 == len(processes)
+    assert 9 == len(processes)
     assert "workflow_for_testing_processes_py", processes[0]["workflow"]
 
     response = test_client.get("/api/processes?filter=status,completed")
     assert 3 == len(response.json())
     response = test_client.get("/api/processes?filter=status,suspended")
     assert 2 == len(response.json())
+    response = test_client.get("/api/processes?filter=status,resumed")
+    assert 2 == len(response.json())
 
     product_name = SubscriptionTable.query.get(generic_subscription_1).product.name
     response = test_client.get(f"/api/processes?filter=product,{product_name}")
-    assert 3 == len(response.json())
+    assert 4 == len(response.json())
     response = test_client.get("/api/processes?sort=assignee,asc")
     assert response.json()[0]["assignee"] == "NOC"
     response = test_client.get("/api/processes?sort=started&filter=istask,y")
-    assert 3 == len(response.json())
+    assert 4 == len(response.json())
     response = test_client.get(f"/api/processes?filter=istask,y,organisation,{CUSTOMER_ID}")
     assert 2 == len(response.json())
 
 
 def test_processes_filterable_response_model(
     test_client, mocked_processes, generic_subscription_2, generic_subscription_1
 ):
     response = test_client.get("/api/processes/?sort=started,asc")
     assert HTTPStatus.OK == response.status_code
     processes = response.json()
-    assert len(processes) == 7
+    assert len(processes) == 9
     process = processes[0]
 
     assert len(process["subscriptions"]) == 1
 
     # Check if the other fields are filled with correct data
     del process["pid"]  # skip pid as it's dynamic
     del process["subscriptions"]
@@ -419,15 +433,15 @@
 
 def test_processes_filterable_response_model_contains_product_info(
     test_client, mocked_processes, generic_subscription_2, generic_subscription_1
 ):
     response = test_client.get("/api/processes/?sort=started,asc")
     assert HTTPStatus.OK == response.status_code
     processes = response.json()
-    assert len(processes) == 7
+    assert len(processes) == 9
     process = processes[0]
 
     assert len(process["subscriptions"]) == 1
     assert process["subscriptions"][0]["product"]["tag"] == "GEN1"
     assert process["subscriptions"][0]["product"]["name"] == "Product 1"
```

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_processes_ws.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_product_blocks.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_products.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_resource_types.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_settings.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_subscriptions.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/api/test_workflows.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/conftest.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/domain/test_base.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/domain/test_base_with_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/__init__.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/forms/shared.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/forms/test_generic_validators.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/forms/test_network_validators.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/forms/test_post_process.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/schedules/test_scheduling.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/services/test_processes.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/services/test_processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -621,31 +621,38 @@
         assert f"Failed to write failure step to process: process with PID {pid} not found" in str(e.value)
 
 
 @mock.patch("orchestrator.services.processes._get_process")
 @mock.patch("orchestrator.services.processes.resume_process")
 def test_async_resume_processes(mock_resume_process, mock_get_process, caplog):
     """Test that _async_resume_process() rejects running processes and handles failures."""
-    processes = [mock.Mock(spec=ProcessTable()), mock.Mock(spec=ProcessTable()), mock.Mock(spec=ProcessTable())]
+    processes = [
+        mock.Mock(spec=ProcessTable()),
+        mock.Mock(spec=ProcessTable()),
+        mock.Mock(spec=ProcessTable()),
+        mock.Mock(spec=ProcessTable()),
+    ]
     processes[0].pid, processes[0].last_status = 123, ProcessStatus.RUNNING
     processes[1].pid, processes[1].last_status = 124, ProcessStatus.FAILED
     processes[2].pid, processes[2].last_status = 125, ProcessStatus.API_UNAVAILABLE
+    processes[3].pid, processes[3].last_status = 126, ProcessStatus.RESUMED
 
-    # get_process() should be called 3 times
+    # get_process() should be called 4 times
     mock_get_process.side_effect = processes
 
-    # resume_process() should be called 2 times for the non-running processes; let 1 call fail
+    # resume_process() should be called 2 times for the non-running / non-resumed processes; let 1 call fail
     mock_resume_process.side_effect = [None, ValueError("This workflow cannot be resumed")]
 
     # Don't set app_settings.TESTING=False because we want to await the result
     asyncio.run(_async_resume_processes(processes, "testusername"))
 
-    assert len(mock_get_process.mock_calls) == 3
+    assert len(mock_get_process.mock_calls) == 4
     assert len(mock_resume_process.mock_calls) == 2
     assert "Cannot resume a running process" in caplog.text  # pid 123 should not be resumed
+    assert "Cannot resume a resumed process" in caplog.text  # pid 126 should not be resumed
     assert "Failed to resume process" in caplog.text  # pid 125 should fail
     assert "Completed resuming processes" in caplog.text
 
 
 def test_db_log_process_ex():
     pid = uuid4()
```

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/services/test_products.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/services/test_subscriptions.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/services/test_translations.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/test_db.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/test_workflow.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/test_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         log.append((step.name, state))
         return state
 
     return _store
 
 
 def test_failing_inputstep_with_form_state_params() -> None:
-    @inputstep("Modify")
+    @inputstep("Modify", assignee=Assignee.SYSTEM)
     def modify(subscription_id: UUIDstr) -> NoReturn:
         raise Exception("Something went wrong")
 
     class Form(FormPage):
         subscription_id: UUID
 
     @workflow("Workflow", initial_input_form=const(Form))
```

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_errors.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_functional.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_json.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_speed.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_state.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/utils/test_vlans.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/__init__.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/test/unit_tests/workflows/test_modify_note.py` & `orchestrator-core-1.0.2rc1/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.1rc3/PKG-INFO` & `orchestrator-core-1.0.2rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.0.1rc3
+Version: 1.0.2rc1
 Summary: Open source orchestration software for NREN's
 Requires-Python: >3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -31,24 +31,21 @@
 Requires-Dist: click==8.0.3
 Requires-Dist: deepmerge==0.1.0
 Requires-Dist: fastapi~=0.91.0
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=9.0.0
 Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: Jinja2==3.1.2
-Requires-Dist: opentelemetry-api==1.9.1
-Requires-Dist: opentelemetry-exporter-jaeger==1.9.1
-Requires-Dist: opentelemetry-instrumentation-httpx==0.28b1
-Requires-Dist: opentelemetry-instrumentation-fastapi==0.28b1
-Requires-Dist: opentelemetry-instrumentation-psycopg2==0.28b1
-Requires-Dist: opentelemetry-instrumentation-redis==0.28b1
-Requires-Dist: opentelemetry-instrumentation-requests==0.28b1
-Requires-Dist: opentelemetry-instrumentation-sqlalchemy==0.28b1
-Requires-Dist: opentelemetry-instrumentation-wsgi==0.28b1
-Requires-Dist: opentelemetry-sdk==1.9.1
+Requires-Dist: opentelemetry-distro
+Requires-Dist: opentelemetry-exporter-otlp
+Requires-Dist: opentelemetry-instrumentation-httpx
+Requires-Dist: opentelemetry-instrumentation-fastapi
+Requires-Dist: opentelemetry-instrumentation-psycopg2
+Requires-Dist: opentelemetry-instrumentation-redis
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: orjson==3.8.0
 Requires-Dist: psycopg2-binary==2.9.5
 Requires-Dist: pydantic[email]==1.10.2
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson==1.9
 Requires-Dist: pytz==2022.7.1
 Requires-Dist: redis~=4.4.2
```

