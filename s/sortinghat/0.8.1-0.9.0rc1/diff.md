# Comparing `tmp/sortinghat-0.8.1.tar.gz` & `tmp/sortinghat-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat-0.8.1.tar", max compression
+gzip compressed data, was "sortinghat-0.9.0rc1.tar", max compression
```

## Comparing `sortinghat-0.8.1.tar` & `sortinghat-0.9.0rc1.tar`

### file list

```diff
@@ -1,110 +1,130 @@
--rw-r--r--   0        0        0      326 2023-02-03 08:31:08.689913 sortinghat-0.8.1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-02-03 08:31:08.689913 sortinghat-0.8.1/LICENSE
--rw-r--r--   0        0        0    11752 2023-02-03 08:31:08.689913 sortinghat-0.8.1/NEWS
--rw-r--r--   0        0        0     6989 2023-02-03 08:31:08.689913 sortinghat-0.8.1/README.md
--rw-r--r--   0        0        0     2008 2023-02-03 08:31:08.689913 sortinghat-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/_version.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/app/__init__.py
--rw-r--r--   0        0        0     1250 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/app/schema.py
--rw-r--r--   0        0        0      518 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/app/urls.py
--rw-r--r--   0        0        0      196 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/app/wsgi.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.689913 sortinghat-0.8.1/sortinghat/cli/__init__.py
--rw-r--r--   0        0        0      977 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/client/__init__.py
--rw-r--r--   0        0        0     5577 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/client/client.py
--rw-r--r--   0        0        0    43408 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/client/schema.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/__init__.py
--rw-r--r--   0        0        0     3072 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/add.py
--rw-r--r--   0        0        0     6145 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/config.py
--rw-r--r--   0        0        0     3219 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/countries.py
--rw-r--r--   0        0        0     3462 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/enroll.py
--rw-r--r--   0        0        0     2860 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/lock.py
--rw-r--r--   0        0        0     2342 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/merge.py
--rw-r--r--   0        0        0     2352 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/mv.py
--rw-r--r--   0        0        0     7466 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/orgs.py
--rw-r--r--   0        0        0     2934 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/profile.py
--rw-r--r--   0        0        0     1992 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/rm.py
--rw-r--r--   0        0        0     2909 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/show.py
--rw-r--r--   0        0        0     2365 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/split.py
--rw-r--r--   0        0        0     3364 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/cmds/withdraw.py
--rwxr-xr-x   0        0        0     2857 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/sortinghat.py
--rw-r--r--   0        0        0       43 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/add.tmpl
--rw-r--r--   0        0        0       23 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/config.tmpl
--rw-r--r--   0        0        0       83 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/countries.tmpl
--rw-r--r--   0        0        0       54 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/lock.tmpl
--rw-r--r--   0        0        0      169 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/mv.tmpl
--rw-r--r--   0        0        0      208 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/organizations.tmpl
--rw-r--r--   0        0        0      375 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/profile.tmpl
--rw-r--r--   0        0        0      106 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/rm.tmpl
--rw-r--r--   0        0        0     1016 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/show.tmpl
--rw-r--r--   0        0        0       69 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/templates/split.tmpl
--rw-r--r--   0        0        0     4856 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/cli/utils.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/config/__init__.py
--rw-r--r--   0        0        0     7973 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/config/settings.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/__init__.py
--rw-r--r--   0        0        0     1544 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/admin.py
--rw-r--r--   0        0        0    47885 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/api.py
--rw-r--r--   0        0        0      861 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/apps.py
--rw-r--r--   0        0        0     5169 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/aux.py
--rw-r--r--   0        0        0      976 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/context.py
--rw-r--r--   0        0        0    32221 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/db.py
--rw-r--r--   0        0        0     2260 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/decorators.py
--rw-r--r--   0        0        0     3525 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/errors.py
--rw-r--r--   0        0        0    41236 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/fixtures/countries.json
--rw-r--r--   0        0        0    23777 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/jobs.py
--rw-r--r--   0        0        0     7231 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/log.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/management/commands/__init__.py
--rw-r--r--   0        0        0     3827 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/management/commands/create_groups.py
--rw-r--r--   0        0        0     1629 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/middleware.py
--rw-r--r--   0        0        0    14035 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/migrations/0001_sortinghat.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/migrations/__init__.py
--rw-r--r--   0        0        0    10735 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/models.py
--rw-r--r--   0        0        0      839 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/recommendations/__init__.py
--rw-r--r--   0        0        0     4272 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/recommendations/affiliation.py
--rw-r--r--   0        0        0     3137 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/recommendations/engine.py
--rw-r--r--   0        0        0     5313 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/recommendations/exclusion.py
--rw-r--r--   0        0        0     5642 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/recommendations/gender.py
--rw-r--r--   0        0        0     9134 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/recommendations/matching.py
--rw-r--r--   0        0        0    66688 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/schema.py
--rw-r--r--   0        0        0     2944 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/core/views.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/server/__init__.py
--rw-r--r--   0        0        0     9659 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/server/sortinghat_admin.py
--rw-r--r--   0        0        0     2884 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/server/sortinghatd.py
--rw-r--r--   0        0        0     2344 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/server/sortinghatw.py
--rwxr-xr-x   0        0        0     9218 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/server/utils/create_sh_0_7_fixture.py
--rw-r--r--   0        0        0     3485 2023-02-03 08:31:08.693913 sortinghat-0.8.1/sortinghat/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/config_file.cfg
--rw-r--r--   0        0        0     7601 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/test_cmd_add.py
--rw-r--r--   0        0        0    17698 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/test_cmd_config.py
--rw-r--r--   0        0        0    10234 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/test_cmd_countries.py
--rw-r--r--   0        0        0     7597 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/test_cmd_enroll.py
--rw-r--r--   0        0        0     5397 2023-02-03 08:31:08.693913 sortinghat-0.8.1/tests/cli/test_cmd_lock.py
--rw-r--r--   0        0        0     3851 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_merge.py
--rw-r--r--   0        0        0     5041 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_mv.py
--rw-r--r--   0        0        0    13658 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_orgs.py
--rw-r--r--   0        0        0     9117 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_profile.py
--rw-r--r--   0        0        0     4599 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_rm.py
--rw-r--r--   0        0        0    10993 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_show.py
--rw-r--r--   0        0        0     5280 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_split.py
--rw-r--r--   0        0        0     6294 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/cli/test_cmd_withdraw.py
--rw-r--r--   0        0        0        0 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/rec/__init__.py
--rw-r--r--   0        0        0     7474 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/rec/test_affiliations.py
--rw-r--r--   0        0        0     2922 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/rec/test_engine.py
--rw-r--r--   0        0        0     3937 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/rec/test_exclusion.py
--rw-r--r--   0        0        0     8536 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/rec/test_gender.py
--rw-r--r--   0        0        0    11764 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/rec/test_matches.py
--rw-r--r--   0        0        0   246207 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_api.py
--rw-r--r--   0        0        0    18369 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_aux.py
--rw-r--r--   0        0        0    10429 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_client.py
--rw-r--r--   0        0        0   108682 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_db.py
--rw-r--r--   0        0        0     8272 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_errors.py
--rw-r--r--   0        0        0    51906 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_jobs.py
--rw-r--r--   0        0        0    14074 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_log.py
--rw-r--r--   0        0        0    42952 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_model.py
--rw-r--r--   0        0        0   396484 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_schema.py
--rw-r--r--   0        0        0     6316 2023-02-03 08:31:08.697913 sortinghat-0.8.1/tests/test_utils.py
--rw-r--r--   0        0        0     9271 1970-01-01 00:00:00.000000 sortinghat-0.8.1/setup.py
--rw-r--r--   0        0        0     8822 1970-01-01 00:00:00.000000 sortinghat-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/LICENSE
+-rw-r--r--   0        0        0    11752 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/NEWS
+-rw-r--r--   0        0        0     8566 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/README.md
+-rw-r--r--   0        0        0     2013 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/_version.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/schema.py
+-rw-r--r--   0        0        0      518 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/urls.py
+-rw-r--r--   0        0        0      196 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/app/wsgi.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/client/__init__.py
+-rw-r--r--   0        0        0     5738 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/client/client.py
+-rw-r--r--   0        0        0    43408 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/client/schema.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     3072 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/add.py
+-rw-r--r--   0        0        0     6145 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/config.py
+-rw-r--r--   0        0        0     3219 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/countries.py
+-rw-r--r--   0        0        0     3462 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/enroll.py
+-rw-r--r--   0        0        0     2860 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/lock.py
+-rw-r--r--   0        0        0     2342 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/merge.py
+-rw-r--r--   0        0        0     2352 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/mv.py
+-rw-r--r--   0        0        0     7466 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/orgs.py
+-rw-r--r--   0        0        0     2934 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/profile.py
+-rw-r--r--   0        0        0     1992 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/rm.py
+-rw-r--r--   0        0        0     2909 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/show.py
+-rw-r--r--   0        0        0     2365 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/split.py
+-rw-r--r--   0        0        0     3364 2023-04-20 16:55:14.079059 sortinghat-0.9.0rc1/sortinghat/cli/cmds/withdraw.py
+-rwxr-xr-x   0        0        0     2857 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/sortinghat.py
+-rw-r--r--   0        0        0       43 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/add.tmpl
+-rw-r--r--   0        0        0       23 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/config.tmpl
+-rw-r--r--   0        0        0       83 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/countries.tmpl
+-rw-r--r--   0        0        0       54 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/lock.tmpl
+-rw-r--r--   0        0        0      169 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/mv.tmpl
+-rw-r--r--   0        0        0      208 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/organizations.tmpl
+-rw-r--r--   0        0        0      375 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/profile.tmpl
+-rw-r--r--   0        0        0      106 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/rm.tmpl
+-rw-r--r--   0        0        0     1016 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/show.tmpl
+-rw-r--r--   0        0        0       69 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/templates/split.tmpl
+-rw-r--r--   0        0        0     4856 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/config/__init__.py
+-rw-r--r--   0        0        0     9252 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/config/settings.py
+-rw-r--r--   0        0        0       20 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/config/tenants.json
+-rw-r--r--   0        0        0     1544 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/admin.py
+-rw-r--r--   0        0        0    50534 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/api.py
+-rw-r--r--   0        0        0      926 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/apps.py
+-rw-r--r--   0        0        0     5169 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/aux.py
+-rw-r--r--   0        0        0      997 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/context.py
+-rw-r--r--   0        0        0    37055 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/db.py
+-rw-r--r--   0        0        0     3019 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/decorators.py
+-rw-r--r--   0        0        0     3875 2023-04-20 16:55:14.083059 sortinghat-0.9.0rc1/sortinghat/core/errors.py
+-rw-r--r--   0        0        0    41236 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/fixtures/countries.json
+-rw-r--r--   0        0        0     7820 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/backend.py
+-rw-r--r--   0        0        0     7136 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/backends/mailmap.py
+-rw-r--r--   0        0        0     5817 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/base.py
+-rw-r--r--   0        0        0     2143 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/models.py
+-rw-r--r--   0        0        0     2059 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/importer/utils.py
+-rw-r--r--   0        0        0    25814 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/jobs.py
+-rw-r--r--   0        0        0     7298 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/log.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     4155 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/management/commands/create_groups.py
+-rw-r--r--   0        0        0     4354 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/middleware.py
+-rw-r--r--   0        0        0    14035 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/0001_sortinghat.py
+-rw-r--r--   0        0        0     1717 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/0002_importidentitiestask.py
+-rw-r--r--   0        0        0     1502 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/0003_multi_tenancy.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/migrations/__init__.py
+-rw-r--r--   0        0        0    11931 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/models.py
+-rw-r--r--   0        0        0      839 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/__init__.py
+-rw-r--r--   0        0        0     4272 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/affiliation.py
+-rw-r--r--   0        0        0     3137 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/engine.py
+-rw-r--r--   0        0        0     5313 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/exclusion.py
+-rw-r--r--   0        0        0     5642 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/gender.py
+-rw-r--r--   0        0        0     9134 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/recommendations/matching.py
+-rw-r--r--   0        0        0    74254 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/schema.py
+-rw-r--r--   0        0        0     2394 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/tenant.py
+-rw-r--r--   0        0        0     2944 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/core/views.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/__init__.py
+-rw-r--r--   0        0        0    13705 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/sortinghat_admin.py
+-rw-r--r--   0        0        0     2884 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/sortinghatd.py
+-rw-r--r--   0        0        0     2365 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/sortinghatw.py
+-rwxr-xr-x   0        0        0     9218 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/server/utils/create_sh_0_7_fixture.py
+-rw-r--r--   0        0        0     3485 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/sortinghat/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/config_file.cfg
+-rw-r--r--   0        0        0     7601 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_add.py
+-rw-r--r--   0        0        0    17698 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_config.py
+-rw-r--r--   0        0        0    10234 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_countries.py
+-rw-r--r--   0        0        0     7597 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_enroll.py
+-rw-r--r--   0        0        0     5397 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_lock.py
+-rw-r--r--   0        0        0     3851 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_merge.py
+-rw-r--r--   0        0        0     5041 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_mv.py
+-rw-r--r--   0        0        0    13658 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_orgs.py
+-rw-r--r--   0        0        0     9117 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_profile.py
+-rw-r--r--   0        0        0     4599 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_rm.py
+-rw-r--r--   0        0        0    10993 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_show.py
+-rw-r--r--   0        0        0     5280 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_split.py
+-rw-r--r--   0        0        0     6294 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/cli/test_cmd_withdraw.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1055 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/backend_a.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1050 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_c.py
+-rw-r--r--   0        0        0      865 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_not_backend.py
+-rw-r--r--   0        0        0     4797 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/test_backend.py
+-rw-r--r--   0        0        0     2416 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/importer/test_utils.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/__init__.py
+-rw-r--r--   0        0        0     7474 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_affiliations.py
+-rw-r--r--   0        0        0     2922 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_engine.py
+-rw-r--r--   0        0        0     3937 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_exclusion.py
+-rw-r--r--   0        0        0     8536 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_gender.py
+-rw-r--r--   0        0        0    11764 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/rec/test_matches.py
+-rw-r--r--   0        0        0      825 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/runners.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:55:14.087060 sortinghat-0.9.0rc1/tests/tenants/__init__.py
+-rw-r--r--   0        0        0     3781 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/tenants/test_jobs.py
+-rw-r--r--   0        0        0     2273 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/tenants/test_middleware.py
+-rw-r--r--   0        0        0     5872 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/tenants/test_schema.py
+-rw-r--r--   0        0        0   258794 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_api.py
+-rw-r--r--   0        0        0    18369 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_aux.py
+-rw-r--r--   0        0        0    10449 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_client.py
+-rw-r--r--   0        0        0   125568 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_db.py
+-rw-r--r--   0        0        0     9257 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_errors.py
+-rw-r--r--   0        0        0    54990 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_jobs.py
+-rw-r--r--   0        0        0    14074 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_log.py
+-rw-r--r--   0        0        0    47504 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_model.py
+-rw-r--r--   0        0        0   399040 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_schema.py
+-rw-r--r--   0        0        0     6316 2023-04-20 16:55:14.091060 sortinghat-0.9.0rc1/tests/test_utils.py
+-rw-r--r--   0        0        0    10402 1970-01-01 00:00:00.000000 sortinghat-0.9.0rc1/PKG-INFO
```

### Comparing `sortinghat-0.8.1/LICENSE` & `sortinghat-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/NEWS` & `sortinghat-0.9.0rc1/NEWS`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/README.md` & `sortinghat-0.9.0rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ```
 $ apt install libmysqlclient-dev
 ```
 
 * **MariaDB**
 
 ```
-$ apt install libmariadbclient-dev
+$ apt install libmariadbclient-dev-compat
 ```
 
 #### Installation and configuration
 
 **Note**: these examples use `sortinghat.config.settings` configuration file.
 In order to use that configuration you need to define the environment variable
 `SORTINGHAT_SECRET_KEY` with a secret. More info here:
@@ -124,15 +124,15 @@
 $ yarn install
 ```
 
 #### Running the frontend
 
 Run SortingHat frontend Vue app:
 ```
-$ yarn serve
+$ yarn serve --api_url=http://localhost:8000/api/
 ```
 
 
 ## SortingHat service
 
 Starting at version 0.8, SortingHat is released with a server app. The server has two
 modes, `production` and `development`.
@@ -151,14 +151,20 @@
 Following examples will make use of that file.
 
 In order to run the service for the first time, you need to execute the next commands:
 
 Build the UI interface:
 ```
 $ cd ui
+$ yarn install
+$ yarn build --mode development
+```
+If you want to run the UI at `/identities` run (you need to use the server 
+behind a proxy server):
+```
 $ yarn build
 ```
 
 Set a secret key:
 ```
 $ export SORTINGHAT_SECRET_KEY="my-secret-key"
 ```
@@ -179,14 +185,29 @@
 
 You will also need to run some workers to execute tasks like recommendations
 or affiliation. To start a worker run the command:
 ```
 $ sortinghatw --config sortinghat.config.settings
 ```
 
+## Create new accounts
+To create new accounts for SortingHat use the following command:
+
+```
+(.venv)$ sortinghat-admin create-user
+
+Usage: sortinghat-admin create-user [OPTIONS]
+
+  Create a new user given a username and password
+
+Options:
+  --username TEXT   Specifies the login for the user.
+  --is-admin        Specifies if the user is superuser.
+  --no-interactive  Run the command in no interactive mode.
+```
 
 ## Compatibility between versions
 SortingHat 0.7.x is no longer supported. Any database using this version will not work.
 
 SortingHat databases 0.7.x are no longer compatible. The `uidentities` table was renamed
 to `individuals`. The database schema changed in all tables to add the fields `created_at`
 and `last_modified`. Also in `domains`, `enrollments`, `identities`, `profiles` tables,
@@ -203,22 +224,43 @@
     * `uuid` to `individual`
 
 Please update your database running the following command:
 ```
 $ sortinghat-admin --config sortinghat.config.settings migrate-old-database
 ```
 
+## Multi-tenancy
+
+SortingHat allows hosting multiple instances with a single service having each
+instance's data isolated in different databases.
+
+To enable this feature follow these guidelines:
+- Set `MULTI_TENANT` settings to `True`.
+- Define a list of tenants using the configuration file `sortinghat/config/tenants.json`. 
+You can use a different json file using the environment variable 
+`SORTINGHAT_MULTI_TENANT_LIST_PATH`
+- Assign users to tenants with the following command:
+  `sortinghat-admin set-user-tenant username host tenant`
+
+There are some limitations:
+- `default` database is only used to store users information and relations between
+users and databases, it won't store anything else related with SortingHat models.
+- Usernames are shared across all instances, which means that it is not possible
+to have the same username with two different passwords in different instances.
+
+
 ## Running tests
 
 SortingHat comes with a comprehensive list of unit tests for both 
 frontend and backend.
 
 #### Backend test suite
 ```
 (.venv)$ ./manage.py test --settings=config.settings.testing
+(.venv)$ ./manage.py test --settings=config.settings.testing_tenant
 ```
 
 #### Frontend test suite
 ```
 $ cd ui/
 $ yarn test:unit
 ```
```

### Comparing `sortinghat-0.8.1/pyproject.toml` & `sortinghat-0.9.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat"
-version = "0.8.1"
+version = "0.9.0-rc.1"
 description = "A tool to manage identities."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -50,15 +50,15 @@
 [tool.poetry.dependencies]
 python = "^3.7.1"
 
 click = "7.1.1"
 Django = "^3.2"
 django-graphql-jwt = "^0.3.0"
 graphene-django = "^2.15"
-sgqlc = "^10.1"
+sgqlc = "^16.1"
 mysqlclient = "2.0.3"
 python-dateutil = "^2.8.2"
 requests = "^2.7.0"
 Jinja2 = "^3.1.1"
 rq = "<1.12.0"
 django-rq = "^2.3.2"
 pandas = "^1.3.5"
```

### Comparing `sortinghat-0.8.1/sortinghat/app/schema.py` & `sortinghat-0.9.0rc1/sortinghat/app/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/app/urls.py` & `sortinghat-0.9.0rc1/sortinghat/app/urls.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/client/__init__.py` & `sortinghat-0.9.0rc1/sortinghat/cli/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/client/client.py` & `sortinghat-0.9.0rc1/sortinghat/cli/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import requests
 import urllib.parse
 
-from sgqlc.endpoint.http import HTTPEndpoint
+from sgqlc.endpoint.requests import RequestsEndpoint
 from sgqlc.operation import Operation
 from sgqlc.types import Scalar
 
 from .schema import sh_schema
 
 
 # Ensure strings are sent using their original encoding
@@ -66,18 +66,19 @@
     :param path: path to the API endpoint; by default the endpoint is in '/'
     :param user: user name to use when authentication is required
     :param password: password to use when authentication is required
     :param ssl: use SSL/TSL connection; this is the default behaviour
 
     :raises ValueError: when any of the given parameters is invalid
     """
-    def __init__(self, host, port=9314, path=None, user=None, password=None, ssl=True):
+    def __init__(self, host, port=9314, path=None, user=None, password=None, ssl=True, verify_ssl=True):
         self.gqlc = None
         self.host = host
         self.port = port
+        self.verify_ssl = verify_ssl
 
         scheme = 'https' if ssl else 'http'
         netloc = self.host + ':' + str(self.port) if self.port else self.host
 
         if not path:
             self.path = '/'
         elif not path.startswith('/'):
@@ -97,30 +98,33 @@
         except (ValueError, TypeError) as exc:
             msg = "Invalid URL parameters; cause: {}".format(exc)
             raise ValueError(msg)
 
     def connect(self):
         """Establish a connection to the server."""
 
+        session = requests.Session()
+        session.verify = self.verify_ssl
+
         try:
-            result = requests.get(self.url, headers={'Accept': 'text/html'})
+            result = session.get(self.url, headers={'Accept': 'text/html'})
             result.raise_for_status()
         except requests.exceptions.RequestException as exc:
             if result.status_code != 400:
                 msg = "Connection error; cause: {}".format(exc)
                 raise SortingHatClientError(msg)
 
         headers = {
             'X-CSRFToken': result.cookies['csrftoken'],
             'Cookie': 'csrftoken=' + result.cookies['csrftoken'],
             'Host': f"{self.host}:{self.port}" if self.port else self.host,
             'Referer': self.url
         }
 
-        self.gqlc = HTTPEndpoint(self.url, headers)
+        self.gqlc = RequestsEndpoint(self.url, headers, session=session)
 
         if self.user and self.password:
             op = Operation(sh_schema.SortingHatMutation)
             op.token_auth(username=self.user, password=self.password).token()
 
             result = self.gqlc(op)
```

### Comparing `sortinghat-0.8.1/sortinghat/cli/client/schema.py` & `sortinghat-0.9.0rc1/sortinghat/cli/client/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/add.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/config.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/countries.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/enroll.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/lock.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/merge.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/mv.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/orgs.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/profile.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/rm.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/show.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/split.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/cmds/withdraw.py` & `sortinghat-0.9.0rc1/sortinghat/cli/cmds/withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/sortinghat.py` & `sortinghat-0.9.0rc1/sortinghat/cli/sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/templates/show.tmpl` & `sortinghat-0.9.0rc1/sortinghat/cli/templates/show.tmpl`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/cli/utils.py` & `sortinghat-0.9.0rc1/sortinghat/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/config/settings.py` & `sortinghat-0.9.0rc1/sortinghat/config/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 #
 # Please check the next links for details about the configuration
 # in a production environment:
 #
 # https://docs.djangoproject.com/en/3.1/howto/deployment/checklist/
 # https://docs.djangoproject.com/en/3.1/ref/settings/
 #
-
+import json
 import os
 
-
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 SILENCED_SYSTEM_CHECKS = [
     'django_mysql.E016'
 ]
 
 #
@@ -119,15 +118,14 @@
     ],
 }
 
 GRAPHQL_JWT = {
     'JWT_ALLOW_ANY_HANDLER': 'sortinghat.core.middleware.allow_any'
 }
 
-
 #
 # Authentication - DO NOT MODIFY
 #
 
 AUTHENTICATION_BACKENDS = [
     'django.contrib.auth.backends.ModelBackend',
     'graphql_jwt.backends.JSONWebTokenBackend',
@@ -267,14 +265,48 @@
         'PASSWORD': os.environ.get('SORTINGHAT_DB_PASSWORD', ''),
         'NAME': os.environ.get('SORTINGHAT_DB_DATABASE', 'sortinghat_test'),
         'OPTIONS': {'charset': 'utf8mb4'},
     }
 }
 
 #
+# SortingHat Multi-tenant
+#
+# To enable this feature:
+#   - Define SORTINGHAT_MULTI_TENANT to True
+#   - Create a list of tenants in sortinghat.config.tenants
+#   - Assign users to tenants with 'set_user_tenant' command.
+#
+
+MULTI_TENANT = os.environ.get('SORTINGHAT_MULTI_TENANT', 'False').lower() in ('true', '1')
+
+if MULTI_TENANT:
+    MIDDLEWARE += ['sortinghat.core.middleware.TenantDatabaseMiddleware']
+    DATABASE_ROUTERS = [
+        'sortinghat.core.middleware.TenantDatabaseRouter'
+    ]
+    MULTI_TENANT_LIST_PATH = os.environ.get('SORTINGHAT_MULTI_TENANT_LIST_PATH',
+                                            os.path.join(BASE_DIR, 'config', 'tenants.json'))
+    with open(MULTI_TENANT_LIST_PATH, 'r') as f:
+        TENANTS_NAMES = json.load(f).get('tenants', [])
+
+    DATABASES.update({
+        tenant: {
+            'ENGINE': 'django.db.backends.mysql',
+            'HOST': os.environ.get('SORTINGHAT_DB_HOST', '127.0.0.1'),
+            'PORT': os.environ.get('SORTINGHAT_DB_PORT', 3306),
+            'USER': os.environ.get('SORTINGHAT_DB_USER', 'root'),
+            'PASSWORD': os.environ.get('SORTINGHAT_DB_PASSWORD', ''),
+            'NAME': tenant,
+            'OPTIONS': {'charset': 'utf8mb4'},
+        }
+        for tenant in TENANTS_NAMES
+    })
+
+#
 # SortingHat workers
 #
 # SortingHat uses RQ to run background and async jobs.
 # You'll HAVE TO set the next parameters in order to run
 # them in the background. If not, set ASYNC to 'False'.
 #
 # Take into account RQ uses Redis database. You have more
```

### Comparing `sortinghat-0.8.1/sortinghat/core/admin.py` & `sortinghat-0.9.0rc1/sortinghat/core/admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/api.py` & `sortinghat-0.9.0rc1/sortinghat/core/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,56 +18,58 @@
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
 import logging
 
-import django.db.transaction
-
 from grimoirelab_toolkit.datetime import datetime_to_utc
 
 from .db import (find_individual_by_uuid,
                  find_identity,
                  find_organization,
                  find_domain,
                  find_team,
                  find_group,
+                 find_import_identities_task,
                  search_enrollments_in_period,
                  add_individual as add_individual_db,
                  add_identity as add_identity_db,
                  add_organization as add_organization_db,
                  add_team as add_team_db,
                  add_domain as add_domain_db,
                  delete_individual as delete_individual_db,
                  delete_identity as delete_identity_db,
                  delete_organization as delete_organization_db,
                  delete_team as delete_team_db,
+                 delete_import_identities_task as delete_import_task_db,
                  delete_domain as delete_domain_db,
                  update_profile as update_profile_db,
+                 update_import_identities_task as update_import_task_db,
                  move_identity as move_identity_db,
                  lock as lock_db,
                  unlock as unlock_db,
                  add_enrollment,
                  delete_enrollment)
 from .errors import (InvalidValueError,
                      AlreadyExistsError,
                      NotFoundError,
                      DuplicateRangeError,
                      EqualIndividualError)
 from .log import TransactionsLog
 from .models import Identity, MIN_PERIOD_DATE, MAX_PERIOD_DATE
 from .aux import merge_datetime_ranges
+from .decorators import atomic_using_tenant
 from ..utils import generate_uuid
 
 
 logger = logging.getLogger(__name__)
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def add_identity(ctx, source, name=None, email=None, username=None, uuid=None):
     """Add an identity to the registry.
 
     This function adds a new identity to the registry. By default,
     a new individual will be also added and associated to
     the new identity.
 
@@ -150,15 +152,15 @@
         logger.info(f"Individual {individual.mk} created")
 
     logger.info(f"Identity {identity.uuid} created for individual {individual.mk}")
 
     return identity
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def delete_identity(ctx, uuid):
     """Remove an identity from the registry.
 
     This function removes from the registry the identity which
     its identifier matches with `uuid`. When the `uuid` also
     belongs to an individual, this entry and those identities
     linked to it will be removed too. The value of this identifier
@@ -206,15 +208,15 @@
 
     if not individual:
         logger.info(f"Individual {uuid} deleted")
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def update_profile(ctx, uuid, **kwargs):
     """Update individual profile.
 
     This function allows to edit or update the profile information
     of the individual identified by `uuid`. Take into account that
     any UUID of the identities of the individual is a valid identifier.
 
@@ -258,15 +260,15 @@
     trxl.close()
 
     logger.info(f"Identity {uuid} profile successfully updated")
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def move_identity(ctx, from_uuid, to_uuid):
     """Move an identity to an individual.
 
     This function shifts the identity identified by `from_uuid` to
     the individual identified by `to_uuid`. Take into account that
     any UUID of the identities of the individual is a valid
     identifier.
@@ -333,15 +335,15 @@
     trxl.close()
 
     logger.info(f"Identity {from_uuid} moved to {to_uuid}")
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def lock(ctx, uuid):
     """Lock an individual so it cannot be modified.
 
     This function locks the individual identified by `uuid`
     so this object and its related objects such as identities,
     enrollments or the profile cannot be modified.
 
@@ -367,15 +369,15 @@
     trxl.close()
 
     logger.info(f"Individual {uuid} successfully locked")
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def unlock(ctx, uuid):
     """Unlock an individual so it can be modified.
 
     This function unlocks the individual identified by `uuid`
     so this object and its related objects such as identities,
     enrollments or the profile can be modified.
 
@@ -401,15 +403,15 @@
     trxl.close()
 
     logger.info(f"Individual {uuid} successfully unlocked")
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def add_organization(ctx, name):
     """Add an organization to the registry.
 
     This function adds an organization to the registry.
     It checks first whether the organization is already on the registry.
     When it is not found, the new organization is added. Otherwise,
     it raises a 'AlreadyExistsError' exception to notify that the organization
@@ -438,15 +440,15 @@
     trxl.close()
 
     logger.info(f"Organization {org.name} created")
 
     return org
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def add_domain(ctx, organization, domain_name, is_top_domain=True):
     """Add a domain to the registry.
 
     This function adds a new domain to a given organization.
     The organization must exist on the registry prior to insert the new
     domain. Otherwise, it will raise a `NotFoundError` exception. Moreover,
     if the given domain is already in the registry an `AlreadyExistsError`
@@ -503,15 +505,15 @@
     trxl.close()
 
     logger.info(f"Domain {domain.domain} created for organization {organization.name}")
 
     return domain
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def add_team(ctx, team_name, organization=None, parent_name=None):
     """Add a team to the registry.
 
     This function creates a new team. If organization is given, the team is added to
     the organization. The organization must exist on the registry prior to insert the new
     team. Otherwise, it will raise a `NotFoundError` exception. Moreover,
     if the given team already exists in the organization, an `AlreadyExistsError`
@@ -570,15 +572,15 @@
         raise exc
 
     trxl.close()
     logger.info(f"Team {team.name} created " + f"for {organization.name}" if organization else "")
     return team
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def delete_organization(ctx, name):
     """Remove an organization from the registry.
 
     This function removes the given organization from the registry.
     Related information such as domains or enrollments are also removed.
     It checks first whether the organization is already on the registry.
     When it is found, the organization is removed. Otherwise,
@@ -610,15 +612,15 @@
     trxl.close()
 
     logger.info(f"Organization {name} deleted")
 
     return org
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def delete_domain(ctx, domain_name):
     """Remove a domain from the registry.
 
     This function removes the given domain from the registry.
     Domain must exist in the registry. Otherwise, it will raise
     a `NotFoundError` exception.
 
@@ -649,15 +651,15 @@
     trxl.close()
 
     logger.info(f"Domain {domain_name} deleted")
 
     return domain
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def delete_team(ctx, team_name, organization=None):
     """Remove a team from the registry.
 
     This function removes the given team from the registry.
     Deleting a team also deletes all its subteams from the registry.
     If the team belongs to an Organization, the organization name must
     be passed. Both Organization and Team must exist in the registry.
@@ -698,15 +700,15 @@
     delete_team_db(trxl, team)
 
     trxl.close()
     logger.info(f"Team {team.name} deleted")
     return team
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def enroll(ctx, uuid, group, parent_org=None, from_date=None, to_date=None,
            force=False):
     """Enroll an individual in a group.
 
     The function enrolls an individual, identified by `uuid`,
     in the given `group`. Both identity and group must
     exist before adding this enrollment to the registry. Otherwise,
@@ -814,15 +816,15 @@
         f"Individual {uuid} enrolled to {group}; "
         f"from='{from_date}' to='{to_date}'"
     )
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def withdraw(ctx, uuid, group, parent_org=None, from_date=None, to_date=None):
     """Withdraw an individual from a group.
 
     This function withdraws an individual identified by `uuid`
     from the given `group` during the given period of time.
     As in other functions, any UUID of the identities of the individual
     is a valid identifier.
@@ -928,15 +930,15 @@
         f"Individual {uuid} withdrawn from {group}; "
         f"from='{from_date}' to='{to_date}';"
     )
 
     return individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def update_enrollment(ctx, uuid, group, from_date, to_date, parent_org=None,
                       new_from_date=None, new_to_date=None, force=True):
     """Update one or more enrollments from an individual given a new date range.
 
     Use this method to update atomically an individual's enrollment or set
     of enrollments defined by the initial date range to a new date range.
 
@@ -1017,15 +1019,15 @@
         f"Individual {uuid} enrollments of {group} updated; "
         f"from='{from_date}' to='{to_date}'; new_from='{new_from_date}' new_to='{new_to_date}';"
     )
 
     return indv
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def merge(ctx, from_uuids, to_uuid):
     """
     Merge one or more individuals into another.
 
     Use this function to join a list of individuals, defined in `from_uuid`
     by any of their valid identities ids, into `to_uuid` individual.
     Identities and enrollments related to each `from_uuid` will be assigned
@@ -1190,15 +1192,15 @@
     to_individual.refresh_from_db()
 
     logger.info(f"Individuals {from_uuids} merged with {to_uuid}")
 
     return to_individual
 
 
-@django.db.transaction.atomic
+@atomic_using_tenant
 def unmerge_identities(ctx, uuids):
     """
     Unmerge one or more identities from their corresponding individual.
 
     Use this function to separate a list of `uuid` identities, creating
     an individual for each one. A profile for each new individual will
     be created using the `name` and `email` fields of the corresponding
@@ -1284,7 +1286,92 @@
         new_individuals.append(individual)
 
     trxl.close()
 
     logger.info(f"Identities {uuids} unmerged from their individuals")
 
     return new_individuals
+
+
+@atomic_using_tenant
+def delete_import_identities_task(ctx, task_id):
+    """Remove an import identities task from the registry.
+
+    This function removes the given task from the registry.
+    When it is found, the task is removed. Otherwise, it will
+    raise a 'NotFoundError'.
+
+    :param ctx: context from where this method is called
+    :param task_id: id of the task to remove
+
+    :raises InvalidValueError: raised when task is None or an empty string
+    :raises NotFoundError: raised when the task does not exist
+        in the registry
+    """
+    if not task_id:
+        raise InvalidValueError(msg="'task_id' cannot be empty or None")
+
+    trxl = TransactionsLog.open('delete_import_task', ctx)
+
+    try:
+        task = find_import_identities_task(task_id)
+    except NotFoundError as exc:
+        raise exc
+
+    delete_import_task_db(trxl, task=task)
+
+    trxl.close()
+
+    logger.info(f"Task {task_id} deleted")
+
+    return task
+
+
+@atomic_using_tenant
+def update_import_identities_task(ctx, task_id, **kwargs):
+    """Update an import identities task.
+
+    This function allows to edit or update the information of
+    the ImportIdentitiesTask identified by the given id.
+
+    The values to update are given as keyword arguments. The allowed
+    keys are listed below (other keywords will be ignored):
+
+       - `backend`: name of the importer backend
+       - `url`: URL of a file or API to fetch the identities from
+       - `interval`: period of executions, in minutes. None to disable
+       - `params`: specific parameters for the importer backend
+
+    As a result, it will return the `ImportIdentitiesTask` object with
+    the updated data.
+
+    :param ctx: context from where this method is called.
+    :param task_id: identifier of the task to update.
+    :param kwargs: keyword arguments with data to update the task.
+
+    :returns: task object with the updated information
+
+    :raises NotFoundError: raised when either the task does not exist
+        in the registry.
+    :raises InvalidValueError: raised when any of the keyword arguments
+        has an invalid value.
+    """
+    if not task_id:
+        raise InvalidValueError(msg="'task_id' cannot be None")
+
+    trxl = TransactionsLog.open('update_import_task', ctx)
+
+    try:
+        task = find_import_identities_task(task_id)
+    except NotFoundError as exc:
+        raise exc
+
+    try:
+        task = update_import_task_db(trxl, task, **kwargs)
+    except ValueError as e:
+        raise InvalidValueError(msg=str(e))
+
+    trxl.close()
+
+    logger.info(f"Task {task_id} successfully updated")
+
+    return task
```

### Comparing `sortinghat-0.8.1/sortinghat/core/apps.py` & `sortinghat-0.9.0rc1/sortinghat/core/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
+import os
+
 from django.apps import AppConfig
 
 
 class SortingHatCoreConfig(AppConfig):
     name = 'sortinghat.core'
+    path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `sortinghat-0.8.1/sortinghat/core/aux.py` & `sortinghat-0.9.0rc1/sortinghat/core/aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/context.py` & `sortinghat-0.9.0rc1/tests/importer/mocked_package/nested_package/nested_backend_c.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2014-2020 Bitergia
+# Copyright (C) 2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,18 +13,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#     Santiago Dueñas <sduenas@bitergia.com>
-#     Miguel Ángel Fernández <mafesan@bitergia.com>
+#     Jose Javier Merchante <jjmerchante@bitergia.com>
 #
 
-import collections
+from sortinghat.core.importer.backend import IdentitiesImporter
 
 
-SortingHatContext = collections.namedtuple(
-    'SortingHatContext', ['user', 'job_id']
-)
-SortingHatContext.__new__.__defaults__ = (None, None)
+class BackendC(IdentitiesImporter):
+    """Mocked backend class used for testing"""
+
+    NAME = 'C'
+
+    def __init__(self, ctx, url, foo):
+        super().__init__(ctx, url)
+        self.token = foo
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sortinghat-0.8.1/sortinghat/core/db.py` & `sortinghat-0.9.0rc1/sortinghat/core/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                      Group,
                      Domain,
                      Country,
                      Individual,
                      Identity,
                      Profile,
                      Enrollment,
-                     Operation)
+                     Operation,
+                     ImportIdentitiesTask)
 from .aux import validate_field
 
 
 logger = logging.getLogger(__name__)
 
 
 def _set_lock(individual, lock_flag):
@@ -902,14 +903,162 @@
     trxl.log_operation(op_type=Operation.OpType.UPDATE, entity_type='identity',
                        timestamp=datetime_utcnow(), args=op_args,
                        target=op_args['identity'])
 
     return individual
 
 
+def find_import_identities_task(task_id):
+    """Find a group.
+
+    Find a task by its id in the database.
+
+    When the task does not exist the function will raise
+    a `NotFoundError`.
+
+    :param task_id: id of the task to find
+
+    :returns: a ImportIdentitiesTask object
+
+    :raises NotFoundError: when the task with the
+        given `task_id` does not exist.
+    """
+    try:
+        logger.debug(f"Finding task '{task_id}'")
+        task = ImportIdentitiesTask.objects.get(id=task_id)
+    except ImportIdentitiesTask.DoesNotExist:
+        logger.debug(f"Task with id '{task_id}' does not exist")
+        raise NotFoundError(entity=task_id)
+    else:
+        logger.debug(f"Task with id '{task_id}' was found")
+        return task
+
+
+def add_import_identities_task(trxl, backend, url, args=None, interval=None, job_id=None):
+    """Add an import identities task to the database.
+
+    This function adds a new task to the database.
+
+    As a result, the function returns a new `ImportIdentitiesTask` object.
+
+    :param trxl: TransactionsLog object from the method calling this one
+    :param backend: name of the importer backend
+    :param url: URL of a file or API to fetch the identities from
+    :param interval: period of executions, in minutes. None to disable
+    :param args: specific arguments for the importer backend
+    :param job_id: current job running the task
+
+    :returns: a new ImportIdentitiesTask
+    """
+    # Setting operation arguments before they are modified
+    op_args = {
+        'backend': backend,
+        'url': url,
+        'interval': str(interval),
+        'args': str(args),
+        'job_id': job_id,
+    }
+
+    validate_field('backend', backend)
+    validate_field('url', url)
+
+    if interval and interval < 0:
+        raise ValueError("'interval' must be a positive number or 0.")
+
+    try:
+        task = ImportIdentitiesTask(
+            backend=backend,
+            url=url,
+            interval=interval,
+            args=args,
+            job_id=job_id
+        )
+        task.save()
+    except django.db.utils.IntegrityError as exc:
+        _handle_integrity_error(ImportIdentitiesTask, exc)
+
+    trxl.log_operation(op_type=Operation.OpType.ADD, entity_type='import_task',
+                       timestamp=datetime_utcnow(), args=op_args,
+                       target=op_args['url'])
+
+    return task
+
+
+def delete_import_identities_task(trxl, task):
+    """Remove a task from the database.
+
+    This function removes from the database the task given
+    in `task`.
+
+    :param trxl: TransactionsLog object from the method calling this one
+    :param task: task to remove
+    """
+    # Setting operation arguments before they are modified
+    op_args = {
+        'task': str(task.id)
+    }
+
+    task.delete()
+
+    trxl.log_operation(op_type=Operation.OpType.DELETE, entity_type='import_task',
+                       timestamp=datetime_utcnow(), args=op_args,
+                       target=op_args['task'])
+
+
+def update_import_identities_task(trxl, task, **kwargs):
+    """Update an import identities task.
+
+    This function allows to edit or update the information of
+    the given task. The values to update are given as keyword
+    arguments. The allowed keys are listed below
+    (other keywords will be ignored):
+
+       - `backend`: name of the importer backend
+       - `url`: URL of a file or API to fetch the identities from
+       - `interval`: period of executions, in minutes. None to disable
+       - `params`: specific parameters for the importer backend
+
+    As a result, it will return the `ImportIdentitiesTask` object with
+    the updated data.
+
+    :param trxl: TransactionsLog object from the method calling this one
+    :param task: task to update
+    :param kwargs: parameters to edit the task
+
+    :returns: task object with the updated information
+
+    :raises ValueError: raised when an invalid value is provided
+    """
+    # Setting operation arguments before they are modified
+    op_args = copy.deepcopy(kwargs)
+    op_args.update({'task': str(task.id)})
+
+    if 'backend' in kwargs:
+        validate_field('backend', kwargs['backend'])
+        task.backend = kwargs['backend']
+    if 'url' in kwargs:
+        validate_field('url', kwargs['url'])
+        task.url = kwargs['url']
+    if 'interval' in kwargs:
+        interval = kwargs['interval']
+        if not isinstance(interval, int) or interval < 0:
+            raise ValueError("'interval' must be a positive number or 0.")
+        task.interval = interval
+    if 'params' in kwargs:
+        task.args = kwargs['params']
+
+    task.save()
+
+    trxl.log_operation(op_type=Operation.OpType.UPDATE, entity_type='import_task',
+                       timestamp=datetime_utcnow(), args=op_args,
+                       target=op_args['task'])
+
+    return task
+
+
 def lock(trxl, individual):
     """Lock a given individual.
 
     Locks a given `individual` object so this object and its related objects
     such as identities, enrollments or its profile cannot be modified.
 
     :param trxl: TransactionsLog object from the method calling this one
```

### Comparing `sortinghat-0.8.1/sortinghat/core/decorators.py` & `sortinghat-0.9.0rc1/sortinghat/core/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,22 +16,27 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
+from functools import wraps
+
+import django.db.transaction
+
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.http import HttpResponse
 from graphql_jwt.decorators import user_passes_test
 from graphql_jwt.utils import get_credentials
 from graphql_jwt.shortcuts import get_user_by_token
 from graphql_jwt.exceptions import JSONWebTokenError
 
+from . import tenant
 
 # This custom decorator takes the `user` object from the request's
 # context and checks the value of the `is_authenticated` variable
 # and the `AUTHENTICATION_REQUIRED` variable from the config settings.
 check_auth = user_passes_test(
     lambda u: u.is_authenticated or not settings.SORTINGHAT_AUTHENTICATION_REQUIRED
 )
@@ -55,7 +60,30 @@
             except JSONWebTokenError:
                 return HttpResponse(status=401)
             except ObjectDoesNotExist:
                 return HttpResponse(status=404)
         else:
             return HttpResponse(status=401)
     return wrap
+
+
+def atomic_using_tenant(func):
+    """This decorator uses transaction.atomic with the current db tenant"""
+
+    def using_tenant(*args, **kwargs):
+        using = tenant.get_db_tenant()
+        with django.db.transaction.atomic(using=using):
+            return func(*args, **kwargs)
+    return using_tenant
+
+
+def job_using_tenant(func):
+    """Use the tenant provided in the context argument for the job"""
+    @wraps(func)
+    def using_tenant(*args, **kwargs):
+        ctx = kwargs.get('ctx', args[0])
+        tenant.set_db_tenant(ctx.tenant)
+        try:
+            return func(*args, **kwargs)
+        finally:
+            tenant.unset_db_tenant()
+    return using_tenant
```

### Comparing `sortinghat-0.8.1/sortinghat/core/errors.py` & `sortinghat-0.9.0rc1/sortinghat/core/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
 CODE_BASE_ERROR = 1
 CODE_ALREADY_EXISTS_ERROR = 2
+CODE_INVALID_FORMAT_ERROR = 6
+CODE_LOAD_ERROR = 7
 CODE_NOT_FOUND_ERROR = 9
 CODE_VALUE_ERROR = 10
 CODE_CLOSED_TRANSACTION_ERROR = 12
 CODE_LOCKED_IDENTITY_ERROR = 13
 CODE_DUPLICATE_RANGE_ERROR = 14
 CODE_EQUAL_INDIVIDUAL_ERROR = 15
 CODE_FILTER_ERROR = 16
@@ -65,14 +67,28 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.entity = kwargs['entity']
         self.eid = kwargs['eid']
 
 
+class InvalidFormatError(BaseError):
+    """Exception raised when a format is invalid"""
+
+    message = "%(cause)s"
+    code = CODE_INVALID_FORMAT_ERROR
+
+
+class LoadError(BaseError):
+    """Exception raised when an error occurs loading data"""
+
+    message = "%(cause)s"
+    code = CODE_LOAD_ERROR
+
+
 class NotFoundError(BaseError):
     """Exception raised when an entity is not found in the registry"""
 
     message = "%(entity)s not found in the registry"
     code = CODE_NOT_FOUND_ERROR
```

### Comparing `sortinghat-0.8.1/sortinghat/core/fixtures/countries.json` & `sortinghat-0.9.0rc1/sortinghat/core/fixtures/countries.json`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/jobs.py` & `sortinghat-0.9.0rc1/sortinghat/core/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
+import datetime
 import itertools
 import logging
 
 import django_rq
 import django_rq.utils
 import pandas
 import rq
 
 from .db import find_individual_by_uuid, find_organization
 from .api import enroll, merge, update_profile
 from .context import SortingHatContext
+from .decorators import job_using_tenant
 from .errors import BaseError, NotFoundError, EqualIndividualError
+from .importer.backend import find_import_identities_backends
 from .log import TransactionsLog
 from .models import (Individual,
                      AffiliationRecommendation,
                      MergeRecommendation,
                      GenderRecommendation)
 from .recommendations.engine import RecommendationEngine
 
@@ -69,22 +72,31 @@
         raise NotFoundError(entity=job_id)
 
     logger.debug(f"Job with id {job_id} was found")
 
     return jobs[0]
 
 
-def get_jobs():
+def get_jobs(tenant=None):
     """Get a list of all jobs
 
     This function returns a list of all jobs found in the main queue and its
-    registries, sorted by date.
+    registries, sorted by date. If a tenant is specified, filter the jobs for
+    that tenant.
+
+    :param tenant: filter the jobs for a specific tenant
 
     :returns: a list of Job instances
     """
+    def job_in_tenant(job, tenant):
+        ctx = job.kwargs.get('ctx')
+        if not ctx:
+            ctx = job.args[0]
+        return tenant == ctx.tenant
+
     logger.debug("Retrieving list of jobs ...")
 
     queue = django_rq.get_queue()
     started_jobs = [find_job(id)
                     for id
                     in queue.started_job_registry.get_job_ids()]
     deferred_jobs = [find_job(id)
@@ -96,23 +108,26 @@
     failed_jobs = [find_job(id)
                    for id
                    in queue.failed_job_registry.get_job_ids()]
     scheduled_jobs = [find_job(id)
                       for id
                       in queue.scheduled_job_registry.get_job_ids()]
     jobs = (queue.jobs + started_jobs + deferred_jobs + finished_jobs + failed_jobs + scheduled_jobs)
+    if tenant:
+        jobs = (job for job in jobs if job_in_tenant(job, tenant))
 
-    sorted_jobs = sorted(jobs, key=lambda x: x.enqueued_at)
+    sorted_jobs = sorted(jobs, key=lambda x: x.enqueued_at if x.enqueued_at else datetime.datetime.utcnow())
 
     logger.debug(f"List of jobs retrieved; total jobs: {len(sorted_jobs)};")
 
     return sorted_jobs
 
 
 @django_rq.job
+@job_using_tenant
 def recommend_affiliations(ctx, uuids=None):
     """Generate a list of affiliation recommendations from a set of individuals.
 
     This function generates a list of recommendations which include the
     organizations where individuals can be affiliated.
     This job returns a dictionary with which individuals are recommended to be
     affiliated to which organization.
@@ -141,15 +156,15 @@
         'results': results
     }
 
     engine = RecommendationEngine()
 
     # Create a new context to include the reference
     # to the job id that will perform the transaction.
-    job_ctx = SortingHatContext(ctx.user, job.id)
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
 
     # Create an empty transaction to log which job
     # will generate the enroll transactions.
     trxl = TransactionsLog.open('recommend_affiliations', job_ctx)
 
     for chunk in _iter_split(uuids, size=MAX_CHUNK_SIZE):
         for rec in engine.recommend('affiliation', chunk):
@@ -174,14 +189,15 @@
         f"{len(results)} recommendations generated"
     )
 
     return job_result
 
 
 @django_rq.job
+@job_using_tenant
 def recommend_matches(ctx, source_uuids, target_uuids, criteria, exclude=True, verbose=False):
     """Generate a list of affiliation recommendations from a set of individuals.
 
     This function generates a list of recommendations which include the
     matching identities from the individuals which can be merged with.
     This job returns a dictionary with which individuals are recommended to be
     merged to which individual (or which identities is `verbose` mode is activated).
@@ -217,15 +233,15 @@
         'results': results
     }
 
     engine = RecommendationEngine()
 
     # Create a new context to include the reference
     # to the job id that will perform the transaction.
-    job_ctx = SortingHatContext(ctx.user, job.id)
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
 
     trxl = TransactionsLog.open('recommend_matches', job_ctx)
 
     for rec in engine.recommend('matches', source_uuids, target_uuids, criteria, exclude, verbose):
         results[rec.key] = list(rec.options)
         # Store matches in the database
         for match in rec.options:
@@ -247,14 +263,15 @@
         f"{len(results)} recommendations generated"
     )
 
     return job_result
 
 
 @django_rq.job
+@job_using_tenant
 def recommend_gender(ctx, uuids, exclude=True, no_strict_matching=False):
     """Generate a list of gender recommendations from a set of individuals.
 
     This job generates a list of recommendations with the
     probable gender of the given individuals.
 
     :param ctx: context where this job is run
@@ -274,15 +291,15 @@
     results = {}
     job_result = {
         'results': results
     }
 
     engine = RecommendationEngine()
 
-    job_ctx = SortingHatContext(ctx.user, job.id)
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
 
     trxl = TransactionsLog.open('recommend_gender', job_ctx)
 
     for rec in engine.recommend('gender', uuids, exclude, no_strict_matching):
         gender, accuracy = rec.options[0], rec.options[1]
         results[rec.key] = {'gender': gender,
                             'accuracy': accuracy}
@@ -309,14 +326,15 @@
         f"{len(results)} recommendations generated"
     )
 
     return job_result
 
 
 @django_rq.job
+@job_using_tenant
 def affiliate(ctx, uuids=None):
     """Affiliate a set of individuals using recommendations.
 
     This function automates the affiliation process obtaining
     a list of recommendations where individuals can be
     affiliated. After that, individuals are enrolled to them.
     This job returns a dictionary with which individuals were
@@ -348,15 +366,15 @@
         'errors': errors
     }
 
     engine = RecommendationEngine()
 
     # Create a new context to include the reference
     # to the job id that will perform the transaction.
-    job_ctx = SortingHatContext(ctx.user, job.id)
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
 
     # Create an empty transaction to log which job
     # will generate the enroll transactions.
     trxl = TransactionsLog.open('affiliate', job_ctx)
 
     nsuccess = 0
 
@@ -376,14 +394,15 @@
         f"{nsuccess} individuals have new affiliations"
     )
 
     return job_result
 
 
 @django_rq.job
+@job_using_tenant
 def unify(ctx, source_uuids, target_uuids, criteria, exclude=True):
     """Unify a set of individuals by merging them using matching recommendations.
 
     This function automates the identities unify process obtaining
     a list of recommendations where matching individuals can be merged.
     After that, matching individuals are merged.
     This job returns a list with the individuals which have been merged
@@ -441,15 +460,15 @@
         'errors': errors
     }
 
     engine = RecommendationEngine()
 
     # Create a new context to include the reference
     # to the job id that will perform the transaction.
-    job_ctx = SortingHatContext(ctx.user, job.id)
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
 
     trxl = TransactionsLog.open('unify', job_ctx)
 
     match_recs = {}
     for rec in engine.recommend('matches', source_uuids, target_uuids, criteria, exclude=exclude):
         match_recs[rec.key] = list(rec.options)
 
@@ -471,14 +490,15 @@
         f"{len(results)} individuals have been merged"
     )
 
     return job_result
 
 
 @django_rq.job
+@job_using_tenant
 def genderize(ctx, uuids=None, exclude=True, no_strict_matching=False):
     """Assign a gender to a set of individuals using recommendations.
 
     This job autocompletes the gender information (stored in
     the profile) of unique identities after obtaining a list
     of recommendations for their gender based on their name.
 
@@ -512,15 +532,15 @@
         'errors': errors
     }
 
     engine = RecommendationEngine()
 
     # Create a new context to include the reference
     # to the job id that will perform the transaction.
-    job_ctx = SortingHatContext(ctx.user, job.id)
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
 
     # Create an empty transaction to log which job
     # will generate the enroll transactions.
     trxl = TransactionsLog.open('autogender', job_ctx)
 
     nsuccess = 0
 
@@ -540,14 +560,58 @@
         f"Job {job.id} 'genderize' completed; "
         f"{nsuccess} individuals have been updated"
     )
 
     return job_result
 
 
+@django_rq.job
+@job_using_tenant
+def import_identities(ctx, backend_name, url, params):
+    """Import identities to SortingHat.
+
+    This job imports identities to SortingHat using the
+    data obtained from the URL using the specified backend.
+
+    :param ctx: context where this job is run
+    :param backend_name: name of the importer backend
+    :param url: URL of a file or API to fetch the identities from
+    :param params: specific arguments for the importer backend
+
+    :returns: number of identities imported
+    """
+    job = rq.get_current_job()
+
+    logger.info(f"Running job {job.id} 'import_identities'; "
+                f"backend='{backend_name}'; url='{url}'")
+
+    backends = find_import_identities_backends()
+    klass = backends[backend_name]['class']
+
+    if not params:
+        params = {}
+
+    # Create a new context to include the reference
+    # to the job id that will perform the transaction.
+    job_ctx = SortingHatContext(ctx.user, job.id, ctx.tenant)
+    trxl = TransactionsLog.open('import_identities', job_ctx)
+
+    importer = klass(ctx=job_ctx, url=url, **params)
+    nidentities = importer.import_identities()
+
+    trxl.close()
+
+    logger.info(
+        f"Job {job.id} 'import_identities' completed; "
+        f"{nidentities} identities imported"
+    )
+
+    return nidentities
+
+
 def _merge_individuals(job_ctx, source_indv, target_indvs):
     """Merge a set of individuals.
 
     Returns a tuple with two elements: list of the uuids from
     the individuals who were merged; list of errors found
     during the process.
```

### Comparing `sortinghat-0.8.1/sortinghat/core/log.py` & `sortinghat-0.9.0rc1/sortinghat/core/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,24 +102,25 @@
         if not isinstance(ctx.user, AnonymousUser):
             username = ctx.user.username
             validate_field('username', username)
 
         trx = Transaction(tuid=tuid,
                           name=trx_name,
                           created_at=datetime_utcnow(),
-                          authored_by=username)
+                          authored_by=username,
+                          tenant=ctx.tenant)
 
         try:
             trx.save(force_insert=True)
         except django.db.utils.IntegrityError as exc:
             _handle_integrity_error(Transaction, exc, tuid)
 
         logger.debug(
             f"Transaction {trx.tuid} started; "
-            f"name='{trx.name}' author='{trx.authored_by}'"
+            f"name='{trx.name}' author='{trx.authored_by}' tenant='{ctx.tenant}'"
         )
 
         return cls(trx, ctx)
 
     def close(self):
         """Close a given transaction adding a timestamp as closing date and setting a flag"""
```

### Comparing `sortinghat-0.8.1/sortinghat/core/management/commands/create_groups.py` & `sortinghat-0.9.0rc1/sortinghat/core/management/commands/create_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #
 
 import logging
 
 from django.core.management import BaseCommand
 from django.contrib.auth.models import Group, Permission
 from django.contrib.contenttypes.models import ContentType
+from django.db import DEFAULT_DB_ALIAS
 
 logger = logging.getLogger(__name__)
 
 SORTINGHAT_PERMISSION_GROUPS = {
     "admin": {
         "admin": {
             "logentry": ["add", "change", "delete", "view"]
@@ -61,30 +62,37 @@
     }
 }
 
 
 class Command(BaseCommand):
     help = "Create groups with the chosen permissions"
 
+    def add_arguments(self, parser):
+        parser.add_argument(
+            '--database',
+            default=DEFAULT_DB_ALIAS,
+            help='Specifies the database to use. Default is "default".',
+        )
+
     def handle(self, *args, **options):
         for group_name, content_types in SORTINGHAT_PERMISSION_GROUPS.items():
-            new_group, created = Group.objects.get_or_create(name=group_name)
+            new_group, created = Group.objects.using(options['database']).get_or_create(name=group_name)
 
             for app_label, models in content_types.items():
                 for model, permissions in models.items():
                     try:
-                        content_type = ContentType.objects.get(app_label=app_label,
-                                                               model=model)
+                        content_type = ContentType.objects.using(options['database'])\
+                                                          .get(app_label=app_label, model=model)
                         for permission_name in permissions:
                             codename = f"{permission_name}_{model}"
                             if model == "custompermissions":
                                 codename = permission_name
                             try:
-                                permission = Permission.objects.get(codename=codename,
-                                                                    content_type=content_type)
+                                permission = Permission.objects.using(options['database'])\
+                                                               .get(codename=codename, content_type=content_type)
                                 new_group.permissions.add(permission)
                             except Permission.DoesNotExist:
                                 logger.warning(f"Permission {permission_name} not found")
                                 continue
                     except ContentType.DoesNotExist:
                         logger.warning(f"ContentType {model} not found in {app_label}")
                         continue
```

### Comparing `sortinghat-0.8.1/sortinghat/core/migrations/0001_sortinghat.py` & `sortinghat-0.9.0rc1/sortinghat/core/migrations/0001_sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/models.py` & `sortinghat-0.9.0rc1/sortinghat/core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                               CharField,
                               DateTimeField,
                               PositiveIntegerField,
                               ForeignKey,
                               OneToOneField)
 
 from django.db.models import JSONField
+from django.conf import settings
 
 from enum import Enum
 
 from grimoirelab_toolkit.datetime import datetime_utcnow
 
 from treebeard.mp_tree import MP_Node, MP_NodeQuerySet
 
@@ -91,14 +92,16 @@
                      primary_key=True)
     name = CharField(max_length=MAX_SIZE_CHAR_FIELD)
     created_at = DateTimeField()
     closed_at = DateTimeField(null=True)
     is_closed = BooleanField(default=False)
     authored_by = CharField(max_length=MAX_SIZE_CHAR_FIELD,
                             null=True)
+    tenant = CharField(max_length=MAX_SIZE_CHAR_FIELD,
+                       null=True)
 
     class Meta:
         db_table = 'transactions'
         ordering = ('created_at', 'tuid')
 
     def __str__(self):
         return '%s - %s' % (self.tuid, self.name)
@@ -341,7 +344,37 @@
 
     class Meta:
         db_table = 'gender_recommendations'
         unique_together = ('individual',)
 
     def __str__(self):
         return '%s - %s - %s' % (self.individual, self.gender, self.accuracy)
+
+
+class ImportIdentitiesTask(EntityBase):
+    backend = CharField(max_length=MAX_SIZE_CHAR_FIELD)
+    url = CharField(max_length=MAX_SIZE_CHAR_FIELD)
+    interval = PositiveIntegerField(null=True, default=None)
+    args = JSONField(null=True, default=None)
+    job_id = CharField(max_length=MAX_SIZE_CHAR_FIELD, null=True, default=None)
+    scheduled_datetime = DateTimeField(null=True, default=None)
+    last_execution = DateTimeField(null=True, default=None)
+    failed = BooleanField(default=False)
+    failures = PositiveIntegerField(default=0)
+    executions = PositiveIntegerField(default=0)
+
+    class Meta:
+        db_table = 'import_identities_task'
+        unique_together = ('backend', 'url')
+
+    def __str__(self):
+        return '%s - %s' % (self.backend, self.url)
+
+
+class Tenant(EntityBase):
+    user = ForeignKey(settings.AUTH_USER_MODEL, on_delete=CASCADE)
+    host = CharField(max_length=MAX_SIZE_CHAR_FIELD)
+    database = CharField(max_length=MAX_SIZE_CHAR_FIELD)
+
+    class Meta:
+        db_table = 'tenants'
+        unique_together = ('user', 'host')
```

### Comparing `sortinghat-0.8.1/sortinghat/core/recommendations/__init__.py` & `sortinghat-0.9.0rc1/sortinghat/core/recommendations/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/recommendations/affiliation.py` & `sortinghat-0.9.0rc1/sortinghat/core/recommendations/affiliation.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/recommendations/engine.py` & `sortinghat-0.9.0rc1/sortinghat/core/recommendations/engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/recommendations/exclusion.py` & `sortinghat-0.9.0rc1/sortinghat/core/recommendations/exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/recommendations/gender.py` & `sortinghat-0.9.0rc1/sortinghat/core/recommendations/gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/recommendations/matching.py` & `sortinghat-0.9.0rc1/sortinghat/core/recommendations/matching.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/core/schema.py` & `sortinghat-0.9.0rc1/sortinghat/core/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,37 +16,39 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
+import datetime
 import json
 import re
 
 import graphene
 import graphql_jwt
 
 from django.conf import settings
 from django.core.paginator import Paginator
 from django.db.models import Q, Subquery
 
-from django.db.models import JSONField
+from django.db.models import (JSONField, Count)
 
 from django_rq import enqueue
 
 from graphene.types.generic import GenericScalar
 from graphene.utils.str_converters import to_snake_case
 
 from graphene_django.converter import convert_django_field
 from graphene_django.types import DjangoObjectType
 
 from grimoirelab_toolkit.datetime import (str_to_datetime,
                                           InvalidDateError)
 
+from .tenant import get_db_tenant
 from .api import (add_identity,
                   delete_identity,
                   update_profile,
                   move_identity,
                   lock,
                   unlock,
                   merge,
@@ -55,18 +57,22 @@
                   add_team,
                   add_domain,
                   delete_organization,
                   delete_team,
                   delete_domain,
                   enroll,
                   withdraw,
-                  update_enrollment)
+                  update_enrollment,
+                  delete_import_identities_task,
+                  update_import_identities_task)
 from .context import SortingHatContext
 from .decorators import (check_auth, check_permissions)
 from .errors import InvalidFilterError, EqualIndividualError
+from .importer.backend import find_import_identities_backends
+from .importer.base import create_import_task, schedule_import_task
 from .jobs import (affiliate,
                    unify,
                    find_job,
                    get_jobs,
                    recommend_affiliations,
                    recommend_matches,
                    recommend_gender,
@@ -81,18 +87,22 @@
                      Profile,
                      Enrollment,
                      Transaction,
                      Operation,
                      RecommenderExclusionTerm,
                      AffiliationRecommendation,
                      MergeRecommendation,
-                     GenderRecommendation)
+                     GenderRecommendation,
+                     ImportIdentitiesTask)
 from .recommendations.exclusion import delete_recommend_exclusion_term, add_recommender_exclusion_term
 
 
+DEFAULT_IMPORT_IDENTITIES_INTERVAL = 60 * 24 * 7  # minutes
+
+
 @convert_django_field.register(JSONField)
 def convert_json_field_to_generic_scalar(field, registry=None):
     """Convert the content of a `JSONField` loading it as an object"""
 
     return OperationArgsType(description=field.help_text, required=not field.null)
 
 
@@ -157,15 +167,16 @@
     total_results = graphene.Int(description='Total number of items.')
 
 
 class OperationArgsType(GenericScalar):
     @classmethod
     def serialize(cls, value):
         value = super().serialize(value)
-        value = json.loads(value)
+        if not isinstance(value, dict):
+            value = json.loads(value)
         return value
 
 
 class OperationType(DjangoObjectType):
     class Meta:
         model = Operation
 
@@ -281,14 +292,19 @@
 
 
 class RecommenderExclusionTermType(DjangoObjectType):
     class Meta:
         model = RecommenderExclusionTerm
 
 
+class ImportIdentitiesTaskType(DjangoObjectType):
+    class Meta:
+        model = ImportIdentitiesTask
+
+
 class AffiliationResultType(graphene.ObjectType):
     uuid = graphene.String(description='The unique identifier of an individual.')
     organizations = graphene.List(
         graphene.String,
         description='List of organizations an individual was affiliated to using matching recommendations.'
     )
 
@@ -321,14 +337,19 @@
     job_type = graphene.String(description='Type of job.')
     status = graphene.String(description='Job status (`started`, `deferred`, `finished`, `failed` or `scheduled`).')
     result = graphene.List(JobResultType, description='List of job results.')
     errors = graphene.List(graphene.String, description='List of errors.')
     enqueued_at = graphene.DateTime(description='Time the job was enqueued at.')
 
 
+class IdentitiesImporterType(graphene.ObjectType):
+    name = graphene.String(description='Identities importer name.')
+    args = graphene.List(graphene.String, description='List of available arguments.')
+
+
 class ProfileInputType(graphene.InputObjectType):
     name = graphene.String(required=False, description='Name of the individual.')
     email = graphene.String(required=False, description='Email address of the individual.')
     gender = graphene.String(required=False, description='Gender of the individual.')
     gender_acc = graphene.Int(
         required=False,
         description='Gender accuracy (range of 1 to 100; by default, set to 100).'
@@ -336,14 +357,21 @@
     is_bot = graphene.Boolean(required=False, description='Whether an individual is a bot or not.')
     country_code = graphene.String(
         required=False,
         description='ISO-3166 country code. Examples: `DK` for Denmark, `IT` for Italy.'
     )
 
 
+class ImportIdentitiesTaskInputType(graphene.InputObjectType):
+    backend = graphene.String(required=False, description='Name of the importer backend.')
+    url = graphene.String(required=False, description='URL of a file or API to fetch the identities from.')
+    interval = graphene.Int(required=False, description="Period of executions, in minutes. '0' to disable.")
+    params = graphene.JSONString(required=False, description="Specific parameters for the importer backend.")
+
+
 class CountryFilterType(graphene.InputObjectType):
     code = graphene.String(
         required=False,
         description='Filter countries with an ISO Alpha 2 country code. Examples: `DK` for Denmark, `IT` for Italy.'
     )
     term = graphene.String(
         required=False,
@@ -510,14 +538,21 @@
 class RecommendationFilterType(graphene.InputObjectType):
     is_applied = graphene.Boolean(
         required=False,
         description='Filter recommendations by their status.'
     )
 
 
+class ImporterTasksFilterType(graphene.InputObjectType):
+    backend = graphene.String(
+        required=False,
+        description='Name of the backend importer of identities.'
+    )
+
+
 class AbstractPaginatedType(graphene.ObjectType):
 
     @classmethod
     def create_paginated_result(cls, query, page=1,
                                 page_size=settings.SORTINGHAT_API_PAGE_SIZE):
         paginator = Paginator(query, page_size)
         result = paginator.page(page)
@@ -589,24 +624,30 @@
 
 
 class RecommendedGenderPaginatedType(AbstractPaginatedType):
     entities = graphene.List(RecommendedGenderType, description='A list of gender recommendations from individuals.')
     page_info = graphene.Field(PaginationType, description='Information to aid in pagination.')
 
 
+class ImportIdentitiesTaskPaginatedType(AbstractPaginatedType):
+    entities = graphene.List(ImportIdentitiesTaskType, description='A list of tasks importing identities.')
+    page_info = graphene.Field(PaginationType, description='Information to aid in pagination.')
+
+
 class AddOrganization(graphene.Mutation):
     class Arguments:
         name = graphene.String()
 
     organization = graphene.Field(lambda: OrganizationType)
 
     @check_auth
     def mutate(self, info, name):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         org = add_organization(ctx, name)
 
         return AddOrganization(
             organization=org
         )
 
@@ -616,15 +657,16 @@
         name = graphene.String()
 
     organization = graphene.Field(lambda: OrganizationType)
 
     @check_auth
     def mutate(self, info, name):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         org = delete_organization(ctx, name)
 
         return DeleteOrganization(
             organization=org
         )
 
@@ -636,15 +678,16 @@
         parent_name = graphene.String()
 
     team = graphene.Field(lambda: TeamType)
 
     @check_auth
     def mutate(self, info, team_name, organization=None, parent_name=None):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         team = add_team(ctx, team_name, organization, parent_name)
 
         return AddTeam(
             team=team
         )
 
@@ -655,15 +698,16 @@
         organization = graphene.String()
 
     team = graphene.Field(lambda: TeamType)
 
     @check_auth
     def mutate(self, info, team_name, organization=None):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         team = delete_team(ctx, team_name, organization)
 
         return DeleteTeam(
             team=team
         )
 
@@ -675,15 +719,16 @@
         is_top_domain = graphene.Boolean()
 
     domain = graphene.Field(lambda: DomainType)
 
     @check_auth
     def mutate(self, info, organization, domain, is_top_domain=False):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         dom = add_domain(ctx,
                          organization,
                          domain,
                          is_top_domain=is_top_domain)
 
         return AddDomain(
@@ -696,15 +741,16 @@
         domain = graphene.String()
 
     domain = graphene.Field(lambda: DomainType)
 
     @check_auth
     def mutate(self, info, domain):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         dom = delete_domain(ctx, domain)
 
         return DeleteDomain(
             domain=dom
         )
 
@@ -721,15 +767,16 @@
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, source,
                name=None, email=None, username=None,
                uuid=None):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         identity = add_identity(ctx,
                                 source,
                                 name=name,
                                 email=email,
                                 username=username,
                                 uuid=uuid)
@@ -747,15 +794,16 @@
 
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, uuid):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = delete_identity(ctx, uuid)
 
         return DeleteIdentity(
             uuid=uuid,
             individual=individual
         )
@@ -767,15 +815,16 @@
 
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, uuid):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = lock(ctx, uuid)
 
         return Lock(
             uuid=uuid,
             individual=individual
         )
@@ -787,15 +836,16 @@
 
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, uuid):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = unlock(ctx, uuid)
 
         return Unlock(
             uuid=uuid,
             individual=individual
         )
@@ -808,15 +858,16 @@
 
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, uuid, data):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = update_profile(ctx, uuid, **data)
 
         return UpdateProfile(
             uuid=individual.mk,
             individual=individual
         )
@@ -829,15 +880,16 @@
 
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, from_uuid, to_uuid):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = move_identity(ctx, from_uuid, to_uuid)
 
         return MoveIdentity(
             uuid=individual.mk,
             individual=individual
         )
@@ -850,15 +902,16 @@
 
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, from_uuids, to_uuid):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = merge(ctx, from_uuids, to_uuid)
 
         return Merge(
             uuid=individual.mk,
             individual=individual
         )
@@ -870,15 +923,16 @@
 
     uuids = graphene.Field(lambda: graphene.List(graphene.String))
     individuals = graphene.Field(lambda: graphene.List(IndividualType))
 
     @check_auth
     def mutate(self, info, uuids):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individuals = unmerge_identities(ctx, uuids)
         uuids = [individual.mk for individual in individuals]
 
         return UnmergeIdentities(
             uuids=uuids,
             individuals=individuals
@@ -899,15 +953,16 @@
 
     @check_auth
     def mutate(self, info, uuid, group,
                parent_org=None,
                from_date=None, to_date=None,
                force=False):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = enroll(ctx, uuid, group, parent_org=parent_org,
                             from_date=from_date, to_date=to_date,
                             force=force)
         return Enroll(
             uuid=individual.mk,
             individual=individual
@@ -925,15 +980,16 @@
     uuid = graphene.Field(lambda: graphene.String)
     individual = graphene.Field(lambda: IndividualType)
 
     @check_auth
     def mutate(self, info, uuid, group, parent_org=None,
                from_date=None, to_date=None):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = withdraw(ctx, uuid, group, parent_org=parent_org,
                               from_date=from_date, to_date=to_date)
         return Withdraw(
             uuid=individual.mk,
             individual=individual
         )
@@ -955,15 +1011,16 @@
 
     @check_auth
     def mutate(self, info, uuid, group,
                from_date, to_date,
                new_from_date=None, new_to_date=None,
                parent_org=None, force=True):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         individual = update_enrollment(ctx, uuid, group,
                                        parent_org=parent_org,
                                        from_date=from_date,
                                        to_date=to_date,
                                        new_from_date=new_from_date,
                                        new_to_date=new_to_date,
@@ -981,15 +1038,16 @@
 
     job_id = graphene.Field(lambda: graphene.String)
 
     @check_permissions('core.execute_job')
     @check_auth
     def mutate(self, info, uuids=None):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = enqueue(recommend_affiliations, ctx, uuids)
 
         return RecommendAffiliations(
             job_id=job.id
         )
 
@@ -1006,15 +1064,16 @@
 
     job_id = graphene.Field(lambda: graphene.String)
 
     @check_permissions('core.execute_job')
     @check_auth
     def mutate(self, info, criteria, source_uuids=None, target_uuids=None, exclude=True, verbose=False):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = enqueue(recommend_matches, ctx, source_uuids, target_uuids, criteria, exclude, verbose)
 
         return RecommendMatches(
             job_id=job.id
         )
 
@@ -1027,15 +1086,16 @@
 
     job_id = graphene.Field(lambda: graphene.String)
 
     @check_permissions('core.execute_job')
     @check_auth
     def mutate(self, info, uuids=None, exclude=True, no_strict_matching=False):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = enqueue(recommend_gender, ctx, uuids, exclude, no_strict_matching)
 
         return RecommendGender(
             job_id=job.id
         )
 
@@ -1047,15 +1107,16 @@
 
     job_id = graphene.Field(lambda: graphene.String)
 
     @check_permissions('core.execute_job')
     @check_auth
     def mutate(self, info, uuids=None):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = enqueue(affiliate, ctx, uuids)
 
         return Affiliate(
             job_id=job.id
         )
 
@@ -1071,15 +1132,16 @@
 
     job_id = graphene.Field(lambda: graphene.String)
 
     @check_permissions('core.execute_job')
     @check_auth
     def mutate(self, info, criteria, source_uuids=None, target_uuids=None, exclude=True):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = enqueue(unify, ctx, source_uuids, target_uuids, criteria, exclude)
 
         return Unify(
             job_id=job.id
         )
 
@@ -1092,15 +1154,16 @@
 
     job_id = graphene.Field(lambda: graphene.String)
 
     @check_permissions('core.execute_job')
     @check_auth
     def mutate(self, info, uuids=None, exclude=True, no_strict_matching=False):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = enqueue(genderize, ctx, uuids, exclude, no_strict_matching)
 
         return Genderize(
             job_id=job.id
         )
 
@@ -1110,15 +1173,16 @@
         term = graphene.String()
 
     exclusion = graphene.Field(lambda: RecommenderExclusionTermType)
 
     @check_auth
     def mutate(self, info, term):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         rel = add_recommender_exclusion_term(ctx, term)
 
         return AddRecommenderExclusionTerm(
             exclusion=rel
         )
 
@@ -1128,15 +1192,16 @@
         term = graphene.String()
 
     exclusion = graphene.Field(lambda: RecommenderExclusionTermType)
 
     @check_auth
     def mutate(self, info, term):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         rel = delete_recommend_exclusion_term(ctx, term)
 
         return DeleteRecommenderExclusionTerm(
             exclusion=rel
         )
 
@@ -1147,15 +1212,16 @@
         apply = graphene.Boolean()
 
     applied = graphene.Boolean()
 
     @check_auth
     def mutate(self, info, recommendation_id, apply):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         recommendation = MergeRecommendation.objects.get(id=int(recommendation_id))
         if apply:
             try:
                 merge(ctx, [recommendation.individual2.mk], recommendation.individual1.mk)
             except EqualIndividualError:
                 pass
@@ -1176,15 +1242,16 @@
         apply = graphene.Boolean()
 
     applied = graphene.Boolean()
 
     @check_auth
     def mutate(self, info, recommendation_id, apply):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         recommendation = AffiliationRecommendation.objects.get(id=int(recommendation_id))
         if apply:
             enroll(ctx, recommendation.individual.mk, recommendation.organization.name)
 
         recommendation.applied = apply
         recommendation.save()
@@ -1200,15 +1267,16 @@
         apply = graphene.Boolean()
 
     applied = graphene.Boolean()
 
     @check_auth
     def mutate(self, info, recommendation_id, apply):
         user = info.context.user
-        ctx = SortingHatContext(user)
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
 
         recommendation = GenderRecommendation.objects.get(id=int(recommendation_id))
 
         if apply:
             update_profile(ctx,
                            recommendation.individual.mk,
                            gender=recommendation.gender,
@@ -1218,14 +1286,97 @@
         recommendation.save()
 
         return ManageGenderRecommendation(
             applied=apply
         )
 
 
+class AddImportIdentitiesTask(graphene.Mutation):
+    class Arguments:
+        backend = graphene.String()
+        url = graphene.String()
+        interval = graphene.Int(required=False)
+        params = graphene.JSONString(required=False)
+
+    task = graphene.Field(lambda: ImportIdentitiesTaskType)
+
+    @check_auth
+    def mutate(self, info, backend, url, interval=DEFAULT_IMPORT_IDENTITIES_INTERVAL, params=None):
+        user = info.context.user
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
+
+        task = create_import_task(ctx, backend, url, interval, params)
+
+        return AddImportIdentitiesTask(
+            task=task
+        )
+
+
+class DeleteImportIdentitiesTask(graphene.Mutation):
+    class Arguments:
+        task_id = graphene.Int()
+
+    deleted = graphene.Boolean()
+
+    @check_auth
+    def mutate(self, info, task_id):
+        user = info.context.user
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
+
+        task = delete_import_identities_task(ctx, task_id)
+
+        if task.job_id:
+            job = find_job(task.job_id)
+            if job:
+                job.cancel()
+
+        return DeleteImportIdentitiesTask(
+            deleted=True
+        )
+
+
+class UpdateImportIdentitiesTask(graphene.Mutation):
+    class Arguments:
+        task_id = graphene.Int()
+        data = ImportIdentitiesTaskInputType()
+
+    task = graphene.Field(lambda: ImportIdentitiesTaskType)
+
+    @check_auth
+    def mutate(self, info, task_id, data):
+        user = info.context.user
+        tenant = get_db_tenant()
+        ctx = SortingHatContext(user=user, tenant=tenant)
+
+        task = update_import_identities_task(ctx, task_id, **data)
+
+        # Update next execution time if the interval is updated
+        if 'interval' in data:
+            new_dt = datetime.datetime.now(datetime.timezone.utc) \
+                + datetime.timedelta(minutes=task.interval)
+            if task.scheduled_datetime and task.scheduled_datetime > new_dt:
+                find_job(task.job_id)
+                if task.job_id:
+                    job = find_job(task.job_id)
+                    if job:
+                        job.cancel()
+                schedule_import_task(ctx, task, new_dt)
+
+        # If the task is updated, and is not scheduled,
+        # force a new execution.
+        if not task.scheduled_datetime:
+            schedule_import_task(ctx, task)
+
+        return UpdateImportIdentitiesTask(
+            task=task
+        )
+
+
 class SortingHatQuery:
 
     countries = graphene.Field(
         CountryPaginatedType,
         page_size=graphene.Int(),
         page=graphene.Int(),
         filters=CountryFilterType(required=False),
@@ -1308,14 +1459,25 @@
     recommended_gender = graphene.Field(
         RecommendedGenderPaginatedType,
         page_size=graphene.Int(),
         page=graphene.Int(),
         filters=RecommendationFilterType(required=False),
         description='Get all gender recommendations for the identities.'
     )
+    import_identities_task = graphene.Field(
+        ImportIdentitiesTaskPaginatedType,
+        page_size=graphene.Int(),
+        page=graphene.Int(),
+        filters=ImporterTasksFilterType(required=False),
+        description='Get all import identities tasks.'
+    )
+    identities_importers_types = graphene.List(
+        IdentitiesImporterType,
+        description='Get the available identities importers.'
+    )
 
     @check_auth
     def resolve_countries(self, info, filters=None,
                           page=1,
                           page_size=settings.SORTINGHAT_API_PAGE_SIZE):
         query = Country.objects.order_by('code')
 
@@ -1388,15 +1550,15 @@
 
     @check_auth
     def resolve_individuals(self, info, filters=None,
                             page=1,
                             page_size=settings.SORTINGHAT_API_PAGE_SIZE,
                             order_by='mk',
                             **kwargs):
-        query = Individual.objects.order_by(to_snake_case(order_by))
+        query = Individual.objects.annotate(identities_count=Count('identities')).order_by(to_snake_case(order_by))
 
         if filters and 'uuid' in filters:
             indv_uuid = filters['uuid']
             # Search among all the individuals and their identities
             query = query.filter(mk__in=Subquery(Identity.objects
                                                  .filter(Q(uuid=indv_uuid) |
                                                          Q(individual__mk=indv_uuid))
@@ -1557,15 +1719,16 @@
                        status=status,
                        result=result,
                        errors=errors,
                        enqueued_at=enqueued_at)
 
     @check_auth
     def resolve_jobs(self, info, page=1, page_size=settings.SORTINGHAT_API_PAGE_SIZE):
-        jobs = get_jobs()
+        tenant = get_db_tenant()
+        jobs = get_jobs(tenant)
         result = []
 
         for job in jobs:
             job_id = job.get_id()
             status = job.get_status()
             job_type = job.func_name.split('.')[-1]
             enqueued_at = job.enqueued_at
@@ -1677,14 +1840,40 @@
 
         query = query.order_by('created_at')
 
         return RecommendedGenderPaginatedType.create_paginated_result(query,
                                                                       page,
                                                                       page_size=page_size)
 
+    @check_auth
+    def resolve_import_identities_task(self, info, filters=None, page=1,
+                                       page_size=settings.SORTINGHAT_API_PAGE_SIZE, **kwargs):
+
+        query = ImportIdentitiesTask.objects.order_by('created_at')
+
+        if filters and 'backend' in filters:
+            query.filter(backend=filters['backend'])
+
+        return ImportIdentitiesTaskPaginatedType.create_paginated_result(query,
+                                                                         page,
+                                                                         page_size=page_size)
+
+    @check_auth
+    def resolve_identities_importers_types(self, info, **kwargs):
+        result = []
+
+        backends = find_import_identities_backends()
+        for name, backend in backends.items():
+            result.append({
+                'name': name,
+                'args': backend['args']
+            })
+
+        return result
+
 
 class SortingHatMutation(graphene.ObjectType):
     add_organization = AddOrganization.Field(
         description='Add an organization to the registry.'
     )
     delete_organization = DeleteOrganization.Field(
         description='Remove an organization from the registry. Related information\
@@ -1783,14 +1972,23 @@
     )
     manage_affiliation_recommendation = ManageAffiliationRecommendation.Field(
         description='Manage an affiliation recommendation for an identity.'
     )
     manage_gender_recommendation = ManageGenderRecommendation.Field(
         description='Manage a gender recommendation.'
     )
+    add_import_identities_task = AddImportIdentitiesTask.Field(
+        description='Create a periodic task to import identities.'
+    )
+    delete_import_identities_task = DeleteImportIdentitiesTask.Field(
+        description='Delete a periodic task to import identities.'
+    )
+    update_import_identities_task = UpdateImportIdentitiesTask.Field(
+        description='Update a periodic task to import identities.'
+    )
 
     # JWT authentication
     token_auth = graphql_jwt.ObtainJSONWebToken.Field()
     verify_token = graphql_jwt.Verify.Field(description='Verify a JSON Web Token.')
     refresh_token = graphql_jwt.Refresh.Field(description='Refresh a JSON Web Token.')
```

### Comparing `sortinghat-0.8.1/sortinghat/core/views.py` & `sortinghat-0.9.0rc1/sortinghat/core/views.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/server/sortinghat_admin.py` & `sortinghat-0.9.0rc1/sortinghat/server/sortinghat_admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,23 +15,28 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
+import getpass
 import logging
 import os
+import sys
 
 import click
 
 import importlib_resources
 
+from django.contrib.auth import get_user_model
 from django.core.wsgi import get_wsgi_application
-from django.core import management
+from django.core import management, exceptions
+from django.db import IntegrityError
+from django.conf import settings
 
 
 logger = logging.getLogger('main')
 
 
 @click.group()
 @click.option('--config', envvar='SORTINGHAT_CONFIG',
@@ -75,14 +80,33 @@
     'SORTINGHAT_SUPERUSER_USERNAME' and 'SORTINGHAT_SUPERUSER_PASSWORD'.
     It the flag 'no-interactive' was given, these environment
     variables are mandatory.
     """
     _setup(no_interactive=no_interactive, only_ui=only_ui)
 
 
+@click.command()
+@click.argument('username')
+@click.argument('host')
+@click.argument('tenant')
+def set_user_tenant(username, host, tenant):
+    """Assign a user and host to a specific tenant"""
+
+    from sortinghat.core.models import Tenant
+
+    try:
+        user = get_user_model().objects.get(username=username)
+    except exceptions.ObjectDoesNotExist:
+        raise click.ClickException(f"User '{username}' does not exist.")
+
+    Tenant.objects.update_or_create(user=user, host=host,
+                                    defaults={'database': tenant})
+    click.echo(f"User '{username}' at '{host}' assigned to '{tenant}'")
+
+
 def _setup(no_interactive, only_ui):
     env = os.environ
     env_vars = False
 
     if 'SORTINGHAT_SUPERUSER_USERNAME' in env:
         env_vars = True
     if 'SORTINGHAT_SUPERUSER_PASSWORD' in env:
@@ -110,18 +134,20 @@
 
     _install_static_files()
 
     if only_ui:
         click.secho("SortingHat UI deployed. Exiting.", fg='bright_cyan')
         return
 
-    _create_database()
-    _setup_database()
-    _setup_database_superuser(no_interactive)
-    _setup_group_permissions()
+    for database in settings.DATABASES:
+        _create_database(database=database)
+        _setup_database(database=database)
+        if database == 'default':
+            _setup_database_superuser(no_interactive, database=database)
+            _setup_group_permissions(database=database)
 
     click.secho("\nSortingHat configuration completed", fg='bright_cyan')
 
 
 @click.command()
 @click.option('--no-database', is_flag=True, default=False,
               help="Do not update the database.")
@@ -133,29 +159,29 @@
     migrations or load pre-defined data.
     """
     click.secho("Upgrading SortingHat service...\n", fg='bright_cyan')
 
     update_database = not no_database
 
     if update_database:
-        _setup_database()
+        for database in settings.DATABASES:
+            _setup_database(database=database)
 
     _install_static_files()
 
     click.secho("SortingHat upgrade completed", fg='bright_cyan')
 
 
 @click.command()
 @click.option('--no-interactive', is_flag=True, default=False,
               help="Run the command in no interactive mode.")
 def migrate_old_database(no_interactive):
     """Migrate SortingHat 0.7 database schema to 0.8 and all the data"""
 
     import MySQLdb
-    from django.conf import settings
     from .utils.create_sh_0_7_fixture import create_sh_fixture
 
     def _database_table_exists(db_params, table):
         try:
             MySQLdb.connect(
                 user=db_params['USER'],
                 password=db_params['PASSWORD'],
@@ -185,107 +211,162 @@
                 cursor.execute(
                     f"RENAME TABLE {from_db}.{table} TO {to_db}.{table};"
                 )
         except MySQLdb.DatabaseError as exc:
             msg = f"Error in backup database '{from_db}': {exc}."
             raise click.ClickException(msg)
 
-    db_params = settings.DATABASES['default']
+    for database in settings.DATABASES:
+        db_params = settings.DATABASES[database]
 
-    if not _database_table_exists(db_params, 'matching_blacklist'):
-        click.echo("SortingHat database schema is >= 0.8. Done.")
-        return
+        if not _database_table_exists(db_params, 'matching_blacklist'):
+            click.echo("SortingHat database schema is >= 0.8. Done.")
+            return
+
+        click.secho("Migrate 0.7.X SortingHat database schema ...", fg='bright_cyan')
+
+        backup_db_name = f"{db_params['NAME']}_backup"
+
+        with open('/tmp/sortinghat_0_7_fixture.json', 'w') as output_fh:
+            create_sh_fixture(db_host=db_params['HOST'],
+                              db_port=int(db_params['PORT']),
+                              db_user=db_params['USER'],
+                              db_password=db_params['PASSWORD'],
+                              database=db_params['NAME'],
+                              output_fh=output_fh)
+
+        _create_database(database=database, db_name=backup_db_name)
+        _backup_tables(db_params, db_params['NAME'], backup_db_name)
+        _setup(no_interactive, False)
+        management.call_command('loaddata', '/tmp/sortinghat_0_7_fixture.json', database=database)
 
-    click.secho("Migrate 0.7.X SortingHat database schema ...", fg='bright_cyan')
+    click.echo("Migration completed!")
 
-    backup_db_name = f"{db_params['NAME']}_backup"
 
-    with open('/tmp/sortinghat_0_7_fixture.json', 'w') as output_fh:
-        create_sh_fixture(db_host=db_params['HOST'],
-                          db_port=int(db_params['PORT']),
-                          db_user=db_params['USER'],
-                          db_password=db_params['PASSWORD'],
-                          database=db_params['NAME'],
-                          output_fh=output_fh)
-
-    _create_database(backup_db_name)
-    _backup_tables(db_params, db_params['NAME'], backup_db_name)
-    _setup(no_interactive, False)
-    management.call_command('loaddata', '/tmp/sortinghat_0_7_fixture.json')
+@click.command()
+@click.option('--username', help="Specifies the login for the user.")
+@click.option('--is-admin', is_flag=True, default=False,
+              help="Specifies if the user is superuser.")
+@click.option('--no-interactive', is_flag=True, default=False,
+              help="Run the command in no interactive mode.")
+def create_user(username, is_admin, no_interactive):
+    """Create a new user given a username and password"""
 
-    click.echo("Migration completed!")
+    try:
+        if no_interactive:
+            # Use password from environment variable, if provided.
+            password = os.environ.get('SORTINGHAT_USER_PASSWORD')
+            if not password or not password.strip():
+                raise click.ClickException("Password cannot be empty.")
+            # Use username from environment variable, if not provided in options.
+            if username is None:
+                username = os.environ.get('SORTINGHAT_USER_USERNAME')
+            error = _validate_username(username)
+            if error:
+                click.ClickException(error)
+        else:
+            # Get username
+            if username is None:
+                username = input("Username: ")
+            error = _validate_username(username)
+            if error:
+                click.ClickException(error)
+            # Prompt for a password
+            password = getpass.getpass()
+            password2 = getpass.getpass('Password (again): ')
+            if password != password2:
+                raise click.ClickException("Error: Your passwords didn't match.")
+            if password.strip() == '':
+                raise click.ClickException("Error: Blank passwords aren't allowed.")
+
+        extra_fields = {}
+        if is_admin:
+            extra_fields['is_staff'] = True
+            extra_fields['is_superuser'] = True
+
+        get_user_model().objects.create_user(username=username,
+                                             password=password,
+                                             **extra_fields)
+
+        click.echo("User created successfully.")
+    except KeyboardInterrupt:
+        click.echo("\nOperation cancelled.")
+        sys.exit(1)
+    except IntegrityError:
+        click.echo(f"User '{username}' already exists.")
+        sys.exit(1)
 
 
-def _create_database(db_name=None):
+def _create_database(database='default', db_name=None):
     """Create an empty database."""
 
     import MySQLdb
-    from django.conf import settings
 
-    db_params = settings.DATABASES['default']
-    database = db_name if db_name else db_params['NAME']
+    db_params = settings.DATABASES[database]
+    db_name = db_name if db_name else db_params['NAME']
 
     click.secho("## SortingHat database creation\n", fg='bright_cyan')
 
     try:
         cursor = MySQLdb.connect(
             user=db_params['USER'],
             password=db_params['PASSWORD'],
             host=db_params['HOST'],
             port=int(db_params['PORT'])
         ).cursor()
         cursor.execute(
-            f"CREATE DATABASE IF NOT EXISTS {database} "
+            f"CREATE DATABASE IF NOT EXISTS {db_name} "
             "CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_520_ci;"
         )
     except MySQLdb.DatabaseError as exc:
-        msg = f"Error creating database '{database}': {exc}."
+        msg = f"Error creating database '{db_name}' for '{database}': {exc}."
         raise click.ClickException(msg)
 
-    click.echo(f"SortingHat database '{database}' created.\n")
+    click.echo(f"SortingHat database '{db_name}' for '{database}' created.\n")
 
 
-def _setup_database():
+def _setup_database(database='default'):
     """Apply migrations and fixtures to the database."""
 
-    click.secho("## SortingHat database setup\n", fg='bright_cyan')
+    click.secho(f"## SortingHat database setup for {database}\n", fg='bright_cyan')
 
-    management.call_command('migrate')
+    management.call_command('migrate', database=database)
 
     with importlib_resources.path('sortinghat.core.fixtures', 'countries.json') as p:
         fixture_countries_path = p
 
-    management.call_command('loaddata', fixture_countries_path)
+    management.call_command('loaddata', fixture_countries_path, database=database)
 
     click.echo()
 
 
-def _setup_database_superuser(no_interactive=False):
+def _setup_database_superuser(no_interactive=False, database='default'):
     """Create database superuser."""
 
-    click.secho("## SortingHat superuser configuration\n", fg='bright_cyan')
+    click.secho(f"## SortingHat superuser configuration for {database}\n", fg='bright_cyan')
 
     env = os.environ
     kwargs = {}
 
     if no_interactive:
         env['DJANGO_SUPERUSER_USERNAME'] = env['SORTINGHAT_SUPERUSER_USERNAME']
         env['DJANGO_SUPERUSER_PASSWORD'] = env['SORTINGHAT_SUPERUSER_PASSWORD']
         env['DJANGO_SUPERUSER_EMAIL'] = 'noreply@localhost'
         kwargs['interactive'] = False
 
+    kwargs['database'] = database
     management.call_command('createsuperuser', **kwargs)
 
 
-def _setup_group_permissions():
+def _setup_group_permissions(database='default'):
     """Create permission groups."""
 
-    click.secho("## SortingHat groups creation\n", fg='bright_cyan')
+    click.secho(f"## SortingHat groups creation for {database}\n", fg='bright_cyan')
 
-    management.call_command('create_groups')
+    management.call_command('create_groups', database=database)
 
     click.echo("SortingHat groups created.\n")
 
 
 def _install_static_files():
     """Collect static files and installed them."""
 
@@ -294,10 +375,24 @@
 
     management.call_command('collectstatic', clear=True,
                             interactive=False)
 
     click.echo()
 
 
+def _validate_username(username):
+    """Check if the username is valid and return the error"""
+
+    if not username:
+        return "Username cannot be empty."
+    username_field = get_user_model()._meta.get_field(get_user_model().USERNAME_FIELD)
+    try:
+        username_field.clean(username, None)
+    except exceptions.ValidationError as e:
+        return '; '.join(e.messages)
+
+
 sortinghat_admin.add_command(setup)
 sortinghat_admin.add_command(upgrade)
 sortinghat_admin.add_command(migrate_old_database)
+sortinghat_admin.add_command(create_user)
+sortinghat_admin.add_command(set_user_tenant)
```

### Comparing `sortinghat-0.8.1/sortinghat/server/sortinghatd.py` & `sortinghat-0.9.0rc1/sortinghat/server/sortinghatd.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/server/sortinghatw.py` & `sortinghat-0.9.0rc1/sortinghat/server/sortinghatw.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,10 +58,10 @@
             "Set it with '--config' option "
             "or 'SORTINGHAT_CONFIG' env variable."
         )
 
     _ = get_wsgi_application()
 
     try:
-        management.call_command('rqworker', *queues)
+        management.call_command('rqworker', *queues, with_scheduler=True)
     except KeyError as e:
         raise click.ClickException(f"Queue '{e.args[0]}' not found")
```

### Comparing `sortinghat-0.8.1/sortinghat/server/utils/create_sh_0_7_fixture.py` & `sortinghat-0.9.0rc1/sortinghat/server/utils/create_sh_0_7_fixture.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/sortinghat/utils/__init__.py` & `sortinghat-0.9.0rc1/sortinghat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_add.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_config.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_countries.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_enroll.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_lock.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_merge.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_mv.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_orgs.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_profile.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_rm.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_show.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_split.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/cli/test_cmd_withdraw.py` & `sortinghat-0.9.0rc1/tests/cli/test_cmd_withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/rec/test_affiliations.py` & `sortinghat-0.9.0rc1/tests/rec/test_affiliations.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/rec/test_engine.py` & `sortinghat-0.9.0rc1/tests/rec/test_engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/rec/test_exclusion.py` & `sortinghat-0.9.0rc1/tests/rec/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/rec/test_gender.py` & `sortinghat-0.9.0rc1/tests/rec/test_gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/rec/test_matches.py` & `sortinghat-0.9.0rc1/tests/rec/test_matches.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/test_api.py` & `sortinghat-0.9.0rc1/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,16 @@
                                     Individual,
                                     Identity,
                                     Enrollment,
                                     Organization,
                                     Team,
                                     Domain,
                                     Transaction,
-                                    Operation)
+                                    Operation,
+                                    ImportIdentitiesTask)
 
 NOT_FOUND_ERROR = "{entity} not found in the registry"
 ENROLLMENT_RANGE_INVALID = "range date '{start}'-'{end}' is part of an existing range for {org}"
 ALREADY_EXISTS_ERROR = "{entity} already exists in the registry"
 SOURCE_NONE_OR_EMPTY_ERROR = "'source' cannot be"
 IDENTITY_NONE_OR_EMPTY_ERROR = "identity data cannot be empty"
 UUID_NONE_OR_EMPTY_ERROR = "'uuid' cannot be"
@@ -82,14 +83,16 @@
 TEAM_ORG_NAME_MISSING = "'org_name' cannot be"
 TEAM_NAME_MISSING = "'team_name' cannot be"
 DOMAIN_NAME_NONE_OR_EMPTY_ERROR = "'domain_name' cannot be"
 DOMAIN_NOT_FOUND_ERROR = "{domain_name} not found in the registry"
 DOMAIN_ALREADY_EXISTS_ERROR = "'{domain_name}' already exists in the registry"
 DOMAIN_VALUE_ERROR = "field value must be a string; int given"
 DOMAIN_ORG_NAME_NONE_OR_EMPTY_ERROR = "'org_name' cannot be"
+FORMAT_NONE_OR_EMPTY_ERROR = "'{}' cannot be"
+INTERVAL_MUST_BE_NUMBER_ERROR = "'interval' must be a positive number"
 
 
 class TestAddIdentity(TestCase):
     """Unit tests for add_identity"""
 
     def setUp(self):
         """Load initial values"""
@@ -5701,7 +5704,303 @@
         self.assertEqual(op3.trx, trx)
         self.assertGreater(op3.timestamp, timestamp)
 
         op3_args = json.loads(op3.args)
         self.assertEqual(len(op3_args), 2)
         self.assertEqual(op3_args['identity'], '67fc4f8a56aa12ab981d2a4c1de065bb9936c9f6')
         self.assertEqual(op3_args['individual'], '67fc4f8a56aa12ab981d2a4c1de065bb9936c9f6')
+
+
+class TestDeleteImportTask(TestCase):
+    """Unit tests for delete_import_identities_task"""
+
+    def setUp(self):
+        """Load initial dataset"""
+
+        self.user = get_user_model().objects.create(username='test')
+        self.ctx = SortingHatContext(self.user)
+
+        self.task_foo = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+        self.task_bar = ImportIdentitiesTask.objects.create(backend='bar', url='bar.url', interval=1)
+        self.task_baz = ImportIdentitiesTask.objects.create(backend='baz', url='baz.url', interval=2)
+
+    def test_delete_task(self):
+        """Check whether it deletes a task"""
+
+        # Check initial status
+        tasks = ImportIdentitiesTask.objects.all()
+        self.assertEqual(len(tasks), 3)
+
+        # Delete a task
+        api.delete_import_identities_task(self.ctx, self.task_foo.id)
+
+        # Check result
+        tasks = ImportIdentitiesTask.objects.filter(url='foo.url')
+        self.assertEqual(len(tasks), 0)
+
+        # Check remaining tasks
+        tasks = ImportIdentitiesTask.objects.all()
+        self.assertEqual(len(tasks), 2)
+
+        with self.assertRaises(ObjectDoesNotExist):
+            ImportIdentitiesTask.objects.get(id=self.task_foo.id)
+
+    def test_non_existing_task_id(self):
+        """Check if it fails removing a task that does not exists"""
+
+        trx_date = datetime_utcnow()  # After this datetime no transactions should be created
+
+        with self.assertRaises(NotFoundError):
+            api.delete_import_identities_task(self.ctx, 999)
+
+        # It should raise an error when the registry is empty
+        ImportIdentitiesTask.objects.all().delete()
+        self.assertEqual(len(ImportIdentitiesTask.objects.all()), 0)
+
+        with self.assertRaises(NotFoundError):
+            api.delete_import_identities_task(self.ctx, 1)
+
+        # Check if there are no transactions created when there is an error
+        transactions = Transaction.objects.filter(created_at__gt=trx_date)
+        self.assertEqual(len(transactions), 0)
+
+    def test_none_task_id(self):
+        """Check whether tasks cannot be removed when giving a None id"""
+
+        trx_date = datetime_utcnow()  # After this datetime no transactions should be created
+
+        with self.assertRaisesRegex(InvalidValueError, FORMAT_NONE_OR_EMPTY_ERROR.format('task_id')):
+            api.delete_import_identities_task(self.ctx, None)
+
+        # Check if there are no transactions created when there is an error
+        transactions = Transaction.objects.filter(created_at__gt=trx_date)
+        self.assertEqual(len(transactions), 0)
+
+    def test_empty_task_id(self):
+        """Check whether tasks cannot be removed when giving an empty id"""
+
+        trx_date = datetime_utcnow()  # After this datetime no transactions should be created
+
+        with self.assertRaisesRegex(InvalidValueError, FORMAT_NONE_OR_EMPTY_ERROR.format('task_id')):
+            api.delete_import_identities_task(self.ctx, '')
+
+        # Check if there are no transactions created when there is an error
+        transactions = Transaction.objects.filter(created_at__gt=trx_date)
+        self.assertEqual(len(transactions), 0)
+
+    def test_transaction(self):
+        """Check if a transaction is created when deleting a task"""
+
+        timestamp = datetime_utcnow()
+
+        api.delete_import_identities_task(self.ctx, self.task_foo.id)
+
+        transactions = Transaction.objects.filter(created_at__gte=timestamp)
+        self.assertEqual(len(transactions), 1)
+
+        trx = transactions[0]
+        self.assertIsInstance(trx, Transaction)
+        self.assertEqual(trx.name, 'delete_import_task')
+        self.assertGreater(trx.created_at, timestamp)
+        self.assertEqual(trx.authored_by, self.ctx.user.username)
+
+    def test_operations(self):
+        """Check if the right operations are created when deleting a task"""
+
+        timestamp = datetime_utcnow()
+
+        api.delete_import_identities_task(self.ctx, self.task_foo.id)
+
+        transactions = Transaction.objects.filter(created_at__gte=timestamp)
+        trx = transactions[0]
+
+        operations = Operation.objects.filter(trx=trx)
+        self.assertEqual(len(operations), 1)
+
+        op1 = operations[0]
+        self.assertIsInstance(op1, Operation)
+        self.assertEqual(op1.op_type, Operation.OpType.DELETE.value)
+        self.assertEqual(op1.entity_type, 'import_task')
+        self.assertEqual(op1.trx, trx)
+        self.assertEqual(op1.target, str(self.task_foo.id))
+        self.assertGreater(op1.timestamp, timestamp)
+
+        op1_args = json.loads(op1.args)
+        self.assertEqual(len(op1_args), 1)
+        self.assertEqual(op1_args['task'], str(self.task_foo.id))
+
+
+class TestUpdateImportTask(TestCase):
+    """Unit tests for update_import_identities_task"""
+
+    def setUp(self):
+        """Load initial dataset"""
+
+        self.user = get_user_model().objects.create(username='test')
+        self.ctx = SortingHatContext(self.user)
+
+        self.task_foo = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url')
+        self.task_bar = ImportIdentitiesTask.objects.create(backend='bar', url='bar.url', interval=1)
+        self.task_baz = ImportIdentitiesTask.objects.create(backend='baz', url='baz.url', interval=2)
+
+    def test_update_import_task(self):
+        """Check if it updates a task"""
+
+        task = api.update_import_identities_task(self.ctx,
+                                                 self.task_foo.id,
+                                                 backend='foo2',
+                                                 url='foo2.url',
+                                                 interval=4,
+                                                 params={'token': '1234'})
+        # Tests
+        self.assertIsInstance(task, ImportIdentitiesTask)
+
+        self.assertEqual(task.backend, 'foo2')
+        self.assertEqual(task.url, 'foo2.url')
+        self.assertEqual(task.interval, 4)
+        self.assertDictEqual(task.args, {'token': '1234'})
+
+        # Check database object
+        task_db = ImportIdentitiesTask.objects.get(id=task.id)
+        self.assertEqual(task, task_db)
+
+    def test_update_task_only_interval(self):
+        """Check if it updates a task"""
+
+        task = api.update_import_identities_task(self.ctx,
+                                                 self.task_foo.id,
+                                                 interval=4)
+        # Tests
+        self.assertIsInstance(task, ImportIdentitiesTask)
+
+        self.assertEqual(task.backend, 'foo')
+        self.assertEqual(task.url, 'foo.url')
+        self.assertEqual(task.interval, 4)
+        self.assertIsNone(task.args)
+
+        # Check database object
+        task_db = ImportIdentitiesTask.objects.get(id=task.id)
+        self.assertEqual(task, task_db)
+
+    def test_last_modified(self):
+        """Check if last modification date is updated"""
+
+        before_dt = datetime_utcnow()
+        task = api.update_import_identities_task(self.ctx,
+                                                 self.task_foo.id,
+                                                 interval=4)
+        after_dt = datetime_utcnow()
+
+        self.assertLessEqual(before_dt, task.last_modified)
+        self.assertGreaterEqual(after_dt, task.last_modified)
+
+    def test_non_existing_task(self):
+        """Check if it fails updating a task that does not exist"""
+
+        with self.assertRaises(NotFoundError):
+            api.update_import_identities_task(self.ctx,
+                                              999,
+                                              interval=4)
+
+        # Check if there are no transactions created when there is an error
+        transactions = Transaction.objects.all()
+        self.assertEqual(len(transactions), 0)
+
+    def test_invalid_backend(self):
+        """Check that empty backend is not valid"""
+
+        with self.assertRaisesRegex(InvalidValueError, FORMAT_NONE_OR_EMPTY_ERROR.format('backend')):
+            api.update_import_identities_task(self.ctx,
+                                              self.task_foo.id,
+                                              backend='')
+        with self.assertRaisesRegex(InvalidValueError, FORMAT_NONE_OR_EMPTY_ERROR.format('backend')):
+            api.update_import_identities_task(self.ctx,
+                                              self.task_foo.id,
+                                              backend=None)
+
+            # Check if there are no transactions created when there is an error
+            transactions = Transaction.objects.all()
+            self.assertEqual(len(transactions), 0)
+
+    def test_invalid_url(self):
+        """Check that empty url is not valid"""
+
+        with self.assertRaisesRegex(InvalidValueError, FORMAT_NONE_OR_EMPTY_ERROR.format('url')):
+            api.update_import_identities_task(self.ctx,
+                                              self.task_foo.id,
+                                              url='')
+        with self.assertRaisesRegex(InvalidValueError, FORMAT_NONE_OR_EMPTY_ERROR.format('url')):
+            api.update_import_identities_task(self.ctx,
+                                              self.task_foo.id,
+                                              url=None)
+
+            # Check if there are no transactions created when there is an error
+            transactions = Transaction.objects.all()
+            self.assertEqual(len(transactions), 0)
+
+    def test_invalid_interval(self):
+        """Check wrong interval is not valid"""
+
+        with self.assertRaisesRegex(InvalidValueError, INTERVAL_MUST_BE_NUMBER_ERROR):
+            api.update_import_identities_task(self.ctx,
+                                              self.task_foo.id,
+                                              interval='5')
+        with self.assertRaisesRegex(InvalidValueError, INTERVAL_MUST_BE_NUMBER_ERROR):
+            api.update_import_identities_task(self.ctx,
+                                              self.task_foo.id,
+                                              interval=-1)
+
+            # Check if there are no transactions created when there is an error
+            transactions = Transaction.objects.all()
+            self.assertEqual(len(transactions), 0)
+
+    def test_transaction(self):
+        """Check if a transaction is created when updating a task"""
+
+        timestamp = datetime_utcnow()
+
+        api.update_import_identities_task(self.ctx,
+                                          self.task_foo.id,
+                                          interval=60)
+
+        transactions = Transaction.objects.filter(created_at__gte=timestamp)
+        self.assertEqual(len(transactions), 1)
+
+        trx = transactions[0]
+        self.assertIsInstance(trx, Transaction)
+        self.assertEqual(trx.name, 'update_import_task')
+        self.assertGreater(trx.created_at, timestamp)
+        self.assertEqual(trx.authored_by, self.ctx.user.username)
+
+    def test_operations(self):
+        """Check if the right operations are created when updating a task"""
+
+        timestamp = datetime_utcnow()
+
+        task = api.update_import_identities_task(self.ctx,
+                                                 self.task_foo.id,
+                                                 backend='foo2',
+                                                 url='foo2.url',
+                                                 interval=4,
+                                                 params={'token': '1234'})
+
+        transactions = Transaction.objects.filter(created_at__gte=timestamp)
+        trx = transactions[0]
+
+        operations = Operation.objects.filter(trx=trx)
+        self.assertEqual(len(operations), 1)
+
+        op1 = operations[0]
+        self.assertIsInstance(op1, Operation)
+        self.assertEqual(op1.op_type, Operation.OpType.UPDATE.value)
+        self.assertEqual(op1.entity_type, 'import_task')
+        self.assertEqual(op1.target, str(self.task_foo.id))
+        self.assertEqual(op1.trx, trx)
+        self.assertGreater(op1.timestamp, timestamp)
+
+        op1_args = json.loads(op1.args)
+        self.assertEqual(len(op1_args), 5)
+        self.assertEqual(op1_args['task'], str(self.task_foo.id))
+        self.assertEqual(op1_args['backend'], 'foo2')
+        self.assertEqual(op1_args['url'], 'foo2.url')
+        self.assertEqual(op1_args['interval'], 4)
+        self.assertDictEqual(op1_args['params'], {'token': '1234'})
```

### Comparing `sortinghat-0.8.1/tests/test_aux.py` & `sortinghat-0.9.0rc1/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/test_client.py` & `sortinghat-0.9.0rc1/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 
 import logging
 import json
 import unittest
 
 import httpretty
-import sgqlc.endpoint.http
+import sgqlc.endpoint.requests
 
 from sgqlc.operation import Operation
 
 from sortinghat.cli.client import (SortingHatClient,
                                    SortingHatClientError,
                                    SortingHatSchema)
 
@@ -131,15 +131,15 @@
         """Test whether the client establishes a connection with a SortingHat server"""
 
         MockSortingHatServer(SORTINGHAT_SERVER_URL)
 
         client = SortingHatClient('localhost', ssl=False)
         client.connect()
 
-        self.assertIsInstance(client.gqlc, sgqlc.endpoint.http.HTTPEndpoint)
+        self.assertIsInstance(client.gqlc, sgqlc.endpoint.requests.RequestsEndpoint)
 
         latest_requests = httpretty.latest_requests()
         self.assertEqual(len(latest_requests), 1)
 
         request = latest_requests[0]
         self.assertEqual(request.method, 'GET')
 
@@ -182,15 +182,15 @@
         """Test whether the client authenticates on a SortingHat server"""
 
         MockSortingHatServer(SORTINGHAT_SERVER_URL)
 
         client = SortingHatClient('localhost', user='admin', password='admin', ssl=False)
         client.connect()
 
-        self.assertIsInstance(client.gqlc, sgqlc.endpoint.http.HTTPEndpoint)
+        self.assertIsInstance(client.gqlc, sgqlc.endpoint.requests.RequestsEndpoint)
 
         latest_requests = httpretty.latest_requests()
         self.assertEqual(len(latest_requests), 3)
 
         request = latest_requests[0]
         self.assertEqual(request.method, 'GET')
         self.assertEqual(dict(request.headers)['Host'], 'localhost:9314')
```

### Comparing `sortinghat-0.8.1/tests/test_db.py` & `sortinghat-0.9.0rc1/tests/test_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                                     Domain,
                                     Country,
                                     Individual,
                                     Identity,
                                     Profile,
                                     Enrollment,
                                     Transaction,
-                                    Operation)
-
+                                    Operation,
+                                    ImportIdentitiesTask)
 
 DUPLICATED_ORG_ERROR = "Organization 'Example' already exists in the registry"
 DUPLICATED_DOM_ERROR = "Domain 'example.org' already exists in the registry"
 DUPLICATED_TEAM_ERROR = "Team 'error_team' already exists in the registry"
 DUPLICATED_INDIVIDUAL_ERROR = "Individual '1234567890ABCDFE' already exists in the registry"
 DUPLICATED_ID_ERROR = "Identity '1234567890ABCDFE' already exists in the registry"
 DUPLICATED_ID_DATA_ERROR = "Identity 'John Smith-jsmith@example.org-jsmith-scm' already exists in the registry"
@@ -95,14 +95,18 @@
 GENDER_ACC_INVALID_RANGE_ERROR = r"'gender_acc' \({acc}\) is not in range \(1,100\)"
 START_DATE_NONE_ERROR = "'start' date cannot be None"
 END_DATE_NONE_ERROR = "'end' date cannot be None"
 PERIOD_INVALID_ERROR = "'start' date {start} cannot be greater than {end}"
 PERIOD_OUT_OF_BOUNDS_ERROR = "'{type}' date {date} is out of bounds"
 MOVE_ERROR = "identity '0001' is already assigned to 'AAAA'"
 INDIVIDUAL_LOCKED_ERROR = "Individual {mk} is locked"
+INTERVAL_INVALID_ERROR = "'interval' must be a positive number or 0."
+FORMAT_NOT_FOUND_ERROR = "{} not found in the registry"
+FORMAT_EMPTY_ERROR = "'{}' cannot be .+"
+FORMAT_ALREADY_EXISTS = "'{}' already exists in the registry"
 
 
 class TestFindIndividual(TestCase):
     """Unit tests for find_individual"""
 
     def test_find_individual(self):
         """Test if an individual is found by its main key"""
@@ -2653,14 +2657,410 @@
 
         op1_args = json.loads(op1.args)
         self.assertEqual(len(op1_args), 2)
         self.assertEqual(op1_args['identity'], '0001')
         self.assertEqual(op1_args['individual'], 'BBBB')
 
 
+class TestFindImportTask(TestCase):
+    """Unit tests for find_import_identities_task"""
+
+    def test_find_import_task(self):
+        """Test if a task is found by its id"""
+
+        task = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+
+        task_db = db.find_import_identities_task(task.id)
+        self.assertIsInstance(task_db, ImportIdentitiesTask)
+        self.assertEqual(task_db.id, task.id)
+
+    def test_task_not_found(self):
+        """Test whether it raises an exception when the task is not found"""
+
+        with self.assertRaisesRegex(NotFoundError, FORMAT_NOT_FOUND_ERROR.format(999)):
+            db.find_import_identities_task(999)
+
+
+class TestAddImportTask(TestCase):
+    """Unit tests for add_import_identities_task"""
+
+    def setUp(self):
+        """Load initial dataset"""
+
+        self.user = get_user_model().objects.create(username='test')
+        self.ctx = SortingHatContext(self.user)
+        self.trxl = TransactionsLog.open('add_import_task', self.ctx)
+
+    def test_add_import_task(self):
+        """Check if a new task is created"""
+
+        task = db.add_import_identities_task(self.trxl,
+                                             backend='foo_backend',
+                                             url='foo_url',
+                                             interval=1,
+                                             args={})
+
+        self.assertIsInstance(task, ImportIdentitiesTask)
+        self.assertEqual(task.backend, 'foo_backend')
+        self.assertEqual(task.url, 'foo_url')
+        self.assertEqual(task.interval, 1)
+        self.assertEqual(task.args, {})
+
+    def test_add_multiple_import_task(self):
+        """Check if multiple tasks can be added"""
+
+        task1 = db.add_import_identities_task(self.trxl,
+                                              backend='foo_backend',
+                                              url='foo_url',
+                                              interval=1,
+                                              args={})
+        task2 = db.add_import_identities_task(self.trxl,
+                                              backend='bar_backend',
+                                              url='bar_url',
+                                              interval=1,
+                                              args={})
+
+        tasks = ImportIdentitiesTask.objects.all()
+        self.assertEqual(len(tasks), 2)
+
+        task = tasks[0]
+        self.assertIsInstance(task, ImportIdentitiesTask)
+        self.assertEqual(task.backend, 'foo_backend')
+        self.assertEqual(task.url, 'foo_url')
+        self.assertEqual(task.interval, 1)
+        self.assertEqual(task.args, {})
+
+        task = tasks[1]
+        self.assertIsInstance(task, ImportIdentitiesTask)
+        self.assertEqual(task.backend, 'bar_backend')
+        self.assertEqual(task.url, 'bar_url')
+        self.assertEqual(task.interval, 1)
+        self.assertEqual(task.args, {})
+
+    def test_last_modified(self):
+        """Check if last modification date is updated"""
+
+        before_dt = datetime_utcnow()
+        task = db.add_import_identities_task(self.trxl,
+                                             backend='foo_backend',
+                                             url='foo_url',
+                                             interval=1,
+                                             args={})
+        after_dt = datetime_utcnow()
+
+        # Tests
+        self.assertLessEqual(before_dt, task.last_modified)
+        self.assertGreaterEqual(after_dt, task.last_modified)
+
+    def test_task_backend_empty(self):
+        """Check whether a task with empty backend cannot be added"""
+
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('backend')):
+            db.add_import_identities_task(self.trxl,
+                                          backend='',
+                                          url='foo_url',
+                                          interval=1,
+                                          args={})
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('backend')):
+            db.add_import_identities_task(self.trxl,
+                                          backend=None,
+                                          url='foo_url',
+                                          interval=1,
+                                          args={})
+
+        # Check if operations have not been generated after the failure
+        operations = Operation.objects.all()
+        self.assertEqual(len(operations), 0)
+
+    def test_task_url_empty(self):
+        """Check whether a task with empty URL cannot be added"""
+
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('url')):
+            db.add_import_identities_task(self.trxl,
+                                          backend='foo',
+                                          url='',
+                                          interval=1,
+                                          args={})
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('url')):
+            db.add_import_identities_task(self.trxl,
+                                          backend='foo',
+                                          url=None,
+                                          interval=1,
+                                          args={})
+
+        # Check if operations have not been generated after the failure
+        operations = Operation.objects.all()
+        self.assertEqual(len(operations), 0)
+
+    def test_task_invalid_interval(self):
+        """Check whether a task with wrong interval cannot be added"""
+
+        with self.assertRaisesRegex(ValueError, INTERVAL_INVALID_ERROR):
+            db.add_import_identities_task(self.trxl,
+                                          backend='foo',
+                                          url='foo.url',
+                                          interval=-1,
+                                          args={})
+
+        # Check if operations have not been generated after the failure
+        operations = Operation.objects.all()
+        self.assertEqual(len(operations), 0)
+
+    def test_integrity_error(self):
+        """Check whether tasks with the same url and backend cannot be inserted"""
+
+        with self.assertRaisesRegex(AlreadyExistsError, FORMAT_ALREADY_EXISTS.format('foo-foo.url')):
+            db.add_import_identities_task(self.trxl,
+                                          backend='foo',
+                                          url='foo.url',
+                                          interval=1,
+                                          args={})
+            db.add_import_identities_task(self.trxl,
+                                          backend='foo',
+                                          url='foo.url',
+                                          interval=3,
+                                          args={})
+
+    def test_operations(self):
+        """Check if the right operations are created when adding a new task"""
+
+        timestamp = datetime_utcnow()
+        task = db.add_import_identities_task(self.trxl,
+                                             backend='foo',
+                                             url='foo.url',
+                                             interval=1,
+                                             args={})
+        transactions = Transaction.objects.all()
+        trx = transactions[0]
+
+        operations = Operation.objects.filter(trx=trx)
+        self.assertEqual(len(operations), 1)
+
+        op1 = operations[0]
+        self.assertIsInstance(op1, Operation)
+        self.assertEqual(op1.op_type, Operation.OpType.ADD.value)
+        self.assertEqual(op1.entity_type, 'import_task')
+        self.assertGreater(op1.timestamp, timestamp)
+        self.assertEqual(op1.target, task.url)
+        self.assertEqual(op1.trx, trx)
+
+        op1_args = json.loads(op1.args)
+        self.assertEqual(len(op1_args), 5)
+        self.assertEqual(op1_args['backend'], task.backend)
+        self.assertEqual(op1_args['url'], task.url)
+        self.assertEqual(op1_args['interval'], str(task.interval))
+        self.assertEqual(op1_args['args'], str(task.args))
+        self.assertEqual(op1_args['job_id'], task.job_id)
+
+
+class TestDeleteImportTask(TestCase):
+    """Unit tests for delete import task"""
+
+    def setUp(self):
+        """Load initial dataset"""
+
+        self.user = get_user_model().objects.create(username='test')
+        self.ctx = SortingHatContext(self.user)
+
+        self.trxl = TransactionsLog.open('delete_task', self.ctx)
+
+    def test_delete_task(self):
+        """Check whether it deletes an import task"""
+
+        task = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+
+        db.delete_import_identities_task(self.trxl, task)
+
+        # Tests
+        with self.assertRaises(ObjectDoesNotExist):
+            ImportIdentitiesTask.objects.get(id=task.id)
+
+    def test_operations(self):
+        """Check if the right operations are created when deleting a task"""
+
+        # Set the initial dataset
+        timestamp = datetime_utcnow()
+        task = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+        task_id = task.id
+
+        db.delete_import_identities_task(self.trxl, task)
+
+        transactions = Transaction.objects.filter(name='delete_task')
+        trx = transactions[0]
+
+        operations = Operation.objects.filter(trx=trx)
+        self.assertEqual(len(operations), 1)
+
+        op1 = operations[0]
+        self.assertIsInstance(op1, Operation)
+        self.assertEqual(op1.op_type, Operation.OpType.DELETE.value)
+        self.assertEqual(op1.entity_type, 'import_task')
+        self.assertEqual(op1.trx, trx)
+        self.assertEqual(op1.target, str(task_id))
+        self.assertGreater(op1.timestamp, timestamp)
+
+        op1_args = json.loads(op1.args)
+        self.assertEqual(len(op1_args), 1)
+        self.assertEqual(op1_args['task'], str(task_id))
+
+
+class TestUpdateImportTask(TestCase):
+    """Unit tests for update_import_identities_task"""
+
+    def setUp(self):
+        """Load initial dataset"""
+
+        self.user = get_user_model().objects.create(username='test')
+        self.ctx = SortingHatContext(self.user)
+
+        self.trxl = TransactionsLog.open('update_import_task', self.ctx)
+
+        self.task = ImportIdentitiesTask.objects.create(backend='foo',
+                                                        url='foo.url',
+                                                        interval=0)
+
+    def test_update_import_task(self):
+        """Check if it updates a task"""
+
+        task = db.update_import_identities_task(self.trxl,
+                                                self.task,
+                                                backend='foo2',
+                                                url='foo2.url',
+                                                interval=4,
+                                                params={'token': '1234'})
+        # Tests
+        self.assertIsInstance(task, ImportIdentitiesTask)
+        self.assertEqual(task.id, self.task.id)
+        self.assertEqual(task.backend, 'foo2')
+        self.assertEqual(task.url, 'foo2.url')
+        self.assertEqual(task.interval, 4)
+        self.assertDictEqual(task.args, {'token': '1234'})
+
+        # Check database object
+        task_db = ImportIdentitiesTask.objects.get(id=task.id)
+        self.assertEqual(task, task_db)
+
+    def test_update_task_only_interval(self):
+        """Check if it updates a task using only an interval"""
+
+        task = db.update_import_identities_task(self.trxl,
+                                                self.task,
+                                                interval=4)
+        # Tests
+        self.assertIsInstance(task, ImportIdentitiesTask)
+
+        self.assertEqual(task.backend, 'foo')
+        self.assertEqual(task.url, 'foo.url')
+        self.assertEqual(task.interval, 4)
+        self.assertIsNone(task.args)
+
+        # Check database object
+        task_db = ImportIdentitiesTask.objects.get(id=task.id)
+        self.assertEqual(task, task_db)
+
+    def test_invalid_backend(self):
+        """Check that empty backend is not valid"""
+
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('backend')):
+            db.update_import_identities_task(self.trxl,
+                                             self.task,
+                                             backend='')
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('backend')):
+            db.update_import_identities_task(self.trxl,
+                                             self.task,
+                                             backend=None)
+
+            # Check if there are no transactions created when there is an error
+            transactions = Transaction.objects.all()
+            self.assertEqual(len(transactions), 0)
+
+    def test_invalid_url(self):
+        """Check that empty url is not valid"""
+
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('url')):
+            db.update_import_identities_task(self.trxl,
+                                             self.task,
+                                             url='')
+        with self.assertRaisesRegex(ValueError, FORMAT_EMPTY_ERROR.format('url')):
+            db.update_import_identities_task(self.trxl,
+                                             self.task,
+                                             url=None)
+
+            # Check if there are no transactions created when there is an error
+            transactions = Transaction.objects.all()
+            self.assertEqual(len(transactions), 0)
+
+    def test_invalid_interval(self):
+        """Check wrong interval is not valid"""
+
+        with self.assertRaisesRegex(ValueError, INTERVAL_INVALID_ERROR):
+            db.update_import_identities_task(self.trxl,
+                                             self.task,
+                                             interval='5')
+        with self.assertRaisesRegex(ValueError, INTERVAL_INVALID_ERROR):
+            db.update_import_identities_task(self.trxl,
+                                             self.task,
+                                             interval=-1)
+
+            # Check if there are no transactions created when there is an error
+            transactions = Transaction.objects.all()
+            self.assertEqual(len(transactions), 0)
+
+    def test_last_modified(self):
+        """Check if last modification date is updated"""
+
+        before_dt = datetime_utcnow()
+        task = db.update_import_identities_task(self.trxl,
+                                                self.task,
+                                                backend='foo2',
+                                                url='foo2.url',
+                                                interval=4,
+                                                params={'token': '1234'})
+        after_dt = datetime_utcnow()
+
+        # Tests
+        self.assertLessEqual(before_dt, task.last_modified)
+        self.assertGreaterEqual(after_dt, task.last_modified)
+
+    def test_operations(self):
+        """Check if the right operations are created when updating a task"""
+
+        timestamp = datetime_utcnow()
+
+        # Update the task
+        task = db.update_import_identities_task(self.trxl,
+                                                self.task,
+                                                backend='foo2',
+                                                url='foo2.url',
+                                                interval=4,
+                                                params={'token': '1234'})
+
+        transactions = Transaction.objects.filter(name='update_import_task')
+        trx = transactions[0]
+
+        operations = Operation.objects.filter(trx=trx)
+        self.assertEqual(len(operations), 1)
+
+        op1 = operations[0]
+        self.assertIsInstance(op1, Operation)
+        self.assertEqual(op1.op_type, Operation.OpType.UPDATE.value)
+        self.assertEqual(op1.entity_type, 'import_task')
+        self.assertEqual(op1.trx, trx)
+        self.assertEqual(op1.target, str(task.id))
+        self.assertGreater(op1.timestamp, timestamp)
+
+        op1_args = json.loads(op1.args)
+        self.assertEqual(len(op1_args), 5)
+        self.assertEqual(op1_args['backend'], 'foo2')
+        self.assertEqual(op1_args['url'], 'foo2.url')
+        self.assertEqual(op1_args['interval'], 4)
+        self.assertDictEqual(op1_args['params'], {'token': '1234'})
+        self.assertEqual(op1_args['task'], str(task.id))
+
+
 class TestLock(TestCase):
     """Unit tests for lock"""
 
     def setUp(self):
         """Load initial dataset"""
 
         self.user = get_user_model().objects.create(username='test')
```

### Comparing `sortinghat-0.8.1/tests/test_errors.py` & `sortinghat-0.9.0rc1/tests/test_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
 from django.test import TestCase
 
 from sortinghat.core.errors import (BaseError,
                                     AlreadyExistsError,
+                                    InvalidFormatError,
+                                    LoadError,
                                     NotFoundError,
                                     InvalidValueError,
                                     InvalidFilterError,
                                     EqualIndividualError,
                                     ClosedTransactionError,
                                     LockedIdentityError,
                                     DuplicateRangeError,
@@ -105,14 +107,46 @@
     def test_no_args(self):
         """Check when required arguments are not given"""
 
         kwargs = {}
         self.assertRaises(KeyError, AlreadyExistsError, **kwargs)
 
 
+class TestInvalidFormatError(TestCase):
+    """Unit tests for InvalidFormatError"""
+
+    def test_message(self):
+        """Make sure it prints the right error"""
+
+        e = InvalidFormatError(cause="line 30: invalid format")
+        self.assertEqual(str(e), "line 30: invalid format")
+
+    def test_no_args(self):
+        """Check when required arguments are not given"""
+
+        kwargs = {}
+        self.assertRaises(KeyError, InvalidFormatError, **kwargs)
+
+
+class TestLoadError(TestCase):
+    """Unit tests for LoadError"""
+
+    def test_message(self):
+        """Make sure it prints the right error"""
+
+        e = LoadError(cause="Load error message")
+        self.assertEqual(str(e), "Load error message")
+
+    def test_no_args(self):
+        """Check when required arguments are not given"""
+
+        kwargs = {}
+        self.assertRaises(KeyError, LoadError, **kwargs)
+
+
 class TestNotFoundError(TestCase):
     """Unit tests for NotFoundError"""
 
     def test_message(self):
         """Make sure that prints the right error"""
 
         e = NotFoundError(entity='example.com')
```

### Comparing `sortinghat-0.8.1/tests/test_jobs.py` & `sortinghat-0.9.0rc1/tests/test_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,21 +34,23 @@
 from django_rq import enqueue
 
 from grimoirelab_toolkit.datetime import datetime_utcnow
 
 from sortinghat.core import api
 from sortinghat.core.context import SortingHatContext
 from sortinghat.core.errors import DuplicateRangeError, NotFoundError
+from sortinghat.core.importer.backend import IdentitiesImporter
 from sortinghat.core.jobs import (find_job,
                                   affiliate,
                                   unify,
                                   recommend_affiliations,
                                   recommend_matches,
                                   recommend_gender,
-                                  genderize)
+                                  genderize,
+                                  import_identities)
 from sortinghat.core.models import (Individual,
                                     Transaction,
                                     AffiliationRecommendation,
                                     MergeRecommendation,
                                     GenderRecommendation)
 
 JOB_NOT_FOUND_ERROR = "DEF not found in the registry"
@@ -1430,7 +1432,90 @@
         individual_1 = Individual.objects.get(mk=self.jsmith.uuid)
         gender_1 = individual_1.profile.gender
         self.assertEqual(gender_1, 'male')
 
         individual_2 = Individual.objects.get(mk=self.jdoe.uuid)
         gender_2 = individual_2.profile.gender
         self.assertEqual(gender_2, 'female')
+
+
+class MockTestImporter(IdentitiesImporter):
+    NAME = 'test_backend'
+
+    def __init__(self, ctx, url, token=None):
+        super().__init__(ctx, url)
+        self.token = token
+
+    def get_individuals(self):
+        from sortinghat.core.importer.models import Individual, Identity
+        indiv = Individual()
+        indiv.identities.append(Identity(source='test_backend', username='test_user'))
+        return [indiv]
+
+
+class TestImportIdentities(TestCase):
+    """Unit tests for import_identities"""
+
+    def setUp(self):
+        """Initialize database"""
+
+        self.user = get_user_model().objects.create(username='test')
+        self.ctx = SortingHatContext(self.user)
+
+    @unittest.mock.patch('sortinghat.core.importer.backend.find_backends')
+    def test_import_identities(self, mock_find_backends):
+        """Check if the importer is executed correctly"""
+
+        mock_find_backends.return_value = {'test_backend': MockTestImporter}
+
+        # Test
+        ctx = SortingHatContext(self.user)
+
+        job = import_identities.delay(ctx, 'test_backend', 'my_url', None)
+        result = job.result
+
+        self.assertEqual(result, 1)
+
+        # Check individual and identity are inserted
+        indiv = Individual.objects.first()
+        identity = indiv.identities.first()
+        self.assertEqual(identity.source, 'test_backend')
+        self.assertEqual(identity.username, 'test_user')
+
+    @unittest.mock.patch('sortinghat.core.importer.backend.find_backends')
+    def test_backend_not_found(self, mock_find_backends):
+        """Check if the importer is executed correctly"""
+
+        mock_find_backends.return_value = {}
+
+        # Test
+        ctx = SortingHatContext(self.user)
+
+        job = import_identities.delay(ctx, 'test_backend', 'my_url', None)
+        self.assertEqual(job.is_failed, True)
+
+    @unittest.mock.patch('sortinghat.core.importer.backend.find_backends')
+    def test_transactions(self, mock_find_backends):
+        """Check if the right transactions were created"""
+
+        mock_find_backends.return_value = {'test_backend': MockTestImporter}
+
+        timestamp = datetime_utcnow()
+
+        ctx = SortingHatContext(self.user)
+
+        import_identities.delay(ctx, 'test_backend', 'my_url', None,
+                                job_id='ABCD-EF12-3456-7890')
+
+        transactions = Transaction.objects.filter(created_at__gte=timestamp)
+        self.assertEqual(len(transactions), 2)
+
+        trx = transactions[0]
+        self.assertIsInstance(trx, Transaction)
+        self.assertEqual(trx.name, 'import_identities-ABCD-EF12-3456-7890')
+        self.assertGreater(trx.created_at, timestamp)
+        self.assertEqual(trx.authored_by, ctx.user.username)
+        trx = transactions[1]
+        self.assertIsInstance(trx, Transaction)
+        self.assertEqual(trx.name, 'add_identity-ABCD-EF12-3456-7890')
+        self.assertGreater(trx.created_at, timestamp)
+        self.assertEqual(trx.authored_by, ctx.user.username)
```

### Comparing `sortinghat-0.8.1/tests/test_log.py` & `sortinghat-0.9.0rc1/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/tests/test_model.py` & `sortinghat-0.9.0rc1/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #     Miguel Ángel Fernández <mafesan@bitergia.com>
 #
 
 import datetime
 import dateutil
 import json
 
+from django.contrib.auth import get_user_model
 from django.core.exceptions import ValidationError
 from django.db.utils import IntegrityError
 from django.test import TransactionTestCase
 
 from grimoirelab_toolkit.datetime import datetime_utcnow
 
 from sortinghat.core.models import (Organization,
@@ -41,15 +42,17 @@
                                     Profile,
                                     Enrollment,
                                     RecommenderExclusionTerm,
                                     Transaction,
                                     Operation,
                                     AffiliationRecommendation,
                                     MergeRecommendation,
-                                    GenderRecommendation)
+                                    GenderRecommendation,
+                                    ImportIdentitiesTask,
+                                    Tenant)
 
 # Test check errors messages
 DUPLICATE_CHECK_ERROR = "Duplicate entry .+"
 NULL_VALUE_CHECK_ERROR = "Column .+ cannot be null"
 INVALID_BOOLEAN_CHECK_ERROR = "['“true” value must be either True or False.']"
 
 
@@ -927,16 +930,16 @@
 
     def test_last_modified(self):
         """Check last modification date is set when the object is updated"""
 
         before_dt = datetime_utcnow()
         indiv = Individual.objects.create(mk='AAAA')
         gender_re = GenderRecommendation.objects.create(individual=indiv,
-                                                       gender='Male',
-                                                       accuracy=89)
+                                                        gender='Male',
+                                                        accuracy=89)
         after_dt = datetime_utcnow()
 
         self.assertEqual(gender_re.individual, indiv)
         self.assertEqual(gender_re.gender, 'Male')
         self.assertEqual(gender_re.accuracy, 89)
         self.assertGreaterEqual(gender_re.last_modified, before_dt)
         self.assertLessEqual(gender_re.last_modified, after_dt)
@@ -947,14 +950,87 @@
         after_modified_dt = datetime_utcnow()
 
         self.assertEqual(gender_re.individual, indiv)
         self.assertGreaterEqual(gender_re.last_modified, before_modified_dt)
         self.assertLessEqual(gender_re.last_modified, after_modified_dt)
 
 
+class TestImportIdentitiesTask(TransactionTestCase):
+    """Unit tests for ImportIdentitiesTask class"""
+
+    def test_not_null_relationships(self):
+        """Check whether every enrollment is assigned organizations and individuals"""
+
+        with self.assertRaisesRegex(IntegrityError, NULL_VALUE_CHECK_ERROR):
+            Enrollment.objects.create()
+
+        with self.assertRaisesRegex(IntegrityError, NULL_VALUE_CHECK_ERROR):
+            indv = Individual.objects.create(mk='AAAA')
+            Enrollment.objects.create(individual=indv)
+
+        with self.assertRaisesRegex(IntegrityError, NULL_VALUE_CHECK_ERROR):
+            org = Organization.add_root(name='Example')
+            Enrollment.objects.create(group=org)
+
+    def test_unique_tasks(self):
+        """Check if there is only one tuple with the same values"""
+
+        with self.assertRaisesRegex(IntegrityError, DUPLICATE_CHECK_ERROR):
+            ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+            ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=1)
+
+    def test_default_values(self):
+        """Check whether the default values are set when initializing the class"""
+
+        task = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+        self.assertEqual(task.backend, 'foo')
+        self.assertEqual(task.url, 'foo.url')
+        self.assertEqual(task.interval, 0)
+        self.assertEqual(task.args, None)
+        self.assertEqual(task.job_id, None)
+        self.assertEqual(task.scheduled_datetime, None)
+        self.assertEqual(task.last_execution, None)
+        self.assertEqual(task.failures, 0)
+        self.assertEqual(task.executions, 0)
+
+    def test_created_at(self):
+        """Check creation date is only set when the object is created"""
+
+        before_dt = datetime_utcnow()
+        task = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+        after_dt = datetime_utcnow()
+
+        self.assertGreaterEqual(task.created_at, before_dt)
+        self.assertLessEqual(task.created_at, after_dt)
+
+        task.url = 'foo.url2'
+        task.save()
+
+        self.assertGreaterEqual(task.created_at, before_dt)
+        self.assertLessEqual(task.created_at, after_dt)
+
+    def test_last_modified(self):
+        """Check last modification date is set when the object is updated"""
+
+        before_dt = datetime_utcnow()
+        task = ImportIdentitiesTask.objects.create(backend='foo', url='foo.url', interval=0)
+        after_dt = datetime_utcnow()
+
+        self.assertGreaterEqual(task.last_modified, before_dt)
+        self.assertLessEqual(task.last_modified, after_dt)
+
+        before_modified_dt = datetime_utcnow()
+        task.url = 'foo.url2'
+        task.save()
+        after_modified_dt = datetime_utcnow()
+
+        self.assertGreaterEqual(task.last_modified, before_modified_dt)
+        self.assertLessEqual(task.last_modified, after_modified_dt)
+
+
 class TestTransaction(TransactionTestCase):
     """Unit tests for Transaction class"""
 
     def test_unique_transactions(self):
         """Check whether transactions are unique"""
 
         with self.assertRaisesRegex(IntegrityError, DUPLICATE_CHECK_ERROR):
@@ -971,15 +1047,16 @@
     def test_created_at(self):
         """Check creation date is only set when the object is created"""
 
         before_dt = datetime_utcnow()
         trx = Transaction.objects.create(tuid='12345abcd',
                                          name='test',
                                          created_at=datetime_utcnow(),
-                                         authored_by='username')
+                                         authored_by='username',
+                                         tenant='tenant_1')
         after_dt = datetime_utcnow()
 
         self.assertGreaterEqual(trx.created_at, before_dt)
         self.assertLessEqual(trx.created_at, after_dt)
 
         trx.save()
 
@@ -1049,7 +1126,42 @@
 
         trx = Transaction.objects.get(tuid='0123456789abcdef')
 
         with self.assertRaisesRegex(IntegrityError, NULL_VALUE_CHECK_ERROR):
             Operation.objects.create(ouid='12345abcd', op_type=Operation.OpType.ADD,
                                      entity_type='individual', target='test',
                                      timestamp=datetime_utcnow(), args=None, trx=trx)
+
+
+class TestTenant(TransactionTestCase):
+    """Unit tests for Tenant class"""
+
+    def test_unique_tenants(self):
+        """Check whether tenants are unique"""
+
+        with self.assertRaisesRegex(IntegrityError, DUPLICATE_CHECK_ERROR):
+            user = get_user_model().objects.create(username='test')
+            Tenant.objects.create(user=user,
+                                  host='localhost:8000',
+                                  database='tenant_1')
+            Tenant.objects.create(user=user,
+                                  host='localhost:8000',
+                                  database='tenant_2')
+
+    def test_created_at(self):
+        """Check creation date is only set when the object is created"""
+
+        before_dt = datetime_utcnow()
+        user = get_user_model().objects.create(username='test')
+        tenant = Tenant.objects.create(user=user,
+                                       host='localhost:8000',
+                                       database='tenant_2')
+        after_dt = datetime_utcnow()
+
+        self.assertGreaterEqual(tenant.created_at, before_dt)
+        self.assertLessEqual(tenant.created_at, after_dt)
+
+        tenant.save()
+
+        # Check if creation date does not change after saving the object
+        self.assertGreaterEqual(tenant.created_at, before_dt)
+        self.assertLessEqual(tenant.created_at, after_dt)
```

### Comparing `sortinghat-0.8.1/tests/test_schema.py` & `sortinghat-0.9.0rc1/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -3850,14 +3850,72 @@
         indv = individuals[0]
         self.assertEqual(indv['mk'], indv2.mk)
         indv = individuals[1]
         self.assertEqual(indv['mk'], indv3.mk)
         indv = individuals[2]
         self.assertEqual(indv['mk'], indv1.mk)
 
+    def test_order_by_identities_count(self):
+        """Check whether it returns the individuals ordered by their number of identities"""
+
+        indv1 = Individual.objects.create(mk='a9b403e150dd4af8953a52a4bb841051e4b705d9')
+        Identity.objects.create(uuid='A001',
+                                name='John Doe',
+                                source='scm',
+                                individual=indv1)
+        indv2 = Individual.objects.create(mk='185c4b709e5446d250b4fde0e34b78a2b4fde0e3')
+        Identity.objects.create(uuid='B001',
+                                name='Jane Roe',
+                                source='scm',
+                                individual=indv2)
+        Identity.objects.create(uuid='B002',
+                                name='Jane Roe',
+                                source='mls',
+                                individual=indv2)
+        Identity.objects.create(uuid='B003',
+                                name='Jane Roe',
+                                source='alt',
+                                individual=indv2)
+        indv3 = Individual.objects.create(mk='c6d2504fde0e34b78a185c4b709e5442d045451c')
+        Identity.objects.create(uuid='C001',
+                                name='John Smith',
+                                source='scm',
+                                individual=indv3)
+        Identity.objects.create(uuid='C002',
+                                name='John Smith',
+                                source='mls',
+                                individual=indv3)
+
+        # Test ascending order
+        client = graphene.test.Client(schema)
+        executed = client.execute(SH_INDIVIDUALS_ORDER_BY % 'identitiesCount',
+                                  context_value=self.context_value)
+
+        individuals = executed['data']['individuals']['entities']
+
+        indv = individuals[0]
+        self.assertEqual(indv['mk'], indv1.mk)
+        indv = individuals[1]
+        self.assertEqual(indv['mk'], indv3.mk)
+        indv = individuals[2]
+        self.assertEqual(indv['mk'], indv2.mk)
+
+        # Test descending order
+        executed = client.execute(SH_INDIVIDUALS_ORDER_BY % '-identitiesCount',
+                                  context_value=self.context_value)
+
+        individuals = executed['data']['individuals']['entities']
+
+        indv = individuals[0]
+        self.assertEqual(indv['mk'], indv2.mk)
+        indv = individuals[1]
+        self.assertEqual(indv['mk'], indv3.mk)
+        indv = individuals[2]
+        self.assertEqual(indv['mk'], indv1.mk)
+
     def test_pagination(self):
         """Check whether it returns the individuals searched when using pagination"""
 
         indv1 = Individual.objects.create(mk='185c4b709e5446d250b4fde0e34b78a2b4fde0e3')
         indv2 = Individual.objects.create(mk='a9b403e150dd4af8953a52a4bb841051e4b705d9')
         indv3 = Individual.objects.create(mk='c6d2504fde0e34b78a185c4b709e5442d045451c')
```

### Comparing `sortinghat-0.8.1/tests/test_utils.py` & `sortinghat-0.9.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.8.1/PKG-INFO` & `sortinghat-0.9.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat
-Version: 0.8.1
+Version: 0.9.0rc1
 Summary: A tool to manage identities.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,15 @@
 Requires-Dist: mysqlclient (==2.0.3)
 Requires-Dist: numpy (==1.21.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.7.0,<3.0.0)
 Requires-Dist: rq (<1.12.0)
 Requires-Dist: setuptools (>65.5.0)
-Requires-Dist: sgqlc (>=10.1,<11.0)
+Requires-Dist: sgqlc (>=16.1,<17.0)
 Requires-Dist: uWSGI (>=2.0,<3.0)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-sortinghat/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-sortinghat
 Description-Content-Type: text/markdown
 
 # Sorting Hat [![tests](https://github.com/chaoss/grimoirelab-sortinghat/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-sortinghat/actions?query=workflow:tests+branch:master+event:push) [![PyPI version](https://badge.fury.io/py/sortinghat.svg)](https://badge.fury.io/py/sortinghat)
 
@@ -102,15 +102,15 @@
 ```
 $ apt install libmysqlclient-dev
 ```
 
 * **MariaDB**
 
 ```
-$ apt install libmariadbclient-dev
+$ apt install libmariadbclient-dev-compat
 ```
 
 #### Installation and configuration
 
 **Note**: these examples use `sortinghat.config.settings` configuration file.
 In order to use that configuration you need to define the environment variable
 `SORTINGHAT_SECRET_KEY` with a secret. More info here:
@@ -168,15 +168,15 @@
 $ yarn install
 ```
 
 #### Running the frontend
 
 Run SortingHat frontend Vue app:
 ```
-$ yarn serve
+$ yarn serve --api_url=http://localhost:8000/api/
 ```
 
 
 ## SortingHat service
 
 Starting at version 0.8, SortingHat is released with a server app. The server has two
 modes, `production` and `development`.
@@ -195,14 +195,20 @@
 Following examples will make use of that file.
 
 In order to run the service for the first time, you need to execute the next commands:
 
 Build the UI interface:
 ```
 $ cd ui
+$ yarn install
+$ yarn build --mode development
+```
+If you want to run the UI at `/identities` run (you need to use the server 
+behind a proxy server):
+```
 $ yarn build
 ```
 
 Set a secret key:
 ```
 $ export SORTINGHAT_SECRET_KEY="my-secret-key"
 ```
@@ -223,14 +229,29 @@
 
 You will also need to run some workers to execute tasks like recommendations
 or affiliation. To start a worker run the command:
 ```
 $ sortinghatw --config sortinghat.config.settings
 ```
 
+## Create new accounts
+To create new accounts for SortingHat use the following command:
+
+```
+(.venv)$ sortinghat-admin create-user
+
+Usage: sortinghat-admin create-user [OPTIONS]
+
+  Create a new user given a username and password
+
+Options:
+  --username TEXT   Specifies the login for the user.
+  --is-admin        Specifies if the user is superuser.
+  --no-interactive  Run the command in no interactive mode.
+```
 
 ## Compatibility between versions
 SortingHat 0.7.x is no longer supported. Any database using this version will not work.
 
 SortingHat databases 0.7.x are no longer compatible. The `uidentities` table was renamed
 to `individuals`. The database schema changed in all tables to add the fields `created_at`
 and `last_modified`. Also in `domains`, `enrollments`, `identities`, `profiles` tables,
@@ -247,22 +268,43 @@
     * `uuid` to `individual`
 
 Please update your database running the following command:
 ```
 $ sortinghat-admin --config sortinghat.config.settings migrate-old-database
 ```
 
+## Multi-tenancy
+
+SortingHat allows hosting multiple instances with a single service having each
+instance's data isolated in different databases.
+
+To enable this feature follow these guidelines:
+- Set `MULTI_TENANT` settings to `True`.
+- Define a list of tenants using the configuration file `sortinghat/config/tenants.json`. 
+You can use a different json file using the environment variable 
+`SORTINGHAT_MULTI_TENANT_LIST_PATH`
+- Assign users to tenants with the following command:
+  `sortinghat-admin set-user-tenant username host tenant`
+
+There are some limitations:
+- `default` database is only used to store users information and relations between
+users and databases, it won't store anything else related with SortingHat models.
+- Usernames are shared across all instances, which means that it is not possible
+to have the same username with two different passwords in different instances.
+
+
 ## Running tests
 
 SortingHat comes with a comprehensive list of unit tests for both 
 frontend and backend.
 
 #### Backend test suite
 ```
 (.venv)$ ./manage.py test --settings=config.settings.testing
+(.venv)$ ./manage.py test --settings=config.settings.testing_tenant
 ```
 
 #### Frontend test suite
 ```
 $ cd ui/
 $ yarn test:unit
 ```
```

