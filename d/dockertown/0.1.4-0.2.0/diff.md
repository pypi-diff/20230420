# Comparing `tmp/dockertown-0.1.4.tar.gz` & `tmp/dockertown-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockertown-0.1.4.tar", last modified: Fri Jan 27 06:55:05 2023, max compression
+gzip compressed data, was "dockertown-0.2.0.tar", last modified: Thu Apr 20 14:39:31 2023, max compression
```

## Comparing `dockertown-0.1.4.tar` & `dockertown-0.2.0.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2475 2022-11-29 22:47:10.000000 dockertown-0.1.4/CONTRIBUTING.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1087 2022-11-29 22:47:10.000000 dockertown-0.1.4/LICENSE
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       67 2022-11-29 22:47:10.000000 dockertown-0.1.4/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15850 2023-01-27 06:55:05.729067 dockertown-0.1.4/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15396 2022-11-29 22:47:10.000000 dockertown-0.1.4/README.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/docs/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/docs/template/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4875 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_client.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/docs/template/docker_objects/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      692 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/builders.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1078 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/configs.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1042 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/containers.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1249 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/images.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1180 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/networks.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      966 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/nodes.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1037 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/plugins.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1108 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/services.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      689 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/tasks.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1103 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/docker_objects/volumes.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/docs/template/sub-commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1279 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/sub-commands/buildx.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2097 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/sub-commands/compose.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/docs/template/user_guide/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3711 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/user_guide/docker_run.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      961 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/user_guide/exceptions.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6442 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/user_guide/generic_resources.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3364 2022-11-29 22:47:10.000000 dockertown-0.1.4/docs/template/user_guide/running_inside_a_container.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       54 2022-11-29 22:47:10.000000 dockertown-0.1.4/requirements.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-01-27 06:55:05.729067 dockertown-0.1.4/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1022 2023-01-27 06:54:57.000000 dockertown-0.1.4/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.725067 dockertown-0.1.4/src/dockertown/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      904 2023-01-27 06:54:57.000000 dockertown-0.1.4/src/dockertown/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9430 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/client_config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1492 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/command_line_entrypoint.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/buildx/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/buildx/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    22105 2023-01-27 06:52:35.000000 dockertown-0.1.4/src/dockertown/components/buildx/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/buildx/imagetools/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/buildx/imagetools/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1998 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/buildx/imagetools/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1364 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/buildx/imagetools/models.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1017 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/buildx/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/compose/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/compose/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    28447 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/compose/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2706 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/compose/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/config/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/config/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4775 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/config/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      601 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/config/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/container/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/container/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    69357 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/container/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7427 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/container/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/context/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/context/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4037 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/context/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      542 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/context/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/image/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/image/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23407 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/image/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1043 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/image/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/manifest/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/manifest/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3248 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/manifest/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/manifest/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/network/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/network/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7548 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/network/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/network/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/node/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/node/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7452 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/node/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1861 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/node/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/plugin/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/plugin/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9428 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/plugin/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      879 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/plugin/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/secret/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/secret/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3307 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/secret/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/secret/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/service/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/service/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16688 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/service/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2193 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/service/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/stack/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/stack/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5523 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/stack/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/swarm/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/swarm/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9143 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/swarm/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/system/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/system/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6413 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/system/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5429 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/system/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/task/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/task/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3195 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/task/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3811 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/task/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/trust/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/trust/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      486 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/trust/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown/components/volume/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/volume/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10346 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/components/volume/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      385 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/components/volume/models.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12083 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/docker_client.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4364 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/download_binaries.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1808 2023-01-27 06:42:53.000000 dockertown-0.1.4/src/dockertown/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/py.typed
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      710 2022-11-29 22:47:10.000000 dockertown-0.1.4/src/dockertown/test_utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10890 2023-01-27 06:43:19.000000 dockertown-0.1.4/src/dockertown/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/src/dockertown.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15850 2023-01-27 06:55:05.000000 dockertown-0.1.4/src/dockertown.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3822 2023-01-27 06:55:05.000000 dockertown-0.1.4/src/dockertown.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-01-27 06:55:05.000000 dockertown-0.1.4/src/dockertown.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       72 2023-01-27 06:55:05.000000 dockertown-0.1.4/src/dockertown.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       54 2023-01-27 06:55:05.000000 dockertown-0.1.4/src/dockertown.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       11 2023-01-27 06:55:05.000000 dockertown-0.1.4/src/dockertown.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-01-27 06:55:05.729067 dockertown-0.1.4/tests/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       71 2022-11-29 22:47:10.000000 dockertown-0.1.4/tests/test-requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2475 2023-04-19 19:49:15.000000 dockertown-0.2.0/CONTRIBUTING.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1087 2023-04-19 19:49:15.000000 dockertown-0.2.0/LICENSE
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       67 2023-04-19 19:49:15.000000 dockertown-0.2.0/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 14:39:31.985714 dockertown-0.2.0/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14262 2023-04-19 19:49:15.000000 dockertown-0.2.0/README.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/docs/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/docs/template/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4929 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_client.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/docs/template/docker_objects/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      692 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/builders.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1078 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/configs.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1042 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/containers.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1249 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/images.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1180 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/networks.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      966 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/nodes.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1037 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/plugins.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1108 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/services.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      689 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/tasks.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1103 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/docker_objects/volumes.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/docs/template/sub-commands/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1279 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/sub-commands/buildx.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2097 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/sub-commands/compose.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1559 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/sub-commands/context.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/docs/template/user_guide/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3711 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/docker_run.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      961 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/exceptions.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6442 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/generic_resources.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3364 2023-04-19 19:49:15.000000 dockertown-0.2.0/docs/template/user_guide/running_inside_a_container.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:15.000000 dockertown-0.2.0/lint-requirements.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       59 2023-04-19 19:49:15.000000 dockertown-0.2.0/requirements.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 14:39:31.985714 dockertown-0.2.0/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1022 2023-04-20 14:39:24.000000 dockertown-0.2.0/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.977713 dockertown-0.2.0/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1332 2023-04-20 14:39:24.000000 dockertown-0.2.0/src/dockertown/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9429 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/client_config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/command_line_entrypoint.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/buildx/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23517 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2892 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1364 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/imagetools/models.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1016 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/buildx/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/compose/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/compose/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    31127 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/compose/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2918 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/compose/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/config/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/config/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4775 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/config/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      601 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/config/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/container/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/container/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    73220 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/container/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7450 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/container/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/context/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/context/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7724 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/context/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      542 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/context/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/image/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/image/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23635 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/image/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1043 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/image/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/manifest/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/manifest/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5089 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/manifest/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      346 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/manifest/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/network/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/network/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7548 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/network/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/network/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/node/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/node/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7452 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/node/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2176 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/node/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/plugin/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/plugin/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9428 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/plugin/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      879 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/plugin/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/secret/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/secret/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3307 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/secret/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/secret/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/service/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/service/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16688 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/service/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2193 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/service/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/stack/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/stack/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5523 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/stack/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/swarm/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/swarm/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9219 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/swarm/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown/components/system/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/system/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6413 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/system/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5429 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/system/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/src/dockertown/components/task/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/task/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3195 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/task/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3811 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/task/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/src/dockertown/components/trust/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/trust/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      486 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/trust/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/src/dockertown/components/volume/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/volume/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10346 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/volume/cli_wrapper.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      385 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/components/volume/models.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12100 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/docker_client.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4364 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/download_binaries.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1807 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/py.typed
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      710 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/test_utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    11071 2023-04-19 19:49:15.000000 dockertown-0.2.0/src/dockertown/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.981713 dockertown-0.2.0/src/dockertown.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3882 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       72 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       59 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       11 2023-04-20 14:39:31.000000 dockertown-0.2.0/src/dockertown.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:39:31.985714 dockertown-0.2.0/tests/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       29 2023-04-19 19:49:15.000000 dockertown-0.2.0/tests/test-requirements.txt
```

### Comparing `dockertown-0.1.4/CONTRIBUTING.md` & `dockertown-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/LICENSE` & `dockertown-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/PKG-INFO` & `dockertown-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockertown
-Version: 0.1.4
+Version: 0.2.0
 Summary: A decent Python wrapper for Docker CLI
 Home-page: UNKNOWN
 License: MIT
 Project-URL: Documentation, https://duckietown.github.io/dockertown/
 Project-URL: Source Code, https://github.com/duckietown/dockertown
 Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
 Platform: UNKNOWN
@@ -22,14 +22,15 @@
 
 Works on Linux, macOS and Windows, for Python 3.7 and above. 
 
 The docs can be found at this address: <https://duckietown.github.io/dockertown/>
 
 The GitHub repo can be found at this address: <https://github.com/duckietown/dockertown>
 
+------------------------------------------------------------------------
 
 ## How to install?
 
 ```bash
 pip install dockertown
 ```
 
@@ -254,38 +255,14 @@
 do high level operations, use Dockertown.
 For example if you want to write your CI logic in Python rather than in bash (a very good choice 😉).
 Some commands are only available in Dockertown 
 too: `docker.buildx.build(...)`, `docker.stack.deploy(...)`...
 
 Use the right tool for the right job 🙂
 
-## Where is the project now? Where is it going?
-
-| sub-command  | Functions implemented  | Progress |
-|---|---|---|
-| buildx  | 10/11 | ![92%](https://progress-bar.dev/92) |
-| compose  | 18/23 | ![73%](https://progress-bar.dev/78) |
-| config  | 4/4 | ![50%](https://progress-bar.dev/100) |
-| container | 22/24 | ![50%](https://progress-bar.dev/91) |
-| context  | 4/6 | ![50%](https://progress-bar.dev/67) |
-| image  | 12/13 | ![50%](https://progress-bar.dev/92) |
-| manifest  | 0/4 | ![50%](https://progress-bar.dev/0) |
-| network  | 7/7 | ![100%](https://progress-bar.dev/100) |
-| node  | 7/7 | ![100%](https://progress-bar.dev/100) |
-| plugins  | 10/10 | ![50%](https://progress-bar.dev/100) |
-| secret  | 4/4 | ![100%](https://progress-bar.dev/100) |
-| service  | 7/9 | ![50%](https://progress-bar.dev/78) |
-| stack  | 5/5 | ![100%](https://progress-bar.dev/100) |
-| swarm  | 8/8 | ![100%](https://progress-bar.dev/100) |
-| system  | 3/4 | ![50%](https://progress-bar.dev/75) |
-| trust  | 0/3 | ![50%](https://progress-bar.dev/0) |
-| volume  | 7/7 | ![50%](https://progress-bar.dev/100) |
-
-Take those numbers with a grain of salt. The functions don't all need the same amount of work to be implemented.
-
 ## Alternatives to Docker: Podman, nerdctl...
 
 Support for Docker-compatible clients like [Podman](https://podman.io/) and [Nerdctl](https://github.com/containerd/nerdctl) was introduced in Dockertown version 0.44.0.
 
 You can use an arbitrary binary to execute Docker commands by using the argument `client_call` of `dockertown.DockerCLient`.
 Here is an example:
 ```python
```

### Comparing `dockertown-0.1.4/README.md` & `dockertown-0.2.0/src/dockertown.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,36 @@
+Metadata-Version: 2.1
+Name: dockertown
+Version: 0.2.0
+Summary: A decent Python wrapper for Docker CLI
+Home-page: UNKNOWN
+License: MIT
+Project-URL: Documentation, https://duckietown.github.io/dockertown/
+Project-URL: Source Code, https://github.com/duckietown/dockertown
+Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
+Platform: UNKNOWN
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Dockertown
 
 ```text
 NOTE: this project is based on the python-on-whales project, you can find it at https://github.com/gabrieldemarmiesse/python-on-whales.
 ```
 
 A decent Python wrapper for Docker CLI.
 
 Works on Linux, macOS and Windows, for Python 3.7 and above. 
 
 The docs can be found at this address: <https://duckietown.github.io/dockertown/>
 
 The GitHub repo can be found at this address: <https://github.com/duckietown/dockertown>
 
+------------------------------------------------------------------------
 
 ## How to install?
 
 ```bash
 pip install dockertown
 ```
 
@@ -240,38 +255,14 @@
 do high level operations, use Dockertown.
 For example if you want to write your CI logic in Python rather than in bash (a very good choice 😉).
 Some commands are only available in Dockertown 
 too: `docker.buildx.build(...)`, `docker.stack.deploy(...)`...
 
 Use the right tool for the right job 🙂
 
-## Where is the project now? Where is it going?
-
-| sub-command  | Functions implemented  | Progress |
-|---|---|---|
-| buildx  | 10/11 | ![92%](https://progress-bar.dev/92) |
-| compose  | 18/23 | ![73%](https://progress-bar.dev/78) |
-| config  | 4/4 | ![50%](https://progress-bar.dev/100) |
-| container | 22/24 | ![50%](https://progress-bar.dev/91) |
-| context  | 4/6 | ![50%](https://progress-bar.dev/67) |
-| image  | 12/13 | ![50%](https://progress-bar.dev/92) |
-| manifest  | 0/4 | ![50%](https://progress-bar.dev/0) |
-| network  | 7/7 | ![100%](https://progress-bar.dev/100) |
-| node  | 7/7 | ![100%](https://progress-bar.dev/100) |
-| plugins  | 10/10 | ![50%](https://progress-bar.dev/100) |
-| secret  | 4/4 | ![100%](https://progress-bar.dev/100) |
-| service  | 7/9 | ![50%](https://progress-bar.dev/78) |
-| stack  | 5/5 | ![100%](https://progress-bar.dev/100) |
-| swarm  | 8/8 | ![100%](https://progress-bar.dev/100) |
-| system  | 3/4 | ![50%](https://progress-bar.dev/75) |
-| trust  | 0/3 | ![50%](https://progress-bar.dev/0) |
-| volume  | 7/7 | ![50%](https://progress-bar.dev/100) |
-
-Take those numbers with a grain of salt. The functions don't all need the same amount of work to be implemented.
-
 ## Alternatives to Docker: Podman, nerdctl...
 
 Support for Docker-compatible clients like [Podman](https://podman.io/) and [Nerdctl](https://github.com/containerd/nerdctl) was introduced in Dockertown version 0.44.0.
 
 You can use an arbitrary binary to execute Docker commands by using the argument `client_call` of `dockertown.DockerCLient`.
 Here is an example:
 ```python
@@ -317,7 +308,9 @@
 Any and all PRs are welcome. Please see [this documentation](./CONTRIBUTING.md).
 
 ## What about the license?
 
 It's a MIT license, so quite permissive.
 
 The license can be found [in the git repository](https://github.com/duckietown/dockertown/blob/master/LICENSE).
+
+
```

### Comparing `dockertown-0.1.4/docs/template/docker_client.md` & `dockertown-0.2.0/docs/template/docker_client.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 * [`docker.volume`](sub-commands/volume.md)
 
 
 # Other commands
 
 They're actually aliases
 
+* [`docker.attach`](sub-commands/container.md#attach)
 * [`docker.build`](sub-commands/buildx.md#build)
 * [`docker.commit`](sub-commands/container.md#commit)
 * [`docker.copy`](sub-commands/container.md#copy)
 * [`docker.create`](sub-commands/container.md#create)
 * [`docker.diff`](sub-commands/container.md#diff)
 * [`docker.execute`](sub-commands/container.md#execute)
 * [`docker.export`](sub-commands/container.md#export)
```

### Comparing `dockertown-0.1.4/docs/template/docker_objects/builders.md` & `dockertown-0.2.0/docs/template/docker_objects/builders.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/configs.md` & `dockertown-0.2.0/docs/template/docker_objects/configs.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/containers.md` & `dockertown-0.2.0/docs/template/docker_objects/containers.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/images.md` & `dockertown-0.2.0/docs/template/docker_objects/images.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/networks.md` & `dockertown-0.2.0/docs/template/docker_objects/networks.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/nodes.md` & `dockertown-0.2.0/docs/template/docker_objects/nodes.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/plugins.md` & `dockertown-0.2.0/docs/template/docker_objects/plugins.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/services.md` & `dockertown-0.2.0/docs/template/docker_objects/services.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/tasks.md` & `dockertown-0.2.0/docs/template/docker_objects/tasks.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/docker_objects/volumes.md` & `dockertown-0.2.0/docs/template/docker_objects/volumes.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/sub-commands/buildx.md` & `dockertown-0.2.0/docs/template/sub-commands/buildx.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/sub-commands/compose.md` & `dockertown-0.2.0/docs/template/sub-commands/compose.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/user_guide/docker_run.md` & `dockertown-0.2.0/docs/template/user_guide/docker_run.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/user_guide/exceptions.md` & `dockertown-0.2.0/docs/template/user_guide/exceptions.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/user_guide/generic_resources.md` & `dockertown-0.2.0/docs/template/user_guide/generic_resources.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/docs/template/user_guide/running_inside_a_container.md` & `dockertown-0.2.0/docs/template/user_guide/running_inside_a_container.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/setup.py` & `dockertown-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def get_long_description() -> str:
     return (CURRENT_DIR / "README.md").read_text(encoding="utf8")
 
 
 setup(
     name="dockertown",
-    version="0.1.4",
+    version="0.2.0",
     description="A decent Python wrapper for Docker CLI",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     install_requires=(CURRENT_DIR / "requirements.txt").read_text().splitlines(),
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,  # will read the MANIFEST.in
```

### Comparing `dockertown-0.1.4/src/dockertown/client_config.py` & `dockertown-0.2.0/src/dockertown/client_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
             f"The binary '{self.client_call[0]}' could not be found on your PATH. "
             f"Please ensure that your PATH is has the directory of the binary you're looking for. "
             f"You can use `print(os.environ['PATH'])` to verify what directories are in your PATH."
         )
 
     @property
     def docker_cmd(self) -> Command:
-
         result = Command(self.get_client_call_with_path())
 
         if self.config is not None:
             result += ["--config", self.config]
 
         if self.context is not None:
             result += ["--context", self.context]
```

### Comparing `dockertown-0.1.4/src/dockertown/command_line_entrypoint.py` & `dockertown-0.2.0/src/dockertown/command_line_entrypoint.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,29 +23,28 @@
         raise ValueError("No volume was specified. The format is 'volume:path'")
 
 
 image_app = typer.Typer()
 
 
 @image_app.command()
-def copy_from(docker_image: str, source: str, destination: str):
-    image = docker.image._pull_if_necessary(docker_image)
-    docker.image.copy_from(image, source, destination)
+def copy_from(docker_image: str, source: str, destination: str, pull: str = "missing"):
+    docker.image.copy_from(docker_image, source, destination, pull)
 
 
 @image_app.command()
 def copy_to(
     docker_image: str,
     source: str,
     destination: str,
     new_tag: Optional[str] = None,
     push: bool = False,
+    pull: str = "missing",
 ):
-    image = docker.image._pull_if_necessary(docker_image)
-    docker.image.copy_to(image, source, destination, new_tag)
+    docker.image.copy_to(docker_image, source, destination, new_tag, pull)
     if push:
         docker.image.push(new_tag)
 
 
 @app.command()
 def download_cli():
     download_docker_cli()
```

### Comparing `dockertown-0.1.4/src/dockertown/components/buildx/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/buildx/cli_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,33 +198,41 @@
             return json.loads(run(full_cmd + ["--print"] + targets, env=env))
 
     def build(
         self,
         path: ValidPath,
         add_hosts: Dict[str, str] = {},
         allow: List[str] = [],
+        attest: Optional[Dict[str, str]] = None,
         build_args: Dict[str, str] = {},
         build_contexts: Dict[str, ValidPath] = {},
         builder: Optional[ValidBuilder] = None,
         cache: bool = True,
+        # TODO: cache_filters
         cache_from: Union[str, Dict[str, str], List[Dict[str, str]], None] = None,
         cache_to: Union[str, Dict[str, str], None] = None,
+        # TODO: cgroup_parent
         file: Optional[ValidPath] = None,
         labels: Dict[str, str] = {},
         load: bool = False,
+        # TODO: metadata_file
         network: Optional[str] = None,
         output: Dict[str, str] = {},
         platforms: Optional[List[str]] = None,
         progress: Union[str, bool] = "auto",
+        provenance: Union[bool, Dict[str, str], None] = None,
         pull: bool = False,
         push: bool = False,
+        sbom: Union[bool, Dict[str, str], None] = None,
         secrets: Union[str, List[str]] = [],
+        # TODO shm_size
         ssh: Optional[str] = None,
         tags: Union[str, List[str]] = [],
         target: Optional[str] = None,
+        # TODO: ulimit
         stream_logs: bool = False,
     ) -> Union[None, Image, Iterator[str]]:
         """Build a Docker image with builkit as backend.
 
         Alias: `docker.build(...)`
 
         A `dockertown.Image` is returned, even when using multiple tags.
@@ -233,14 +241,15 @@
         then `None` is returned.
 
         # Arguments
             path: The path of the build context.
             add_hosts: Hosts to add. `add_hosts={"my_host1": "192.168.32.35"}`
             allow: List of extra privileges.
                 Eg `allow=["network.host", "security.insecure"]`
+            attest: Attestation parameters. Eg `attest={"type": "sbom", "generator": "my_image"}`
             build_args: The build arguments.
                 ex `build_args={"PY_VERSION": "3.7.8", "UBUNTU_VERSION": "20.04"}`.
             build_contexts: Additional build contexts (e.g., name=path).
                 ex `build_contexts={"cxt1": "/app/dir1", "cxt2": "/app/dir2"}`.
             builder: Specify which builder to use.
             cache: Whether or not to use the cache
             cache_from: Works only with the container driver. Loads the cache
@@ -266,16 +275,21 @@
                 `["local", "tar", "oci", "docker", "image", "registry"]`.
                 See [this link](https://github.com/docker/buildx#-o---outputpath-typetypekeyvalue)
                 for more details about each exporter.
             platforms: List of target platforms when building the image. Ex:
                 `platforms=["linux/amd64", "linux/arm64"]`
             progress: Set type of progress output (auto, plain, tty, or False).
                 Use plain to keep the container output on screen
+            provenance: Shortand for `attest={"type": "provenance"}`.
+                Eg `provenance=True` or `provenance=dict(mode="max")`. `provenance=False` might be needed
+                if you are having the
+                issue [Default image output from buildx v0.10 cannot run on Google Cloud Run or AWS Lambda](https://github.com/docker/buildx/issues/1533)
             pull: Always attempt to pull a newer version of the image
             push: Shorthand for `output=dict(type="registry")`.
+            sbom: Shorthand for `attest={"type": "sbom"}`. Eg `sbom=True`.
             secrets: One or more secrets passed as string(s). For example
                 `secrets="id=aws,src=/home/my_user/.aws/credentials"`
             ssh: SSH agent socket or keys to expose to the build
                 (format is `default|<id>[=<socket>|<key>[,<key>]]` as a string)
             tags: Tag or tags to put on the resulting image.
             target: Set the target build stage to build.
             stream_logs: If `True` this function will return an iterator of strings.
@@ -295,22 +309,32 @@
         full_cmd.add_args_list(
             "--add-host", format_dict_for_cli(add_hosts, separator=":")
         )
         full_cmd.add_args_list(
             "--build-context", format_dict_for_cli(build_contexts, separator="=")
         )
         full_cmd.add_args_list("--allow", allow)
+        if isinstance(attest, dict):
+            full_cmd.add_simple_arg("--attest", format_dict_for_buildx(attest))
         full_cmd.add_args_list("--build-arg", format_dict_for_cli(build_args))
         full_cmd.add_simple_arg("--builder", builder)
         full_cmd.add_args_list("--label", format_dict_for_cli(labels))
 
         full_cmd.add_simple_arg("--ssh", ssh)
 
+        if isinstance(provenance, bool):
+            full_cmd.append(f"--provenance={str(provenance).lower()}")
+        elif isinstance(provenance, dict):
+            full_cmd.add_simple_arg("--provenance", format_dict_for_buildx(provenance))
         full_cmd.add_flag("--pull", pull)
         full_cmd.add_flag("--push", push)
+        if isinstance(sbom, bool):
+            full_cmd.append(f"--sbom={str(sbom).lower()}")
+        elif isinstance(sbom, dict):
+            full_cmd.add_simple_arg("--sbom", format_dict_for_buildx(sbom))
         full_cmd.add_flag("--load", load)
         full_cmd.add_simple_arg("--file", file)
         full_cmd.add_simple_arg("--target", target)
         if isinstance(cache_from, list):
             for item in cache_from:
                 full_cmd.add_simple_arg("--cache-from", format_dict_for_buildx(item))
         elif isinstance(cache_from, dict):
```

### Comparing `dockertown-0.1.4/src/dockertown/components/buildx/imagetools/models.py` & `dockertown-0.2.0/src/dockertown/components/buildx/imagetools/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/buildx/models.py` & `dockertown-0.2.0/src/dockertown/components/buildx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     name: str
     driver: str
     status: str
     platforms: List[str] = field(default_factory=lambda: [])
 
     @classmethod
     def from_str(cls, string: str) -> BuilderInspectResult:
-
         string = string.strip()
         result_dict = {}
         for line in string.splitlines():
             if line.startswith("Name:") and "name" not in result_dict:
                 result_dict["name"] = line.split(":")[1].strip()
             if line.startswith("Driver:"):
                 result_dict["driver"] = line.split(":")[1].strip()
```

### Comparing `dockertown-0.1.4/src/dockertown/components/compose/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/compose/cli_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
 import json
 from datetime import timedelta
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
-from ...client_config import DockerCLICaller
+from typing_extensions import Literal
+
+from dockertown.client_config import DockerCLICaller
+from dockertown.components.compose.models import ComposeProject
+from dockertown.utils import parse_ls_status_count
+
 from ...components.container import cli_wrapper as container_cli_wrapper
 from ...utils import format_dict_for_cli, run, stream_stdout_and_stderr, to_list
 from .models import ComposeConfig
 
 
 class ComposeCLI(DockerCLICaller):
     def build(
@@ -280,15 +285,19 @@
         if services == []:
             return
         elif services is not None:
             full_cmd += to_list(services)
         run(full_cmd)
 
     def port(
-        self, service: str, private_port: str, index: int = 1, protocol: str = "tcp"
+        self,
+        service: str,
+        private_port: Union[str, int],
+        index: int = 1,
+        protocol: str = "tcp",
     ) -> Tuple[Optional[str], Optional[int]]:
         """Returns the public port for a port binding.
 
         # Arguments
             service: The name of the service.
             private_port: The private port.
             index: Index of the container if service has multiple replicas (default 1)
@@ -312,31 +321,73 @@
             # docker compose cli joins host:str with port:int in the result. If port is unknown
             # then result has default value for the both variables (str->empty string, int -> 0)
             return None, None
 
         host, port = str(result).split(":")
         return host, int(port)
 
-    def ps(self) -> List[container_cli_wrapper.Container]:
+    def ps(
+        self,
+        services: Optional[List[str]] = None,
+        all: bool = False,
+    ) -> List[container_cli_wrapper.Container]:
         """Returns the containers that were created by the current project.
 
         # Returns
             A `List[dockertown.Container]`
         """
         full_cmd = self.docker_compose_cmd + ["ps", "--quiet"]
+        full_cmd.add_flag("--all", all)
+        if services:
+            full_cmd += services
         result = run(full_cmd)
         ids = result.splitlines()
         # The first line might be a warning for experimental
         # See https://github.com/docker/compose-cli/issues/1108
         if len(ids) > 0 and "experimental" in ids[0]:
             ids.pop(0)
 
         Container = container_cli_wrapper.Container
         return [Container(self.client_config, x, is_immutable_id=True) for x in ids]
 
+    def ls(
+        self, all: bool = False, filters: Dict[str, str] = {}
+    ) -> List[ComposeProject]:
+        """Returns a list of docker compose projects
+
+        # Arguments
+            all_stopped: Results include all stopped compose projects.
+            project_filters: Filter results based on conditions provided.
+
+        # Returns
+            A `List[dockertown.ComposeProject]`
+        """
+        full_cmd = self.docker_compose_cmd + ["ls", "--format", "json"]
+        full_cmd.add_flag("--all", all)
+        full_cmd.add_args_list("--filter", format_dict_for_cli(filters))
+
+        return [
+            ComposeProject(
+                name=proj["Name"],
+                created=parse_ls_status_count(proj["Status"], "created"),
+                running=parse_ls_status_count(proj["Status"], "running"),
+                restarting=parse_ls_status_count(proj["Status"], "restarting"),
+                exited=parse_ls_status_count(proj["Status"], "exited"),
+                paused=parse_ls_status_count(proj["Status"], "paused"),
+                dead=parse_ls_status_count(proj["Status"], "dead"),
+                config_files=[
+                    Path(path)
+                    for path in proj.get("ConfigFiles", "").split(",")
+                    if "ConfigFiles" in proj
+                ]
+                or None,
+            )
+            for proj in json.loads(run(full_cmd))
+        ]
+
     def pull(
         self,
         services: Union[List[str], str, None] = None,
         ignore_pull_failures: bool = False,
         include_deps: bool = False,
         quiet: bool = False,
     ):
@@ -441,15 +492,15 @@
     def run(
         self,
         service: str,
         command: List[str] = [],
         detach: bool = False,
         # entrypoint: Optional[List[str]] = None,
         # envs: Dict[str, str] = {},
-        # labels: Dict[str, str] = {},
+        labels: Dict[str, str] = {},
         name: Optional[str] = None,
         tty: bool = True,
         stream: bool = False,
         dependencies: bool = True,
         publish: List[container_cli_wrapper.ValidPortMapping] = [],
         remove: bool = False,
         service_ports: bool = False,
@@ -461,14 +512,15 @@
         """Run a one-off command on a service.
 
         # Arguments
             service: The name of the service.
             command: The command to execute.
             detach: if `True`, returns immediately with the Container.
                     If `False`, returns the command stdout as string.
+            labels: Add or override labels
             name: Assign a name to the container.
             dependencies: Also start linked services.
             publish: Publish a container's port(s) to the host.
             service_ports: Enable service's ports and map them to the host.
             remove: Automatically remove the container when it exits.
             use_aliases: Use the service's network aliases in the connected network(s).
             tty: Allocate a pseudo-TTY. Allow the process to access your terminal
@@ -513,14 +565,15 @@
                 ]
 
         full_cmd.add_flag("--rm", remove)
         full_cmd.add_flag("--service-ports", service_ports)
         full_cmd.add_flag("--use-aliases", use_aliases)
         full_cmd.add_simple_arg("--user", user)
         full_cmd.add_simple_arg("--workdir", workdir)
+        full_cmd.add_args_list("--label", format_dict_for_cli(labels))
         full_cmd.append(service)
         full_cmd += command
 
         if stream:
             return stream_stdout_and_stderr(full_cmd)
         else:
             result = run(full_cmd, tty=tty)
@@ -595,19 +648,23 @@
         services: Union[List[str], str, None] = None,
         build: bool = False,
         detach: bool = False,
         abort_on_container_exit: bool = False,
         scales: Dict[str, int] = {},
         attach_dependencies: bool = False,
         force_recreate: bool = False,
+        recreate: bool = True,
         no_build: bool = False,
+        remove_orphans: bool = False,
         color: bool = True,
         log_prefix: bool = True,
         start: bool = True,
         quiet: bool = False,
+        wait: bool = False,
+        pull: Literal["always", "missing", "never", None] = None,
     ):
         """Start the containers.
 
         Reading the logs of the containers is not yet implemented.
 
         # Arguments
             services: The services to start. If `None` (default), all services are
@@ -624,38 +681,47 @@
                 stopped. Incompatible with `detach=True`.
             scales: Scale SERVICE to NUM instances. Overrides
                 the scale setting in the Compose file if present. For example:
                 `scales={"my_service": 2, "my_other_service": 5}`.
             attach_dependencies: Attach to dependent containers.
             force_recreate: Recreate containers even if their configuration and image
                 haven't changed.
+            recreate: Recreate the containers if already exist.
+                `recreate=False` and `force_recreate=True` are incompatible.
             no_build: Don't build an image, even if it's missing.
+            remove_orphans: Remove containers for services not defined in the Compose file.
             color: If `False`, it will produce monochrome output.
             log_prefix: If `False`, will not display the prefix in the logs.
             start: Start the service after creating them.
             quiet: By default, some progress bars and logs are sent to stderr and stdout.
                 Set `quiet=True` to avoid having any output.
+            wait: Wait for services to be running|healthy. Implies detached mode.
+            pull: Pull image before running (“always”|”missing”|”never”).
 
         # Returns
             `None` at the moment. The plan is to be able to capture and stream the logs later.
             It's not yet implemented.
 
         """
         full_cmd = self.docker_compose_cmd + ["up"]
         full_cmd.add_flag("--build", build)
         full_cmd.add_flag("--detach", detach)
+        full_cmd.add_flag("--wait", wait)
         full_cmd.add_flag("--abort-on-container-exit", abort_on_container_exit)
         for service, scale in scales.items():
             full_cmd.add_simple_arg("--scale", f"{service}={scale}")
         full_cmd.add_flag("--attach-dependencies", attach_dependencies)
         full_cmd.add_flag("--force-recreate", force_recreate)
+        full_cmd.add_flag("--no-recreate", not recreate)
         full_cmd.add_flag("--no-build", no_build)
         full_cmd.add_flag("--no-color", not color)
         full_cmd.add_flag("--no-log-prefix", not log_prefix)
         full_cmd.add_flag("--no-start", not start)
+        full_cmd.add_flag("--remove-orphans", remove_orphans)
+        full_cmd.add_simple_arg("--pull", pull)
 
         if services == []:
             return
         elif services is not None:
             services = to_list(services)
             full_cmd += services
         # important information is written to both stdout AND stderr.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dockertown-0.1.4/src/dockertown/components/compose/models.py` & `dockertown-0.2.0/src/dockertown/components/compose/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,7 +114,18 @@
 @all_fields_optional
 class ComposeConfig(BaseModel):
     services: Dict[str, ComposeConfigService]
     networks: Dict[str, ComposeConfigNetwork] = Field(default_factory=dict)
     volumes: Dict[str, ComposeConfigVolume] = Field(default_factory=dict)
     configs: Any
     secrets: Any
+
+
+class ComposeProject(BaseModel):
+    name: str
+    created: int = 0
+    running: int = 0
+    restarting: int = 0
+    exited: int = 0
+    paused: int = 0
+    dead: int = 0
+    config_files: Optional[List[Path]]
```

### Comparing `dockertown-0.1.4/src/dockertown/components/config/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/config/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/config/models.py` & `dockertown-0.2.0/src/dockertown/components/config/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/container/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/container/cli_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,29 @@
 
     def __repr__(self):
         return f"dockertown.Container(id='{self.id[:12]}', name='{self.name}')"
 
     # --------------------------------------------------------------------
     # public methods
 
+    def attach(
+        self,
+        detach_keys: Optional[str] = None,
+        stdin: bool = True,
+        sig_proxy: bool = True,
+    ) -> None:
+        """Attach local standard input, output, and error streams to a running container.
+
+        Alias: `docker.attach(...)`
+
+        See the [`docker.container.attach`](../sub-commands/container.md#attach) command for
+        information about the arguments.
+        """
+        ContainerCLI(self.client_config).attach(self, detach_keys, not stdin, sig_proxy)
+
     def commit(
         self,
         tag: Optional[str] = None,
         author: Optional[str] = None,
         message: Optional[str] = None,
         pause: bool = True,
     ) -> image_cli_wrapper.Image:
@@ -345,17 +360,43 @@
 
 
 class ContainerCLI(DockerCLICaller):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.remove = self.remove
 
-    def attach(self):
-        """Not yet implemented"""
-        raise NotImplementedError
+    def attach(
+        self,
+        container: ValidContainer,
+        detach_keys: Optional[str] = None,
+        stdin: bool = True,
+        sig_proxy: bool = True,
+    ) -> None:
+        """Attach local standard input, output, and error streams to a running container
+
+        Alias: `docker.attach(...)`
+
+        # Arguments
+            container: The running container to attach to
+            detach_keys: Override the key sequence for detaching a container
+            stdin: Attach STDIN
+            sig_proxy: Proxy all received signals to the process (default true)
+
+        # Raises
+            `dockertown.exceptions.NoSuchContainer` if the container does not exists.
+        """
+        self.inspect(container)
+
+        full_cmd = self.docker_cmd + ["attach"]
+        full_cmd.add_simple_arg("--detach-keys", detach_keys)
+        full_cmd.add_flag("--no-stdin", not stdin)
+        full_cmd.add_flag("--sig-proxy", sig_proxy)
+        full_cmd.append(container)
+
+        run(full_cmd, tty=True)
 
     def commit(
         self,
         container: ValidContainer,
         tag: Optional[str] = None,
         author: Optional[str] = None,
         message: Optional[str] = None,
@@ -443,14 +484,15 @@
         *,
         add_hosts: List[Tuple[str, str]] = [],
         blkio_weight: Optional[int] = None,
         blkio_weight_device: List[str] = [],
         cap_add: List[str] = [],
         cap_drop: List[str] = [],
         cgroup_parent: Optional[str] = None,
+        cgroupns: Optional[str] = None,
         cidfile: Optional[ValidPath] = None,
         cpu_period: Optional[int] = None,
         cpu_quota: Optional[int] = None,
         cpu_rt_period: Optional[int] = None,
         cpu_rt_runtime: Optional[int] = None,
         cpu_shares: Optional[int] = None,
         cpus: Optional[float] = None,
@@ -506,14 +548,15 @@
         oom_score_adj: Optional[int] = None,
         pid: Optional[str] = None,
         pids_limit: Optional[int] = None,
         platform: Optional[str] = None,
         privileged: bool = False,
         publish: List[ValidPortMapping] = [],
         publish_all: bool = False,
+        pull: str = "missing",
         read_only: bool = False,
         restart: Optional[str] = None,
         remove: bool = False,
         runtime: Optional[str] = None,
         security_options: List[str] = [],
         shm_size: Union[int, str, None] = None,
         sig_proxy: bool = True,
@@ -542,27 +585,34 @@
         workflow: `docker create` -> `docker cp` -> `docker start` to put files
         in the container before starting.
 
         There is no `detach` argument since it's a runtime option.
 
         The arguments are the same as [`docker.run`](#run).
         """
-        image_cli_wrapper.ImageCLI(self.client_config)._pull_if_necessary(image)
+
+        image_cli = image_cli_wrapper.ImageCLI(self.client_config)
+        if pull == "missing":
+            image_cli._pull_if_necessary(image)
+        elif pull == "always":
+            image_cli.pull(image)
+
         full_cmd = self.docker_cmd + ["create"]
 
         add_hosts = [f"{host}:{ip}" for host, ip in add_hosts]
         full_cmd.add_args_list("--add-host", add_hosts)
 
         full_cmd.add_simple_arg("--blkio-weight", blkio_weight)
         full_cmd.add_args_list("--blkio-weight-device", blkio_weight_device)
 
         full_cmd.add_args_list("--cap-add", cap_add)
         full_cmd.add_args_list("--cap-drop", cap_drop)
 
         full_cmd.add_simple_arg("--cgroup-parent", cgroup_parent)
+        full_cmd.add_simple_arg("--cgroupns", cgroupns)
         full_cmd.add_simple_arg("--cidfile", cidfile)
 
         full_cmd.add_simple_arg("--cpu-period", cpu_period)
         full_cmd.add_simple_arg("--cpu-quota", cpu_quota)
         full_cmd.add_simple_arg("--cpu-rt-period", cpu_rt_period)
         full_cmd.add_simple_arg("--cpu-rt-runtime", cpu_rt_runtime)
         full_cmd.add_simple_arg("--cpu-shares", cpu_shares)
@@ -649,14 +699,17 @@
 
         full_cmd.add_simple_arg("--platform", platform)
         full_cmd.add_flag("--privileged", privileged)
 
         self._add_publish_to_command(full_cmd, publish)
         full_cmd.add_flag("--publish-all", publish_all)
 
+        if pull == "never":
+            full_cmd.add_simple_arg("--pull", "never")
+
         full_cmd.add_flag("--read-only", read_only)
         full_cmd.add_simple_arg("--restart", restart)
         full_cmd.add_flag("--rm", remove)
 
         full_cmd.add_simple_arg("--runtime", runtime)
         full_cmd.add_args_list("--security-opt", security_options)
 
@@ -763,14 +816,31 @@
 
         # Returns:
             Optional[str]
 
         # Raises
             `dockertown.exceptions.NoSuchContainer` if the container does not exists.
         """
+        if not isinstance(command, list):
+            error_message = (
+                "When calling docker.execute(), the second argument ('command') "
+                "should be a list. "
+                "Here are some examples:"
+                "docker.execute('somecontainer', ['ls']), "
+                "docker.execute('somecontainer', ['cat', '/some/file.txt'])"
+            )
+            if isinstance(command, str):
+                # boy this is the most common error in the world
+                if isinstance(container, str):
+                    container = self.inspect(container)
+                error_message += (
+                    f" In your case, command should not be a string. "
+                    f"You can try docker.execute('{container.name}', {command.split()}, ...)."
+                )
+            raise TypeError(error_message)
         full_cmd = self.docker_cmd + ["exec"]
 
         full_cmd.add_flag("--detach", detach)
 
         full_cmd.add_args_list("--env", format_dict_for_cli(envs))
         full_cmd.add_args_list("--env-file", env_files)
 
@@ -868,15 +938,15 @@
             return [Container(self.client_config, reference) for reference in x]
         else:
             return Container(self.client_config, x)
 
     def kill(
         self,
         containers: Union[ValidContainer, List[ValidContainer]],
-        signal: str = None,
+        signal: Optional[str] = None,
     ) -> None:
         """Kill a container.
 
         Alias: `docker.kill(...)`
 
         # Arguments
             containers: One or more containers to kill
@@ -1115,14 +1185,15 @@
         *,
         add_hosts: List[Tuple[str, str]] = [],
         blkio_weight: Optional[int] = None,
         blkio_weight_device: List[str] = [],
         cap_add: List[str] = [],
         cap_drop: List[str] = [],
         cgroup_parent: Optional[str] = None,
+        cgroupns: Optional[str] = None,
         cidfile: Optional[ValidPath] = None,
         cpu_period: Optional[int] = None,
         cpu_quota: Optional[int] = None,
         cpu_rt_period: Optional[int] = None,
         cpu_rt_runtime: Optional[int] = None,
         cpu_shares: Optional[int] = None,
         cpus: Optional[float] = None,
@@ -1179,14 +1250,15 @@
         oom_score_adj: Optional[int] = None,
         pid: Optional[str] = None,
         pids_limit: Optional[int] = None,
         platform: Optional[str] = None,
         privileged: bool = False,
         publish: List[ValidPortMapping] = [],
         publish_all: bool = False,
+        pull: str = "missing",
         read_only: bool = False,
         restart: Optional[str] = None,
         remove: bool = False,
         runtime: Optional[str] = None,
         security_options: List[str] = [],
         shm_size: Union[int, str, None] = None,
         sig_proxy: bool = True,
@@ -1276,14 +1348,15 @@
         # Arguments
             image: The docker image to use for the container
             command: List of arguments to provide to the container.
             add_hosts: hosts to add in the format of a tuple. For example,
                 `add_hosts=[("my_host_1", "192.168.30.31"), ("host2", "192.168.80.81")]`
             blkio_weight: Block IO (relative weight), between 10 and 1000,
                 or 0 to disable (default 0)
+            cgroupns: Cgroup namespace mode to use, one of 'host' or 'private'.
             cpu_period: Limit CPU CFS (Completely Fair Scheduler) period
             cpu_quota: Limit CPU CFS (Completely Fair Scheduler) quota
             cpu_rt_period: Limit CPU real-time period in microseconds
             cpu_rt_runtime: Limit CPU real-time runtime in microseconds
             cpu_shares: CPU shares (relative weight)
             cpus: The maximal amount of cpu the container can use.
                 `1` means one cpu core.
@@ -1334,14 +1407,15 @@
             privileged: Give extended privileges to this container.
             publish: Ports to publish, same as the `-p` argument in the Docker CLI.
                 example are `[(8000, 7000) , ("127.0.0.1:3000", 2000)]` or
                 `[("127.0.0.1:3000", 2000, "udp")]`. You can also use a single entry in
                 the tuple to signify that you want a random free port on the host. For example:
                 `publish=[(80,)]`.
             publish_all: Publish all exposed ports to random ports.
+            pull: Pull image before running ("always"|"missing"|"never") (default "missing").
             read_only: Mount the container's root filesystem as read only.
             restart: Restart policy to apply when a container exits (default "no")
             remove: Automatically remove the container when it exits.
             runtime: Runtime to use for this container.
             security_options: Security options
             shm_size: Size of /dev/shm. `int` is for bytes. But you can use `"512m"` or
                 `"4g"` for example.
@@ -1357,29 +1431,49 @@
             volume_driver: Optional volume driver for the container
             workdir: The directory in the container where the process will be executed.
 
         # Returns
             The container output as a string if detach is `False` (the default),
             and a `dockertown.Container` if detach is `True`.
         """
+        if not isinstance(command, list):
+            error_message = (
+                "When calling docker.run(), the second argument ('command') "
+                "should be a list. "
+                "Here are some examples:"
+                "docker.run('ubuntu', ['ls']), "
+                "docker.run('ubuntu', ['cat', '/some/file.txt'])"
+            )
+            if isinstance(command, str):
+                # boy this is the most common error in the world
+                error_message += (
+                    f" In your case, command should not be a string. "
+                    f"You can try docker.run('{image}', {command.split()}, ...)."
+                )
+            raise TypeError(error_message)
 
-        image_cli_wrapper.ImageCLI(self.client_config)._pull_if_necessary(image)
+        image_cli = image_cli_wrapper.ImageCLI(self.client_config)
+        if pull == "missing":
+            image_cli._pull_if_necessary(image)
+        elif pull == "always":
+            image_cli.pull(image)
 
         full_cmd = self.docker_cmd + ["container", "run"]
 
         add_hosts = [f"{host}:{ip}" for host, ip in add_hosts]
         full_cmd.add_args_list("--add-host", add_hosts)
 
         full_cmd.add_simple_arg("--blkio-weight", blkio_weight)
         full_cmd.add_args_list("--blkio-weight-device", blkio_weight_device)
 
         full_cmd.add_args_list("--cap-add", cap_add)
         full_cmd.add_args_list("--cap-drop", cap_drop)
 
         full_cmd.add_simple_arg("--cgroup-parent", cgroup_parent)
+        full_cmd.add_simple_arg("--cgroupns", cgroupns)
         full_cmd.add_simple_arg("--cidfile", cidfile)
 
         full_cmd.add_simple_arg("--cpu-period", cpu_period)
         full_cmd.add_simple_arg("--cpu-quota", cpu_quota)
         full_cmd.add_simple_arg("--cpu-rt-period", cpu_rt_period)
         full_cmd.add_simple_arg("--cpu-rt-runtime", cpu_rt_runtime)
         full_cmd.add_simple_arg("--cpu-shares", cpu_shares)
@@ -1469,14 +1563,17 @@
 
         full_cmd.add_simple_arg("--platform", platform)
         full_cmd.add_flag("--privileged", privileged)
 
         self._add_publish_to_command(full_cmd, publish)
         full_cmd.add_flag("--publish-all", publish_all)
 
+        if pull == "never":
+            full_cmd.add_simple_arg("--pull", "never")
+
         full_cmd.add_flag("--read-only", read_only)
         full_cmd.add_simple_arg("--restart", restart)
         full_cmd.add_flag("--rm", remove)
 
         full_cmd.add_simple_arg("--runtime", runtime)
         full_cmd.add_args_list("--security-opt", security_options)
```

### Comparing `dockertown-0.1.4/src/dockertown/components/container/models.py` & `dockertown-0.2.0/src/dockertown/components/container/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,15 @@
     auto_remove: bool
     volume_driver: str
     volumes_from: List[str]
     mounts: List[ContainerMount]
     capabilities: List[str]
     cap_add: List[str]
     cap_drop: List[str]
+    cgroupns_mode: str
     dns: List[str]
     dns_options: List[str]
     dns_search: List[str]
     extra_hosts: List[str]
     group_add: List[str]
     ipc_mode: str
     cgroup: str
```

### Comparing `dockertown-0.1.4/src/dockertown/components/context/models.py` & `dockertown-0.2.0/src/dockertown/components/context/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/image/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/image/cli_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,36 +145,41 @@
         """Add a tag to a Docker image.
 
         See the [`docker.image.tag`](../sub-commands/container.md#tag) command for
         information about the arguments.
         """
         return ImageCLI(self.client_config).tag(self, new_tag)
 
-    def copy_from(self, path_in_image: ValidPath, destination: ValidPath):
+    def copy_from(
+        self, path_in_image: ValidPath, destination: ValidPath, pull: str = "missing"
+    ):
         """Copy a file from a docker image in the local filesystem.
 
         See the `docker.image.copy_from` command for information about the arguments.
         """
-        return ImageCLI(self.client_config).copy_from(self, path_in_image, destination)
+        return ImageCLI(self.client_config).copy_from(
+            self, path_in_image, destination, pull
+        )
 
     def copy_to(
         self,
         local_path: ValidPath,
         path_in_image: ValidPath,
         new_tag: Optional[str] = None,
+        pull: str = "missing",
     ) -> Image:
         """Copy a file from the local filesystem in a docker image to create a new
         docker image.
 
         As if you did a dockerfile with a COPY instruction.
 
         See the `docker.image.copy_to` command for information about the arguments.
         """
         return ImageCLI(self.client_config).copy_to(
-            self, local_path, path_in_image, new_tag
+            self, local_path, path_in_image, new_tag, pull
         )
 
     def exists(self) -> bool:
         """Returns `True` if the docker image exists and `False` if it doesn't exists.
 
         Note that you might have done `docker.image.remove("some_tag")` and the image
         might still exists because dockertown references images by id, not by tag.
@@ -254,15 +259,15 @@
         full_cmd.add_simple_arg("--target", target)
         full_cmd.add_simple_arg("--network", network)
         full_cmd.add_flag("--no-cache", not cache)
         full_cmd.add_args_list("--tag", tags)
 
         docker_image = ImageCLI(self.client_config)
         full_cmd.append(context_path)
-        image_id = run(full_cmd).strip()
+        image_id = run(full_cmd).splitlines()[-1].strip()
         return docker_image.inspect(image_id)
 
     def history(self):
         """Not yet implemented"""
         raise NotImplementedError
 
     def import_(
@@ -653,26 +658,31 @@
         try:
             return self.inspect(image)
         except DockerException:
             print(f"Unable to find image '{image}' locally")
             return self.pull(image)
 
     def copy_from(
-        self, image: ValidImage, path_in_image: ValidPath, destination: ValidPath
+        self,
+        image: ValidImage,
+        path_in_image: ValidPath,
+        destination: ValidPath,
+        pull: str = "missing",
     ):
         with container_cli_wrapper.ContainerCLI(self.client_config).create(
-            image
+            image, pull=pull
         ) as tmp_container:
             tmp_container.copy_from(path_in_image, destination)
 
     def copy_to(
         self,
         base_image: ValidImage,
         local_path: ValidPath,
         path_in_image: ValidPath,
         new_tag: Optional[str] = None,
+        pull: str = "missing",
     ) -> Image:
         with container_cli_wrapper.ContainerCLI(self.client_config).create(
-            base_image
+            base_image, pull=pull
         ) as tmp_container:
             tmp_container.copy_to(local_path, path_in_image)
             return tmp_container.commit(tag=new_tag)
```

### Comparing `dockertown-0.1.4/src/dockertown/components/image/models.py` & `dockertown-0.2.0/src/dockertown/components/image/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/network/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/network/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/network/models.py` & `dockertown-0.2.0/src/dockertown/components/network/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/node/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/node/cli_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,12 +228,12 @@
         full_cmd = self.docker_cmd + ["node", "update"]
 
         full_cmd.add_simple_arg("--availability", availability)
         for label_name, label_value in labels_add.items():
             full_cmd += ["--label-add", f"{label_name}={label_value}"]
 
         for label in rm_labels:
-            full_cmd += ["--rm-label", label]
+            full_cmd += ["--label-rm", label]
 
         full_cmd.add_simple_arg("--role", role)
         full_cmd.append(node)
         run(full_cmd)
```

### Comparing `dockertown-0.1.4/src/dockertown/components/node/models.py` & `dockertown-0.2.0/src/dockertown/components/node/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,103 @@
 from datetime import datetime
 from typing import Dict, List, Optional
 
 from pydantic import Field
 
-from ...utils import DockerCamelModel
+from ...utils import DockerCamelModel, all_fields_optional
 
 
+@all_fields_optional
 class NodeVersion(DockerCamelModel):
     index: int
 
 
+@all_fields_optional
 class NodeSpec(DockerCamelModel):
     name: Optional[str]
     labels: Dict[str, str]
     role: str
     availability: str
 
 
+@all_fields_optional
 class NodePlatform(DockerCamelModel):
     architecture: str
     os: str = Field(alias="OS")
 
 
+@all_fields_optional
 class NodeNamedResourceSpec(DockerCamelModel):
     kind: str
     value: str
 
 
+@all_fields_optional
 class NodeDiscreteResourceSpec(DockerCamelModel):
     kind: str
     value: Optional[int]
 
 
+@all_fields_optional
 class NodeGenericResource(DockerCamelModel):
     named_resource_spec: Optional[NodeNamedResourceSpec]
     discrete_resource_spec: Optional[NodeDiscreteResourceSpec]
 
 
+@all_fields_optional
 class NodeResource(DockerCamelModel):
     nano_cpus: int = Field(alias="NanoCPUs")
     memory_bytes: int
     generic_resources: Optional[List[NodeGenericResource]]
 
 
+@all_fields_optional
 class EnginePlugin(DockerCamelModel):
     type: str
     name: str
 
 
+@all_fields_optional
 class NodeEngine(DockerCamelModel):
     engine_version: str
     labels: Optional[Dict[str, str]]
     plugins: List[EnginePlugin]
 
 
+@all_fields_optional
 class NodeTLSInfo(DockerCamelModel):
     trust_root: str
     cert_issuer_subject: str
     cert_issuer_public_key: str
 
 
+@all_fields_optional
 class NodeDescription(DockerCamelModel):
     hostname: str
     platform: NodePlatform
     resources: NodeResource
     engine: NodeEngine
     tls_info: NodeTLSInfo
 
 
+@all_fields_optional
 class NodeStatus(DockerCamelModel):
     state: str
     message: Optional[str]
     addr: str
 
 
+@all_fields_optional
 class NodeManagerStatus(DockerCamelModel):
     leader: bool
     reachability: str
     addr: str
 
 
+@all_fields_optional
 class NodeInspectResult(DockerCamelModel):
     id: str = Field(alias="ID")
     version: NodeVersion
     created_at: datetime
     updated_at: datetime
     spec: NodeSpec
     description: NodeDescription
```

### Comparing `dockertown-0.1.4/src/dockertown/components/plugin/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/plugin/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/plugin/models.py` & `dockertown-0.2.0/src/dockertown/components/plugin/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/secret/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/secret/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/service/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/service/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/service/models.py` & `dockertown-0.2.0/src/dockertown/components/service/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/stack/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/stack/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/swarm/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/swarm/cli_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from ...client_config import DockerCLICaller
 from ...utils import ValidPath, run
 
 
 class SwarmCLI(DockerCLICaller):
     def ca(
         self,
-        ca_certificate: ValidPath = None,
-        ca_key: ValidPath = None,
-        certificate_expiry: Union[int, timedelta] = None,
+        ca_certificate: Optional[ValidPath] = None,
+        ca_key: Optional[ValidPath] = None,
+        certificate_expiry: Union[int, timedelta, None] = None,
         detach: bool = False,
-        external_ca: str = None,
+        external_ca: Optional[str] = None,
         rotate: bool = False,
     ):
         """Get and rotate the root CA
 
         # Arguments
             ca_certificate: Path to the PEM-formatted root CA certificate
                 to use for the new cluster
@@ -91,19 +91,19 @@
         full_cmd.add_simple_arg("--data-path-port", data_path_port)
         full_cmd.add_simple_arg("--listen-addr", listen_address)
         run(full_cmd)
 
     def join(
         self,
         manager_address: str,
-        advertise_address: str = None,
+        advertise_address: Optional[str] = None,
         availability: str = "active",
-        data_path_address: str = None,
-        listen_address: str = None,
-        token: str = None,
+        data_path_address: Optional[str] = None,
+        listen_address: Optional[str] = None,
+        token: Optional[str] = None,
     ):
         """Joins a swarm
 
         # Arguments
             manager_address: The address of the swarm manager in the format `"{ip}:{port}"`
             advertise_address: Advertised address (format: <ip|interface>[:port])
             availability: Availability of the node
```

### Comparing `dockertown-0.1.4/src/dockertown/components/system/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/system/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/system/models.py` & `dockertown-0.2.0/src/dockertown/components/system/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/task/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/task/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/task/models.py` & `dockertown-0.2.0/src/dockertown/components/task/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/components/volume/cli_wrapper.py` & `dockertown-0.2.0/src/dockertown/components/volume/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/docker_client.py` & `dockertown-0.2.0/src/dockertown/docker_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         self.swarm = SwarmCLI(self.client_config)
         self.system = SystemCLI(self.client_config)
         self.task = TaskCLI(self.client_config)
         self.trust = TrustCLI(self.client_config)
         self.volume = VolumeCLI(self.client_config)
 
         # aliases
-        self.attach = None
+        self.attach = self.container.attach
         self.build = self.buildx.build
         self.legacy_build = self.image.legacy_build
         self.commit = self.container.commit
         self.copy = self.container.copy
         self.create = self.container.create
         self.diff = self.container.diff
         self.events = None
```

### Comparing `dockertown-0.1.4/src/dockertown/download_binaries.py` & `dockertown-0.2.0/src/dockertown/download_binaries.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/exceptions.py` & `dockertown-0.2.0/src/dockertown/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     def __init__(
         self,
         command_launched: List[str],
         return_code: int,
         stdout: Optional[bytes] = None,
         stderr: Optional[bytes] = None,
     ):
-
         self.docker_command: List[str] = command_launched
         self.return_code: int = return_code
         if stdout is None:
             self.stdout: Optional[str] = None
         else:
             self.stdout: Optional[str] = stdout.decode()
         if stderr is None:
```

### Comparing `dockertown-0.1.4/src/dockertown/test_utils.py` & `dockertown-0.2.0/src/dockertown/test_utils.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.1.4/src/dockertown/utils.py` & `dockertown-0.2.0/src/dockertown/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,44 +73,44 @@
         alias_generator = to_docker_camel
         allow_population_by_field_name = True
 
 
 @overload
 def run(
     args: List[Any],
-    capture_stdout: bool = True,
-    capture_stderr: bool = True,
-    input: bytes = None,
-    return_stderr: Literal[True] = False,
-    env: Dict[str, str] = {},
-    tty: bool = False,
-    retry: int = 3,
+    capture_stdout: bool = ...,
+    capture_stderr: bool = ...,
+    input: bytes = ...,
+    return_stderr: Literal[True] = ...,
+    env: Dict[str, str] = ...,
+    tty: bool = ...,
+    retry: int = ...,
 ) -> Tuple[str, str]:
     ...
 
 
 @overload
 def run(
     args: List[Any],
-    capture_stdout: bool = True,
-    capture_stderr: bool = True,
-    input: bytes = None,
-    return_stderr: Literal[False] = False,
-    env: Dict[str, str] = {},
-    tty: bool = False,
-    retry: int = 3,
+    capture_stdout: bool = ...,
+    capture_stderr: bool = ...,
+    input: bytes = ...,
+    return_stderr: Literal[False] = ...,
+    env: Dict[str, str] = ...,
+    tty: bool = ...,
+    retry: int = ...,
 ) -> str:
     ...
 
 
 def run(
     args: List[Any],
     capture_stdout: bool = True,
     capture_stderr: bool = True,
-    input: bytes = None,
+    input: Optional[bytes] = None,
     return_stderr: bool = False,
     env: Dict[str, str] = {},
     tty: bool = False,
     retry: int = 3,
 ) -> Union[str, Tuple[str, str]]:
     args = [str(x) for x in args]
     subprocess_env = dict(os.environ)
@@ -351,7 +351,14 @@
 
 
 def format_time_for_docker(time_object: Union[datetime, timedelta]) -> str:
     if isinstance(time_object, datetime):
         return time_object.strftime("%Y-%m-%dT%H:%M:%S")
     elif isinstance(time_object, timedelta):
         return f"{time_object.total_seconds()}s"
+
+
+def parse_ls_status_count(status_output, status) -> int:
+    try:
+        return int(status_output.split(status + "(")[1].split(")")[0])
+    except IndexError:
+        return 0
```

### Comparing `dockertown-0.1.4/src/dockertown.egg-info/PKG-INFO` & `dockertown-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-Metadata-Version: 2.1
-Name: dockertown
-Version: 0.1.4
-Summary: A decent Python wrapper for Docker CLI
-Home-page: UNKNOWN
-License: MIT
-Project-URL: Documentation, https://duckietown.github.io/dockertown/
-Project-URL: Source Code, https://github.com/duckietown/dockertown
-Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
-Platform: UNKNOWN
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Dockertown
 
 ```text
 NOTE: this project is based on the python-on-whales project, you can find it at https://github.com/gabrieldemarmiesse/python-on-whales.
 ```
 
 A decent Python wrapper for Docker CLI.
 
 Works on Linux, macOS and Windows, for Python 3.7 and above. 
 
 The docs can be found at this address: <https://duckietown.github.io/dockertown/>
 
 The GitHub repo can be found at this address: <https://github.com/duckietown/dockertown>
 
+------------------------------------------------------------------------
 
 ## How to install?
 
 ```bash
 pip install dockertown
 ```
 
@@ -254,38 +241,14 @@
 do high level operations, use Dockertown.
 For example if you want to write your CI logic in Python rather than in bash (a very good choice 😉).
 Some commands are only available in Dockertown 
 too: `docker.buildx.build(...)`, `docker.stack.deploy(...)`...
 
 Use the right tool for the right job 🙂
 
-## Where is the project now? Where is it going?
-
-| sub-command  | Functions implemented  | Progress |
-|---|---|---|
-| buildx  | 10/11 | ![92%](https://progress-bar.dev/92) |
-| compose  | 18/23 | ![73%](https://progress-bar.dev/78) |
-| config  | 4/4 | ![50%](https://progress-bar.dev/100) |
-| container | 22/24 | ![50%](https://progress-bar.dev/91) |
-| context  | 4/6 | ![50%](https://progress-bar.dev/67) |
-| image  | 12/13 | ![50%](https://progress-bar.dev/92) |
-| manifest  | 0/4 | ![50%](https://progress-bar.dev/0) |
-| network  | 7/7 | ![100%](https://progress-bar.dev/100) |
-| node  | 7/7 | ![100%](https://progress-bar.dev/100) |
-| plugins  | 10/10 | ![50%](https://progress-bar.dev/100) |
-| secret  | 4/4 | ![100%](https://progress-bar.dev/100) |
-| service  | 7/9 | ![50%](https://progress-bar.dev/78) |
-| stack  | 5/5 | ![100%](https://progress-bar.dev/100) |
-| swarm  | 8/8 | ![100%](https://progress-bar.dev/100) |
-| system  | 3/4 | ![50%](https://progress-bar.dev/75) |
-| trust  | 0/3 | ![50%](https://progress-bar.dev/0) |
-| volume  | 7/7 | ![50%](https://progress-bar.dev/100) |
-
-Take those numbers with a grain of salt. The functions don't all need the same amount of work to be implemented.
-
 ## Alternatives to Docker: Podman, nerdctl...
 
 Support for Docker-compatible clients like [Podman](https://podman.io/) and [Nerdctl](https://github.com/containerd/nerdctl) was introduced in Dockertown version 0.44.0.
 
 You can use an arbitrary binary to execute Docker commands by using the argument `client_call` of `dockertown.DockerCLient`.
 Here is an example:
 ```python
@@ -331,9 +294,7 @@
 Any and all PRs are welcome. Please see [this documentation](./CONTRIBUTING.md).
 
 ## What about the license?
 
 It's a MIT license, so quite permissive.
 
 The license can be found [in the git repository](https://github.com/duckietown/dockertown/blob/master/LICENSE).
-
-
```

### Comparing `dockertown-0.1.4/src/dockertown.egg-info/SOURCES.txt` & `dockertown-0.2.0/src/dockertown.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+lint-requirements.txt
 requirements.txt
 setup.py
 docs/template/docker_client.md
 docs/template/docker_objects/builders.md
 docs/template/docker_objects/configs.md
 docs/template/docker_objects/containers.md
 docs/template/docker_objects/images.md
@@ -13,14 +14,15 @@
 docs/template/docker_objects/nodes.md
 docs/template/docker_objects/plugins.md
 docs/template/docker_objects/services.md
 docs/template/docker_objects/tasks.md
 docs/template/docker_objects/volumes.md
 docs/template/sub-commands/buildx.md
 docs/template/sub-commands/compose.md
+docs/template/sub-commands/context.md
 docs/template/user_guide/docker_run.md
 docs/template/user_guide/exceptions.md
 docs/template/user_guide/generic_resources.md
 docs/template/user_guide/running_inside_a_container.md
 src/dockertown/__init__.py
 src/dockertown/client_config.py
 src/dockertown/command_line_entrypoint.py
```

