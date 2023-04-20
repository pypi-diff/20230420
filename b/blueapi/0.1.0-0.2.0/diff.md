# Comparing `tmp/blueapi-0.1.0.tar.gz` & `tmp/blueapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.1.0.tar", last modified: Tue Mar  7 09:29:47 2023, max compression
+gzip compressed data, was "blueapi-0.2.0.tar", last modified: Thu Apr 20 10:06:04 2023, max compression
```

## Comparing `blueapi-0.1.0.tar` & `blueapi-0.2.0.tar`

### file list

```diff
@@ -1,162 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.286486 blueapi-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.266486 blueapi-0.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-07 09:29:36.000000 blueapi-0.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-07 09:29:36.000000 blueapi-0.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.266486 blueapi-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.262486 blueapi-0.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.266486 blueapi-0.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.266486 blueapi-0.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-07 09:29:36.000000 blueapi-0.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-07 09:29:36.000000 blueapi-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-07 09:29:36.000000 blueapi-0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-07 09:29:36.000000 blueapi-0.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-07 09:29:36.000000 blueapi-0.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-07 09:29:36.000000 blueapi-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-07 09:29:36.000000 blueapi-0.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-07 09:29:36.000000 blueapi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-03-07 09:29:47.286486 blueapi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-07 09:29:36.000000 blueapi-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-07 09:29:36.000000 blueapi-0.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/config/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-07 09:29:36.000000 blueapi-0.1.0/config/adsim.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-07 09:29:36.000000 blueapi-0.1.0/config/bl45p.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.270486 blueapi-0.1.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-07 09:29:36.000000 blueapi-0.1.0/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.262486 blueapi-0.1.0/helm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-07 09:29:36.000000 blueapi-0.1.0/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-07 09:29:36.000000 blueapi-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 09:29:47.286486 blueapi-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.262486 blueapi-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.274486 blueapi-0.1.0/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.278486 blueapi-0.1.0/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.278486 blueapi-0.1.0/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.278486 blueapi-0.1.0/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.282486 blueapi-0.1.0/src/blueapi/plans/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/plans/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/plans/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.282486 blueapi-0.1.0/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/service/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/service/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.282486 blueapi-0.1.0/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/startup/adsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/startup/bl45p.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/startup/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.282486 blueapi-0.1.0/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/utils/thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.282486 blueapi-0.1.0/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-07 09:29:36.000000 blueapi-0.1.0/src/blueapi/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.278486 blueapi-0.1.0/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-07 09:29:47.000000 blueapi-0.1.0/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.282486 blueapi-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.286486 blueapi-0.1.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/core/test_device_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.286486 blueapi-0.1.0/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/messaging/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:47.286486 blueapi-0.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-07 09:29:36.000000 blueapi-0.1.0/tests/utils/test_thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.510317 blueapi-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-20 10:05:49.000000 blueapi-0.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-20 10:05:49.000000 blueapi-0.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.474317 blueapi-0.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 10:05:49.000000 blueapi-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-20 10:05:49.000000 blueapi-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 10:05:49.000000 blueapi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-20 10:06:04.510317 blueapi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-20 10:05:49.000000 blueapi-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 10:05:49.000000 blueapi-0.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 10:05:49.000000 blueapi-0.2.0/config/adsim.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 10:05:49.000000 blueapi-0.2.0/config/bl45p.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.486317 blueapi-0.2.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.486317 blueapi-0.2.0/docs/developer/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.486317 blueapi-0.2.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/type_validators.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.478318 blueapi-0.2.0/helm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-20 10:05:49.000000 blueapi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:06:04.510317 blueapi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.478318 blueapi-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/amq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/plans/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/plans/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/service/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/service/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/adsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/bl45p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/type_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/plans/test_scanspec_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.510317 blueapi-0.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_type_validator.py
```

### Comparing `blueapi-0.1.0/.devcontainer/Dockerfile` & `blueapi-0.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.devcontainer/devcontainer.json` & `blueapi-0.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/CONTRIBUTING.rst` & `blueapi-0.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/actions/install_requirements/action.yml` & `blueapi-0.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/dependabot.yml` & `blueapi-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/pages/make_switcher.py` & `blueapi-0.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/workflows/code.yml` & `blueapi-0.2.0/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         install: ["-e .[dev]"]
         # Make one version be non-editable to test both paths of version code
         include:
           - os: "ubuntu-latest"
             python: "3.8"
             install: ".[dev]"
 
+    services:
+      activemq:
+        image: rmohr/activemq:5.14.5-alpine
+        ports:
+          - 61613:61613
+
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
     steps:
       - name: Checkout
```

### Comparing `blueapi-0.1.0/.github/workflows/docs.yml` & `blueapi-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/workflows/docs_clean.yml` & `blueapi-0.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/workflows/helm.yml` & `blueapi-0.2.0/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.github/workflows/linkcheck.yml` & `blueapi-0.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.gitignore` & `blueapi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.pre-commit-config.yaml` & `blueapi-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.vscode/launch.json` & `blueapi-0.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/.vscode/settings.json` & `blueapi-0.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/LICENSE` & `blueapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/PKG-INFO` & `blueapi-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.1.0
+Version: 0.2.0
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.1.0/README.rst` & `blueapi-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/conf.py` & `blueapi-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/developer/explanations/decisions.rst` & `blueapi-0.2.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/developer/how-to/build-docs.rst` & `blueapi-0.2.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/developer/how-to/lint.rst` & `blueapi-0.2.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/developer/how-to/make-release.rst` & `blueapi-0.2.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/developer/how-to/update-tools.rst` & `blueapi-0.2.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/developer/index.rst` & `blueapi-0.2.0/docs/developer/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     .. grid-item-card:: :material-regular:`apartment;3em`
 
         .. toctree::
             :caption: Explanations
             :maxdepth: 1
 
             explanations/decisions
+            explanations/architecture
+            explanations/lifecycle
+            explanations/type_validators
 
         +++
 
         Explanations of how and why the architecture is why it is.
 
     .. grid-item-card:: :material-regular:`description;3em`
```

### Comparing `blueapi-0.1.0/docs/developer/reference/standards.rst` & `blueapi-0.2.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/images/dls-favicon.ico` & `blueapi-0.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/images/dls-logo.svg` & `blueapi-0.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/index.rst` & `blueapi-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/user/explanations/docs-structure.rst` & `blueapi-0.2.0/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/user/index.rst` & `blueapi-0.2.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/docs/user/tutorials/installation.rst` & `blueapi-0.2.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/helm/blueapi/Chart.yaml` & `blueapi-0.2.0/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.2.0/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/helm/blueapi/templates/deployment.yaml` & `blueapi-0.2.0/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.2.0/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/helm/blueapi/values.yaml` & `blueapi-0.2.0/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/pyproject.toml` & `blueapi-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ]
 description = "One line description of your module"
 dependencies = [
     "bluesky",
     "ophyd",
     "nslsii",
     "pyepics",
-    "apischema",
+    "pydantic",
     "stomp.py",
-    "scanspec<=0.5.5",
+    "scanspec",
     "PyYAML",
     "click",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.8"
@@ -88,19 +88,19 @@
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = ["error", "ignore::DeprecationWarning"]
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/blueapi.coverage"
+omit = ["src/blueapi/startup/**/*"]
 
 [tool.coverage.paths]
 # Tests are run from installed location, map back to the src directory
 source = ["src", "**/site-packages/"]
-omit = ["src/blueapi/startup"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
```

### Comparing `blueapi-0.1.0/src/blueapi/cli/amq.py` & `blueapi-0.2.0/src/blueapi/cli/amq.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/cli/cli.py` & `blueapi-0.2.0/src/blueapi/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,22 @@
 def controller(ctx, host: str, port: int, log_level: str):
     # if no command is supplied, run with the options passed
     if ctx.invoked_subcommand is None:
         print("Please invoke subcommand!")
         return
     logging.basicConfig(level=log_level)
     ctx.ensure_object(dict)
-    client = AmqClient(StompMessagingTemplate.autoconfigured(StompConfig(host, port)))
+    client = AmqClient(
+        StompMessagingTemplate.autoconfigured(
+            StompConfig(
+                host=host,
+                port=port,
+            )
+        )
+    )
     ctx.obj["client"] = client
     client.app.connect()
 
 
 @controller.command(name="plans")
 @click.pass_context
 def get_plans(ctx) -> None:
```

### Comparing `blueapi-0.1.0/src/blueapi/cli/updates.py` & `blueapi-0.2.0/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/core/bluesky_types.py` & `blueapi-0.2.0/src/blueapi/core/bluesky_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-from dataclasses import dataclass
 from typing import Any, Callable, Generator, Mapping, Type, Union
 
 from bluesky.protocols import (
     Checkable,
     Configurable,
     Flyable,
     HasHints,
@@ -16,14 +15,15 @@
     Status,
     Stoppable,
     Subscribable,
     Triggerable,
     WritesExternalAssets,
 )
 from bluesky.utils import Msg
+from pydantic import BaseModel, Field
 
 try:
     from typing import Protocol, runtime_checkable
 except ImportError:
     from typing_extensions import Protocol, runtime_checkable  # type: ignore
 
 #: A true "plan", usually the output of a generator function
@@ -53,41 +53,48 @@
 
 #: Protocols defining interface to hardware
 BLUESKY_PROTOCOLS = list(Device.__args__)  # type: ignore
 
 
 def is_bluesky_compatible_device(obj: Any) -> bool:
     is_object = not inspect.isclass(obj)
-    follows_protocols = any(
-        map(lambda protocol: isinstance(obj, protocol), BLUESKY_PROTOCOLS)
-    )
     # We must separately check if Obj refers to an instance rather than a
     # class, as both follow the protocols but only one is a "device".
-    return is_object and follows_protocols
+    return is_object and _follows_bluesky_protocols(obj)
+
+
+def is_bluesky_compatible_device_type(cls: Type[Any]) -> bool:
+    # We must separately check if Obj refers to an class rather than an
+    # instance, as both follow the protocols but only one is a type.
+    return inspect.isclass(cls) and _follows_bluesky_protocols(cls)
+
+
+def _follows_bluesky_protocols(obj: Any) -> bool:
+    return any(map(lambda protocol: isinstance(obj, protocol), BLUESKY_PROTOCOLS))
 
 
 def is_bluesky_plan_generator(func: PlanGenerator) -> bool:
     return (
         hasattr(func, "__annotations__")
         and func.__annotations__.get("return") is MsgGenerator
     )
 
 
-@dataclass
-class Plan:
+class Plan(BaseModel):
     """
     A plan that can be run
     """
 
-    name: str
-    model: Type[Any]
+    name: str = Field(description="Referenceable name of the plan")
+    model: Type[BaseModel] = Field(
+        description="Validation model of the parameters for the plan"
+    )
 
 
-@dataclass
-class DataEvent:
+class DataEvent(BaseModel):
     """
     Event representing collection of some data. Conforms to the Bluesky event model:
     https://github.com/bluesky/event-model
     """
 
     name: str
     doc: Mapping[str, Any]
```

### Comparing `blueapi-0.1.0/src/blueapi/core/context.py` & `blueapi-0.2.0/src/blueapi/core/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 import logging
 from dataclasses import dataclass, field
 from importlib import import_module
 from pathlib import Path
 from types import ModuleType
-from typing import Dict, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Union
 
 from bluesky import RunEngine
 from bluesky.protocols import Flyable, Readable
+from pydantic import BaseConfig
 
-from blueapi.utils import load_module_all, schema_for_func
+from blueapi.utils import (
+    TypeValidatorDefinition,
+    create_model_with_type_validators,
+    load_module_all,
+)
 
 from .bluesky_types import (
+    BLUESKY_PROTOCOLS,
     Device,
     Plan,
     PlanGenerator,
     is_bluesky_compatible_device,
     is_bluesky_plan_generator,
 )
 from .device_lookup import find_component
 
 LOGGER = logging.getLogger(__name__)
 
 
+class PlanModelConfig(BaseConfig):
+    arbitrary_types_allowed = True
+
+
 @dataclass
 class BlueskyContext:
     """
     Context for building a Bluesky application
     """
 
     run_engine: RunEngine = field(
@@ -103,16 +113,22 @@
         Returns:
             PlanGenerator: The plan passed in for chaining/decorating
         """
 
         if not is_bluesky_plan_generator(plan):
             raise TypeError(f"{plan} is not a valid plan generator function")
 
-        schema = schema_for_func(plan)
-        self.plans[plan.__name__] = Plan(plan.__name__, schema)
+        validators = list(device_validators(self))
+        model = create_model_with_type_validators(
+            plan.__name__,
+            validators,
+            func=plan,
+            config=PlanModelConfig,
+        )
+        self.plans[plan.__name__] = Plan(name=plan.__name__, model=model)
         self.plan_functions[plan.__name__] = plan
         return plan
 
     def device(self, device: Device, name: Optional[str] = None) -> None:
         """
         Register an device in the context. The device needs to be registered with a
         name. If the device is Readable, Movable or Flyable it has a `name`
@@ -134,7 +150,18 @@
         if name is None:
             if isinstance(device, Readable) or isinstance(device, Flyable):
                 name = device.name
             else:
                 raise KeyError(f"Must supply a name for this device: {device}")
 
         self.devices[name] = device
+
+
+def device_validators(ctx: BlueskyContext) -> Iterable[TypeValidatorDefinition]:
+    def get_device(name: str) -> Device:
+        device = ctx.find_device(name)
+        if device is None:
+            raise KeyError(f"Could not find a device named {name}")
+        return device
+
+    for proto in BLUESKY_PROTOCOLS:
+        yield TypeValidatorDefinition(proto, get_device)
```

### Comparing `blueapi-0.1.0/src/blueapi/core/event.py` & `blueapi-0.2.0/src/blueapi/core/event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 import itertools
 from abc import ABC, abstractmethod
-from typing import Callable, Dict, Generic, TypeVar
+from typing import Callable, Dict, Generic, Optional, TypeVar
 
 #: Event type
 E = TypeVar("E")
 
 #: Subscription token type
 S = TypeVar("S")
 
 
 class EventStream(ABC, Generic[E, S]):
     """
     Generic representation of the Observable pattern
     """
 
     @abstractmethod
-    def subscribe(self, __callback: Callable[[E], None]) -> S:
+    def subscribe(self, __callback: Callable[[E, Optional[str]], None]) -> S:
         """
         Subscribe to new events with a callback
 
         Args:
-            __callback (Callable[[E], None]): What to do with each event
+            __callback: What to do with each event, optionally takes a correlation id
 
         Returns:
             S: A unique token representing the subscription
         """
 
-        ...
-
     @abstractmethod
     def unsubscribe(self, __subscription: S) -> None:
         """
         Stop propagating events to a particular subscription
 
         Args:
             __subscription (S): The token identifying the subscription
         """
 
-        ...
-
     @abstractmethod
     def unsubscribe_all(self) -> None:
         """
         Unsubscribe from all subscriptions
         """
 
-        ...
-
 
 class EventPublisher(EventStream[E, int]):
     """
     Simple Observable that can be fed values to publish
     """
 
-    _subscriptions: Dict[int, Callable[[E], None]]
+    _subscriptions: Dict[int, Callable[[E, Optional[str]], None]]
     _count: itertools.count
 
     def __init__(self) -> None:
         self._subscriptions = {}
         self._count = itertools.count()
 
-    def subscribe(self, callback: Callable[[E], None]) -> int:
+    def subscribe(self, callback: Callable[[E, Optional[str]], None]) -> int:
         sub_id = next(self._count)
         self._subscriptions[sub_id] = callback
         return sub_id
 
     def unsubscribe(self, subscription: int) -> None:
         del self._subscriptions[subscription]
 
     def unsubscribe_all(self) -> None:
         self._subscriptions = {}
 
-    def publish(self, event: E) -> None:
+    def publish(self, event: E, correlation_id: Optional[str] = None) -> None:
         """
         Publish a new event to all subscribers
 
         Args:
-            event (E): The event to publish
+            event: The event to publish
+            correlation_id: An optional ID that may be used to correlate this
+                event with other events
         """
 
         for callback in self._subscriptions.values():
-            callback(event)
+            callback(event, correlation_id)
```

### Comparing `blueapi-0.1.0/src/blueapi/messaging/base.py` & `blueapi-0.2.0/src/blueapi/messaging/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC, abstractmethod
 from concurrent.futures import Future
-from types import TracebackType
 from typing import Any, Callable, Optional, Type
 
 from .context import MessageContext
 
 MessageListener = Callable[[MessageContext, Any], None]
 
 
@@ -24,58 +23,50 @@
         Args:
             name (str): The name of the destination
 
         Returns:
             str: Identifier for the destination
         """
 
-        ...
-
     @abstractmethod
     def queue(self, name: str) -> str:
         """
         A queue with the given name
 
         Args:
             name (str): Name of the queue
 
         Returns:
             str: Identifier for the queue
         """
 
-        ...
-
     @abstractmethod
     def topic(self, name: str) -> str:
         """
         A topic with the given name
 
         Args:
             name (str): Name of the topic
 
         Returns:
             str: Identifier for the topic
         """
 
-        ...
-
     @abstractmethod
     def temporary_queue(self, name: str) -> str:
         """
         A temporary queue with the given name
 
         Args:
             name (str): Name of the queue
 
         Returns:
             str: Identifier for the queue
         """
 
-        ...
-
 
 class MessagingTemplate(ABC):
     """
     Class meant for quickly building message-based applications.
     Includes helpers for asyncronous production/consumption and
     synchronous send/recieve model
     """
@@ -87,21 +78,20 @@
         Get a destination provider that can create destination
         identifiers for this particular template
 
         Returns:
             DestinationProvider: Destination provider
         """
 
-        ...
-
     def send_and_recieve(
         self,
         destination: str,
         obj: Any,
         reply_type: Type = str,
+        correlation_id: Optional[str] = None,
     ) -> Future:
         """
         Send a message expecting a single reply.
 
         Args:
             destination (str): Destination to send the message
             obj (Any): Message to send, must be serializable
@@ -114,36 +104,35 @@
 
         future: Future = Future()
 
         def callback(_: MessageContext, reply: Any) -> None:
             future.set_result(reply)
 
         callback.__annotations__["reply"] = reply_type
-        self.send(destination, obj, callback)
+        self.send(destination, obj, callback, correlation_id)
         return future
 
     @abstractmethod
     def send(
         self,
         __destination: str,
         __obj: Any,
         __on_reply: Optional[MessageListener] = None,
+        __correlation_id: Optional[str] = None,
     ) -> None:
         """
         Send a message to a destination
 
         Args:
             destination (str): Destination to send the message
             obj (Any): Message to send, must be serializable
             __on_reply (Optional[MessageListener], optional): Callback function for
                                                               a reply. Defaults to None.
         """
 
-        ...
-
     def listener(self, destination: str):
         """
         Decorator for subscribing to a topic:
 
         @my_app.listener("my-destination")
         def callback(context: MessageContext, message: ???) -> None:
             ...
@@ -175,34 +164,18 @@
         deserialilization.
 
         Args:
             __destination (str): Destination to subscribe to
             __callback (MessageListener): What to do with each message
         """
 
-        ...
-
-    def __enter__(self) -> "MessagingTemplate":
-        self.connect()
-        return self
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> None:
-        self.disconnect()
-
     @abstractmethod
     def connect(self) -> None:
         """
         Connect the app to transport
         """
-        ...
 
     @abstractmethod
     def disconnect(self) -> None:
         """
         Disconnect the app from transport
         """
-        ...
```

### Comparing `blueapi-0.1.0/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.2.0/src/blueapi/service/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,106 @@
-import itertools
-import json
 import logging
 import uuid
-from typing import Any, Callable, Dict, Optional
+from pathlib import Path
+from typing import Mapping, Optional
 
-import stomp
-from apischema import deserialize, serialize
-from stomp.utils import Frame
-
-from blueapi.config import StompConfig
-from blueapi.utils import handle_all_exceptions
-
-from .base import DestinationProvider, MessageListener, MessagingTemplate
-from .context import MessageContext
-from .utils import determine_deserialization_type
-
-LOGGER = logging.getLogger(__name__)
-
-
-class StompDestinationProvider(DestinationProvider):
-    """
-    Destination provider for stomp, stateless so just
-    uses naming conventions
-    """
-
-    def queue(self, name: str) -> str:
-        return f"/queue/{name}"
-
-    def topic(self, name: str) -> str:
-        return f"/topic/{name}"
-
-    def temporary_queue(self, name: str) -> str:
-        return f"/temp-queue/{name}"
-
-    default = queue
-
-
-class StompMessagingTemplate(MessagingTemplate):
-    """
-    MessagingTemplate that uses the stompp protocol, meant for use
-    with ActiveMQ.
-    """
-
-    _conn: stomp.Connection
-    _sub_num: itertools.count
-    _listener: stomp.ConnectionListener
-    _subscriptions: Dict[str, Callable[[Frame], None]]
+from blueapi.config import ApplicationConfig
+from blueapi.core import BlueskyContext, EventStream
+from blueapi.messaging import MessageContext, MessagingTemplate, StompMessagingTemplate
+from blueapi.utils import ConfigLoader
+from blueapi.worker import RunEngineWorker, RunPlan, Worker
+
+from .model import (
+    DeviceModel,
+    DeviceRequest,
+    DeviceResponse,
+    PlanModel,
+    PlanRequest,
+    PlanResponse,
+    TaskResponse,
+)
+
+
+class Service:
+    _config: ApplicationConfig
+    _ctx: BlueskyContext
+    _worker: Worker
+    _template: MessagingTemplate
+
+    def __init__(self, config: ApplicationConfig) -> None:
+        self._config = config
+        self._ctx = BlueskyContext()
+        self._ctx.with_startup_script(self._config.env.startup_script)
+        self._worker = RunEngineWorker(self._ctx)
+        self._template = StompMessagingTemplate.autoconfigured(config.stomp)
+
+    def run(self) -> None:
+        logging.basicConfig(level=self._config.logging.level)
+
+        self._publish_event_streams(
+            {
+                self._worker.worker_events: self._template.destinations.topic(
+                    "public.worker.event"
+                ),
+                self._worker.progress_events: self._template.destinations.topic(
+                    "public.worker.event.progress"
+                ),
+                self._worker.data_events: self._template.destinations.topic(
+                    "public.worker.event.data"
+                ),
+            }
+        )
 
-    # Stateless implementation means attribute can be static
-    _destination_provider: DestinationProvider = StompDestinationProvider()
+        self._template.subscribe("worker.run", self._on_run_request)
+        self._template.subscribe("worker.plans", self._get_plans)
+        self._template.subscribe("worker.devices", self._get_devices)
 
-    def __init__(self, conn: stomp.Connection) -> None:
-        self._conn = conn
-        self._sub_num = itertools.count()
-        self._listener = stomp.ConnectionListener()
+        self._template.connect()
 
-        self._listener.on_message = self._on_message
-        self._conn.set_listener("", self._listener)
+        self._worker.run_forever()
 
-        self._subscriptions = {}
+    def _publish_event_streams(
+        self, streams_to_destinations: Mapping[EventStream, str]
+    ) -> None:
+        for stream, destination in streams_to_destinations.items():
+            self._publish_event_stream(stream, destination)
 
-    @classmethod
-    def autoconfigured(cls, config: StompConfig) -> MessagingTemplate:
-        return cls(
-            stomp.Connection([(config.host, config.port)], auto_content_length=False)
+    def _publish_event_stream(self, stream: EventStream, destination: str) -> None:
+        stream.subscribe(
+            lambda event, correlation_id: self._template.send(
+                destination, event, None, correlation_id
+            )
         )
 
-    @property
-    def destinations(self) -> DestinationProvider:
-        return self._destination_provider
+    def _on_run_request(self, message_context: MessageContext, task: RunPlan) -> None:
+        correlation_id = message_context.correlation_id or str(uuid.uuid1())
+        self._worker.submit_task(correlation_id, task)
+
+        reply_queue = message_context.reply_destination
+        if reply_queue is not None:
+            response = TaskResponse(task_name=correlation_id)
+            self._template.send(reply_queue, response)
+
+    def _get_plans(self, message_context: MessageContext, message: PlanRequest) -> None:
+        plans = list(map(PlanModel.from_plan, self._ctx.plans.values()))
+        response = PlanResponse(plans=plans)
 
-    def send(
-        self, destination: str, obj: Any, on_reply: Optional[MessageListener] = None
-    ) -> None:
-        self._send_str(
-            destination,
-            json.dumps(serialize(obj)),
-            on_reply,
-        )
+        assert message_context.reply_destination is not None
+        self._template.send(message_context.reply_destination, response)
 
-    def _send_str(
-        self,
-        destination: str,
-        message: str,
-        on_reply: Optional[MessageListener] = None,
+    def _get_devices(
+        self, message_context: MessageContext, message: DeviceRequest
     ) -> None:
-        LOGGER.info(f"SENDING {message} to {destination}")
+        devices = list(map(DeviceModel.from_device, self._ctx.devices.values()))
+        response = DeviceResponse(devices=devices)
 
-        headers: Dict[str, Any] = {}
-        if on_reply is not None:
-            reply_queue_name = self.destinations.temporary_queue(str(uuid.uuid1()))
-            headers = {**headers, "reply-to": reply_queue_name}
-            self.subscribe(reply_queue_name, on_reply)
-        self._conn.send(headers=headers, body=message, destination=destination)
-
-    def subscribe(self, destination: str, callback: MessageListener) -> None:
-        LOGGER.info(f"New subscription to {destination}")
-
-        obj_type = determine_deserialization_type(callback, default=str)
-
-        def wrapper(frame: Frame) -> None:
-            as_dict = json.loads(frame.body)
-            value = deserialize(obj_type, as_dict)
-
-            context = MessageContext(
-                frame.headers["destination"], frame.headers.get("reply-to")
-            )
-            callback(context, value)
+        assert message_context.reply_destination is not None
+        self._template.send(message_context.reply_destination, response)
 
-        sub_id = str(next(self._sub_num))
 
-        self._subscriptions[sub_id] = wrapper
-        self._conn.subscribe(destination=destination, id=sub_id, ack="auto")
+def start(config_path: Optional[Path] = None):
+    loader = ConfigLoader(ApplicationConfig)
+    if config_path is not None:
+        loader.use_yaml_or_json_file(config_path)
+    config = loader.load()
 
-    def connect(self) -> None:
-        self._conn.connect()
-
-    def disconnect(self) -> None:
-        self._conn.disconnect()
-
-    @handle_all_exceptions
-    def _on_message(self, frame: Frame) -> None:
-        LOGGER.info(f"Recieved {frame}")
-        sub_id = frame.headers.get("subscription")
-        callback = self._subscriptions.get(sub_id)
-        if callback is not None:
-            callback(frame)
-        else:
-            LOGGER.warn(f"No subscription active for id: {sub_id}")
+    Service(config).run()
```

### Comparing `blueapi-0.1.0/src/blueapi/messaging/utils.py` & `blueapi-0.2.0/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/plans/stubs.py` & `blueapi-0.2.0/src/blueapi/plans/stubs.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/startup/adsim.py` & `blueapi-0.2.0/src/blueapi/startup/adsim.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/startup/bl45p.py` & `blueapi-0.2.0/src/blueapi/startup/bl45p.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/startup/example.py` & `blueapi-0.2.0/src/blueapi/startup/example.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/startup/simmotor.py` & `blueapi-0.2.0/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/utils/config.py` & `blueapi-0.2.0/src/blueapi/utils/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Any, Generic, Mapping, Type, TypeVar
 
 import yaml
-from apischema import deserialize
+from pydantic import BaseModel, parse_obj_as
 
 #: Configuration schema dataclass
-C = TypeVar("C")
+C = TypeVar("C", bound=BaseModel)
 
 
 class ConfigLoader(Generic[C]):
     """
     Small utility class for loading config from various sources.
     You must define a config schema as a dataclass (or series of
     nested dataclasses) that can then be loaded from some combination
@@ -55,8 +55,8 @@
         Finalize and load the config as an instance of the `schema`
         dataclass.
 
         Returns:
             C: Dataclass instance holding config
         """
 
-        return deserialize(self._schema, self._values)
+        return parse_obj_as(self._schema, self._values)
```

### Comparing `blueapi-0.1.0/src/blueapi/utils/modules.py` & `blueapi-0.2.0/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/utils/thread_exception.py` & `blueapi-0.2.0/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/worker/multithread.py` & `blueapi-0.2.0/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/src/blueapi/worker/reworker.py` & `blueapi-0.2.0/src/blueapi/worker/reworker.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,26 +137,41 @@
         self,
     ) -> None:
         task_status: Optional[TaskStatus]
         errors = self._errors
         warnings = self._warnings
         if self._current is not None:
             task_status = TaskStatus(
-                self._current.name,
-                self._current.is_complete,
-                self._current.is_error or bool(errors),
+                task_name=self._current.name,
+                task_complete=self._current.is_complete,
+                task_failed=self._current.is_error or bool(errors),
             )
+            correlation_id = self._current.name
         else:
             task_status = None
+            correlation_id = None
 
-        event = WorkerEvent(self._state, task_status, errors, warnings)
-        self._worker_events.publish(event)
+        event = WorkerEvent(
+            state=self._state,
+            task_status=task_status,
+            errors=errors,
+            warnings=warnings,
+        )
+        self._worker_events.publish(event, correlation_id)
 
     def _on_document(self, name: str, document: Mapping[str, Any]) -> None:
-        self._data_events.publish(DataEvent(name, document))
+        if self._current is not None:
+            correlation_id = self._current.name
+            self._data_events.publish(
+                DataEvent(name=name, doc=document), correlation_id
+            )
+        else:
+            raise KeyError(
+                "Trying to emit a document despite the fact that the RunEngine is idle"
+            )
 
     def _waiting_hook(self, statuses: Optional[Iterable[Status]]) -> None:
         if statuses is not None:
             with self._status_lock:
                 for status in statuses:
                     self._monitor_status(status)
 
@@ -192,31 +207,32 @@
         time_remaining: Optional[float] = None,
     ) -> None:
         if not status.done:
             percentage = float(1.0 - fraction) if fraction is not None else None
         else:
             percentage = 1.0
         view = StatusView(
-            name or "UNKNOWN",
-            current,
-            initial,
-            target,
-            unit or "units",
-            precision or 3,
-            status.done,
-            percentage,
-            time_elapsed,
-            time_remaining,
+            display_name=name or "UNKNOWN",
+            current=current,
+            initial=initial,
+            target=target,
+            unit=unit or "units",
+            precision=precision or 3,
+            done=status.done,
+            percentage=percentage,
+            time_elapsed=time_elapsed,
+            time_remaining=time_remaining,
         )
         self._status_snapshot[status_name] = view
         self._publish_status_snapshot()
 
     def _publish_status_snapshot(self) -> None:
         if self._current is None:
             raise ValueError("Got a status update without an active task!")
         else:
             self._progress_events.publish(
                 ProgressEvent(
-                    self._current.name,
+                    task_name=self._current.name,
                     statuses=self._status_snapshot,
-                )
+                ),
+                self._current.name,
             )
```

### Comparing `blueapi-0.1.0/src/blueapi/worker/worker.py` & `blueapi-0.2.0/src/blueapi/worker/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,51 +19,43 @@
         """
         Submit a task to be run
 
         Args:
             __name (str): A unique name to identify this task
             __task (T): The task to run
         """
-        ...
 
     @abstractmethod
     def run_forever(self) -> None:
         """
         Run all tasks as-submitted. Blocks thread.
         """
-        ...
 
     @property
     @abstractmethod
     def worker_events(self) -> EventStream[WorkerEvent, int]:
         """
         Events representing changes/errors in worker state
 
         Returns:
             EventStream[WorkerEvent, int]: Subscribable stream of events
         """
 
-        ...
-
     @property
     @abstractmethod
     def progress_events(self) -> EventStream[ProgressEvent, int]:
         """
         Events representing progress in running a task
 
         Returns:
             EventStream[ProgressEvent, int]: Subscribable stream of events
         """
 
-        ...
-
     @property
     @abstractmethod
     def data_events(self) -> EventStream[DataEvent, int]:
         """
         Events representing collection of data
 
         Returns:
             EventStream[DataEvent, int]: Subscribable stream of events
         """
-
-        ...
```

### Comparing `blueapi-0.1.0/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.2.0/src/blueapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.1.0
+Version: 0.2.0
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.1.0/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.2.0/src/blueapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,29 @@
 .vscode/tasks.json
 config/adsim.yaml
 config/bl45p.yaml
 docs/conf.py
 docs/genindex.rst
 docs/index.rst
 docs/developer/index.rst
+docs/developer/explanations/architecture.rst
 docs/developer/explanations/decisions.rst
+docs/developer/explanations/lifecycle.rst
+docs/developer/explanations/type_validators.rst
 docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
 docs/developer/how-to/build-docs.rst
 docs/developer/how-to/contribute.rst
 docs/developer/how-to/lint.rst
 docs/developer/how-to/make-release.rst
 docs/developer/how-to/run-tests.rst
 docs/developer/how-to/static-analysis.rst
 docs/developer/how-to/update-tools.rst
 docs/developer/reference/standards.rst
 docs/developer/tutorials/dev-install.rst
+docs/images/blueapi-architecture.png
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
 docs/user/index.rst
 docs/user/explanations/docs-structure.rst
 docs/user/how-to/run-container.rst
 docs/user/reference/api.rst
 docs/user/tutorials/installation.rst
@@ -88,32 +92,36 @@
 src/blueapi/startup/adsim.py
 src/blueapi/startup/bl45p.py
 src/blueapi/startup/example.py
 src/blueapi/startup/simmotor.py
 src/blueapi/utils/__init__.py
 src/blueapi/utils/config.py
 src/blueapi/utils/modules.py
-src/blueapi/utils/schema.py
+src/blueapi/utils/serialization.py
 src/blueapi/utils/thread_exception.py
+src/blueapi/utils/type_validator.py
 src/blueapi/worker/__init__.py
 src/blueapi/worker/event.py
 src/blueapi/worker/multithread.py
 src/blueapi/worker/reworker.py
 src/blueapi/worker/task.py
 src/blueapi/worker/worker.py
+tests/conftest.py
 tests/test_cli.py
 tests/core/__init__.py
 tests/core/test_context.py
-tests/core/test_device_lookup.py
+tests/core/test_event.py
 tests/messaging/__init__.py
 tests/messaging/test_stomptemplate.py
 tests/messaging/test_utils.py
+tests/plans/__init__.py
+tests/plans/test_scanspec_metadata.py
 tests/utils/__init__.py
 tests/utils/config.yaml
 tests/utils/hasall.py
 tests/utils/lacksall.py
 tests/utils/nested_config.yaml
 tests/utils/override_config.yaml
 tests/utils/test_config.py
 tests/utils/test_modules.py
-tests/utils/test_schema.py
-tests/utils/test_thread_exception.py
+tests/utils/test_thread_exception.py
+tests/utils/test_type_validator.py
```

### Comparing `blueapi-0.1.0/tests/core/test_context.py` & `blueapi-0.2.0/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/tests/messaging/test_utils.py` & `blueapi-0.2.0/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.1.0/tests/utils/test_config.py` & `blueapi-0.2.0/tests/utils/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import os
-from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Type
 
 import pytest
-from apischema import ValidationError
+from pydantic import BaseModel, Field, ValidationError
 
 from blueapi.utils import ConfigLoader
 
 
-@dataclass
-class Config:
+class Config(BaseModel):
     foo: int
     bar: str
 
 
-@dataclass
-class ConfigWithDefaults:
+class ConfigWithDefaults(BaseModel):
     foo: int = 3
     bar: str = "hello world"
 
 
-@dataclass
-class NestedConfig:
+class NestedConfig(BaseModel):
     nested: Config
     baz: bool
 
 
-@dataclass
-class NestedConfigWithDefaults:
-    nested: ConfigWithDefaults = field(default_factory=ConfigWithDefaults)
+class NestedConfigWithDefaults(BaseModel):
+    nested: ConfigWithDefaults = Field(default_factory=ConfigWithDefaults)
     baz: bool = False
 
 
 @pytest.fixture
 def package_root() -> Path:
     return Path(os.path.dirname(os.path.realpath(__file__)))
```

### Comparing `blueapi-0.1.0/tests/utils/test_thread_exception.py` & `blueapi-0.2.0/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

