# Comparing `tmp/adaux-2.3.3.tar.gz` & `tmp/adaux-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.3.3.tar", last modified: Thu Apr 13 00:21:54 2023, max compression
+gzip compressed data, was "adaux-2.4.0.tar", last modified: Wed Apr 19 22:46:59 2023, max compression
```

## Comparing `adaux-2.3.3.tar` & `adaux-2.4.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.665895 adaux-2.3.3/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.3.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-13 00:21:54.665895 adaux-2.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-13 00:21:54.665895 adaux-2.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.561891 adaux-2.3.3/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.597892 adaux-2.3.3/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-13 00:14:40.000000 adaux-2.3.3/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14627 2023-04-12 22:22:11.000000 adaux-2.3.3/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14469 2023-04-12 21:20:17.000000 adaux-2.3.3/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.617893 adaux-2.3.3/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-12 21:27:08.000000 adaux-2.3.3/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-12 23:18:12.000000 adaux-2.3.3/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    20260 2023-04-13 00:14:40.000000 adaux-2.3.3/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-12 23:43:59.000000 adaux-2.3.3/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.625893 adaux-2.3.3/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-12 15:47:50.000000 adaux-2.3.3/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 12:28:10.000000 adaux-2.3.3/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15814 2023-04-12 23:05:47.000000 adaux-2.3.3/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.3.3/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.3.3/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-11 12:31:50.000000 adaux-2.3.3/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-12 09:55:20.000000 adaux-2.3.3/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.625893 adaux-2.3.3/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.629894 adaux-2.3.3/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.629894 adaux-2.3.3/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.629894 adaux-2.3.3/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.577892 adaux-2.3.3/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.633894 adaux-2.3.3/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.633894 adaux-2.3.3/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.633894 adaux-2.3.3/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.633894 adaux-2.3.3/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.637894 adaux-2.3.3/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.645894 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.645894 adaux-2.3.3/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.645894 adaux-2.3.3/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.645894 adaux-2.3.3/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.645894 adaux-2.3.3/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.649894 adaux-2.3.3/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.649894 adaux-2.3.3/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.649894 adaux-2.3.3/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.653895 adaux-2.3.3/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.653895 adaux-2.3.3/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.653895 adaux-2.3.3/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-12 15:47:50.000000 adaux-2.3.3/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.657894 adaux-2.3.3/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.581892 adaux-2.3.3/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.657894 adaux-2.3.3/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.657894 adaux-2.3.3/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2530 2023-04-13 00:21:21.000000 adaux-2.3.3/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-12 23:05:47.000000 adaux-2.3.3/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.661895 adaux-2.3.3/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.661895 adaux-2.3.3/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.665895 adaux-2.3.3/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.665895 adaux-2.3.3/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.3.3/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:21:54.601893 adaux-2.3.3/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-13 00:21:54.000000 adaux-2.3.3/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-13 00:21:54.000000 adaux-2.3.3/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:21:54.000000 adaux-2.3.3/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-13 00:21:54.000000 adaux-2.3.3/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:21:20.000000 adaux-2.3.3/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-13 00:21:54.000000 adaux-2.3.3/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-13 00:21:54.000000 adaux-2.3.3/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.328294 adaux-2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.4.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-19 22:46:59.332294 adaux-2.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-19 22:46:59.332294 adaux-2.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:58.924279 adaux-2.4.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.088285 adaux-2.4.0/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14303 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.140287 adaux-2.4.0/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-12 21:27:08.000000 adaux-2.4.0/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-12 23:18:12.000000 adaux-2.4.0/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20260 2023-04-13 00:14:40.000000 adaux-2.4.0/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-12 23:43:59.000000 adaux-2.4.0/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.164288 adaux-2.4.0/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-12 15:47:50.000000 adaux-2.4.0/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15873 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.172288 adaux-2.4.0/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.172288 adaux-2.4.0/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.176288 adaux-2.4.0/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.184289 adaux-2.4.0/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.008282 adaux-2.4.0/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.192289 adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.196289 adaux-2.4.0/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.200289 adaux-2.4.0/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.204289 adaux-2.4.0/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.208289 adaux-2.4.0/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.248291 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.248291 adaux-2.4.0/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.252291 adaux-2.4.0/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.256291 adaux-2.4.0/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.256291 adaux-2.4.0/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.276292 adaux-2.4.0/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.284292 adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.288292 adaux-2.4.0/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.296293 adaux-2.4.0/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.296293 adaux-2.4.0/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.304293 adaux-2.4.0/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-12 15:47:50.000000 adaux-2.4.0/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.036283 adaux-2.4.0/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-04-19 22:45:48.000000 adaux-2.4.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-12 23:05:47.000000 adaux-2.4.0/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.312293 adaux-2.4.0/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.328294 adaux-2.4.0/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.328294 adaux-2.4.0/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.104286 adaux-2.4.0/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:45:47.000000 adaux-2.4.0/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.3.3/LICENSE.txt` & `adaux-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/setup.cfg` & `adaux-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_base_parser.py` & `adaux-2.4.0/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_cli.py` & `adaux-2.4.0/source/adaux/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
     r"""
     Synchronizes local auxilium file with potentially newer template.
     """
     with convert_runtime_to_click_error():
         ctx.obj.sync()
 
     if bake_after:
-        ctx.obj.set_defaults()
         ctx.obj.bake()
 
 
 @adaux.command()
 @click.pass_context
 def bake(ctx: click.Context) -> None:  # pylint: disable=too-many-statements
     """
@@ -331,14 +330,15 @@
     with convert_runtime_to_click_error():
         return_code = ctx.obj.ci(trigger_str, dry=dry)
     ctx.exit(return_code)
 
 
 @adaux.command()
 @click.pass_context
+@click.option("-v", "--open_html", is_flag=True, default=False)
 def cov(ctx: click.Context, open_html: bool) -> None:
     """
     Creates the coverage html report.
     """
     with convert_runtime_to_click_error():
         ctx.obj.cov(open_html)
 
@@ -348,26 +348,14 @@
     """
     Shortcut for docker compose with corresponding compose file.
     """
     with convert_runtime_to_click_error():
         ctx.obj.dcp(*args)
 
 
-@adaux.command(context_settings={"ignore_unknown_options": True})
-@click.pass_context
-@click.argument("composition")
-@click.argument("args", nargs=-1)
-def comp(ctx: click.Context, composition: str, args: tp.List[str]) -> None:
-    """
-    Shortcut for specific compositions shell file: x-compose.sh
-    """
-    with convert_runtime_to_click_error():
-        ctx.obj.comp(composition, *args)
-
-
 @adaux.command()
 @click.pass_context
 @click.argument("payload_names", nargs=-1)
 @click.option(
     "-f", "--force", is_flag=True, default=False, help="runs payload even if up to date"
 )
 @click.option(
```

### Comparing `adaux-2.3.3/source/adaux/_cli_mixin.py` & `adaux-2.4.0/source/adaux/_cli_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,31 +200,25 @@
 
             if open_html:
                 cmd = ["open", str(cov_cache / "index.html")]
                 subprocess.run(cmd, check=True)
 
     def dcp(self: "CliMixin", *args: str) -> None:
         self._raise_if_disabled("docker")
-        cmd = [
-            "docker",
-            "compose",
-            "-f",
-            str(self.target / "docker" / "compose.yml"),
-            *args,
-        ]
-        subprocess.run(cmd, check=False)
-
-    def comp(self: "CliMixin", composition: str, *args: str) -> None:
-        self._raise_if_disabled("docker")
-        cmd = [
-            "sh",
-            str(self.target / "docker" / f"{composition}-compose.sh"),
-            *args,
-        ]
-        subprocess.run(cmd, check=False)
+        with self.extra() as aux:
+            cmd = [
+                "docker",
+                "compose",
+                "-p",
+                aux.project.slug,
+                "-f",
+                str(self.target / "docker" / "compose.yml"),
+                *args,
+            ]
+            subprocess.run(cmd, check=False)
 
     def run(
         self: "CliMixin", *payload_names: str, force: bool = False, dry: bool = False
     ) -> None:
         self._raise_if_disabled("payload")
         with self.extra(ExtraLevel.HYDRATED), self.cwd_to_root():
             data = self.auxh.payload
```

### Comparing `adaux-2.3.3/source/adaux/_components/_01_file_io_support.py` & `adaux-2.4.0/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_02_base.py` & `adaux-2.4.0/source/adaux/_components/_02_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_03_meta.py` & `adaux-2.4.0/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.4.0/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_05_project.py` & `adaux-2.4.0/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_06_dependency.py` & `adaux-2.4.0/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_07_package.py` & `adaux-2.4.0/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_08_pip.py` & `adaux-2.4.0/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_09_gitignore.py` & `adaux-2.4.0/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_10_gitlab.py` & `adaux-2.4.0/source/adaux/_components/_10_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_11_precommit.py` & `adaux-2.4.0/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_12_pylint.py` & `adaux-2.4.0/source/adaux/_components/_12_pylint.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_13_executable.py` & `adaux-2.4.0/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_14_mypy.py` & `adaux-2.4.0/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_15_pytest.py` & `adaux-2.4.0/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_17_docs.py` & `adaux-2.4.0/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_18_payload.py` & `adaux-2.4.0/source/adaux/_components/_18_payload.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_19_docker.py` & `adaux-2.4.0/source/adaux/_components/_19_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_20_ci.py` & `adaux-2.4.0/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_98_sentinel.py` & `adaux-2.4.0/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_99_all.py` & `adaux-2.4.0/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_aux_ci.py` & `adaux-2.4.0/source/adaux/_components/_aux_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/__init__.py` & `adaux-2.4.0/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/_base.py` & `adaux-2.4.0/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/_docker.py` & `adaux-2.4.0/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.4.0/source/adaux/_components/_payload/_docker_build.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             images=images,
             slug=self.auxh.project.slug,
             service=self.param.service_name,
             image_name=self.param.image_name,
             branch_match=self.param.get("branch_match", []),
             base_match=self.param.get("base_match", []),
             parents=parents,
+            always_build=self.param.get("always_build", False),
             files=[f"devops/docker/{self.param.service_name}.dockerfile"],
         )
 
     def is_up_to_date(self) -> bool:
         if self.param.get("always_build", False):
             return False
         return self.executor.is_up_to_date()  # type: ignore
```

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.4.0/source/adaux/_components/_payload/_docker_executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,47 +73,46 @@
     image_name: str
 
 
 @dc.dataclass(frozen=True)
 class DockerBuildMixin(DockerShared, _DockerBuildMixinState):
     images: tp.List[str] = dc.field(default_factory=list)
     files: tp.List[str] = dc.field(default_factory=list)
+    always_build: bool = False
 
     def script(self) -> None:
         super().script()
         local_tag = self.local_tag
         if self.remote_exists():
             remote_tag = self.remote_tag
-
-            check_and_pull_if_not_existent(remote_tag, self.service, local_tag)
+            check_and_pull_if_not_existent(remote_tag, local_tag, self.service)
             # download other images which are not a direct dependency (cross-repo)
             for image_tag in self.images:
                 image_remote_tag = (
                     f"{self.registry_host}/{self._remove_namespace_local(image_tag)}"
                 )
                 check_and_pull_if_not_existent(image_remote_tag, image_tag)
 
-        if not exists_locally(self.local_tag):
-            # build
+        if not exists_locally(self.local_tag) or self.always_build:
             cmd = [
                 "docker",
                 "--log-level",
                 "ERROR",
                 "compose",
                 "-p",
                 self.slug,
                 "-f",
                 "devops/docker/compose.yml",
                 "build",
                 self.service,
             ]
             subprocess_run(cmd, check=True)
 
-            # upload
-            tag_image(self.use_tag, local_tag)
+        # upload
+        tag_image(self.use_tag, local_tag)
         if self.remote_exists():
             upload_to_remote(local_tag, remote_tag)
             logger.info("uploaded %s to %s", local_tag, remote_tag)
 
     @functools.cached_property
     def tag(self) -> str:
         hasher = hashlib.md5()
@@ -407,27 +406,27 @@
             print("========>> stderr")
             print(err.stderr.decode("utf-8"))
         raise
 
 
 # try to download for caching (or reuse if already there)
 def check_and_pull_if_not_existent(
-    remote_tag: str, service: str, local_tag: tp.Optional[str] = None
+    remote_tag: str, local_tag: str, service: tp.Optional[str] = None
 ) -> None:
     if local_tag and exists_locally(local_tag):
-        return
-
-    if not exists_locally(remote_tag):
+        pass
+    elif not exists_locally(remote_tag):
         cmd = ["docker", "pull", remote_tag]
-        res = subprocess_run(cmd, check=False)
+        res = subprocess_run(cmd, check=False, capture_output=True)
         if res.returncode != 0:
             return
+
+    tag_image(remote_tag, local_tag)
+    if service:
         tag_image(remote_tag, service)
-    if local_tag:
-        tag_image(remote_tag, local_tag)
 
 
 def upload_to_remote(
     local_tag: str, remote_tag: str, registry: tp.Optional[str] = None
 ) -> None:
     tag_image(local_tag, remote_tag)
     cmd = ["docker", "push", remote_tag]
@@ -435,15 +434,15 @@
         cmd += [registry]
     subprocess_run(cmd, check=True, capture_output=True)
     logger.info("pushed '%s'", remote_tag)
 
 
 def tag_image(src_tag: str, dest_tag: str) -> None:
     cmd = ["docker", "image", "tag", src_tag, dest_tag]
-    subprocess_run(cmd, check=True)
+    subprocess_run(cmd, check=True, capture_output=True)
     logger.info("tagged '%s' -> '%s'", src_tag, dest_tag)
 
 
 def exists_locally(local_tag: str) -> bool:
     cmd = ["docker", "image", "inspect", local_tag]
     res = subprocess_run(cmd, check=False, capture_output=True)
     return res.returncode == 0
```

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/_python.py` & `adaux-2.4.0/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.4.0/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_create_badge.py` & `adaux-2.4.0/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_gitlab.py` & `adaux-2.4.0/source/adaux/_gitlab.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __post_init__(self) -> None:
         out = subprocess.run(["git", "remote", "-v"], capture_output=True, check=True)
         (line,) = (x.strip() for x in out.stdout.decode().split("\n") if "fetch" in x)
         line = line.rsplit(" ", 1)[0]
         host, repo = line.split("git@")[1].split(":")
         base_url = "https://" + host
         is_name = repo.replace(".git", "")
-        should_name = self.ns.auxd.project.name.replace(".", "/")
+        should_name = self.ns.auxe.project.name.replace(".", "/")
         if is_name != should_name:
             logger.info("names dont match %s != %s", is_name, should_name)
 
         self.repo_name = is_name
         self.base_url = base_url
         # self.headers = {"Authorization": f"Bearer {self.token}"}
         self.headers = {"PRIVATE-TOKEN": self.token}
@@ -68,15 +68,15 @@
                 enabled=True,
                 cadence="1d",
                 keep_n=1,
                 older_than="7d",
                 name_regex_keep=None,
                 name_regex="aux-.*",
             ),
-            default_branch=self.ns.auxd.gitlab.default_branch,
+            default_branch=self.ns.auxe.gitlab.default_branch,
         )
 
         for key, val in settings.items():
             added = ""
             outdated = self._check_outdated(val, resp[key])
             if isinstance(val, dict):
                 added += "_attributes"
@@ -156,15 +156,15 @@
         if key in ["push_access_level", "merge_access_level"]:
             lvls = resp[f"{key}s"]
             assert len(lvls) == 1
             return lvls[0]["access_level"]
         return resp[key]
 
     def sync_protection(self) -> None:
-        vip_branches = self.ns.auxd.gitlab.vip_branches
+        vip_branches = self.ns.auxe.gitlab.vip_branches
         resp = self.api_request("projects", self.project_id, "protected_branches")
         on_remote = [x["name"] for x in resp]
         to_remove = set(on_remote) - set(vip_branches)
 
         resp_dict = {x["name"]: x for x in resp}
         for branch, setting in vip_branches.items():
             if branch not in on_remote:
```

### Comparing `adaux-2.3.3/source/adaux/_parser.py` & `adaux-2.4.0/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_proto_namespace.py` & `adaux-2.4.0/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_tick.py` & `adaux-2.4.0/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_todo.py` & `adaux-2.4.0/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/_util.py` & `adaux-2.4.0/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.4.0/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.4.0/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.4.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.4.0/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/docs/postprocess_html.py` & `adaux-2.4.0/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.4.0/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.4.0/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.4.0/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.4.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/payload/python/functions.py` & `adaux-2.4.0/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.4.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.4.0/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.3/source/adaux.egg-info/SOURCES.txt` & `adaux-2.4.0/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

