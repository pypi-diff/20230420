# Comparing `tmp/molecule-plugins-23.0.0.tar.gz` & `tmp/molecule-plugins-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-plugins-23.0.0.tar", last modified: Sun Jan  8 15:50:38 2023, max compression
+gzip compressed data, was "molecule-plugins-23.4.0.tar", last modified: Thu Apr 20 13:37:02 2023, max compression
```

## Comparing `molecule-plugins-23.0.0.tar` & `molecule-plugins-23.4.0.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.077611 molecule-plugins-23.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.077611 molecule-plugins-23.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.057610 molecule-plugins-23.0.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/doc/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/doc/ec2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/doc/ec2/platforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/doc/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/doc/vagrant/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/molecule/test-podman/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/molecule/test-podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/molecule/test-podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/molecule/test-podman/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/src/molecule_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-08 15:50:37.000000 molecule-plugins-23.0.0/src/molecule_plugins/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/src/molecule_plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/azure/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/containers/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/containers/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/containers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/docker/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/tasks/delete_network.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.085611 molecule-plugins-23.0.0/src/molecule_plugins/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/ec2/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/podman/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/podman/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.089611 molecule-plugins-23.0.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.061610 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/modules/vagrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.081611 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-08 15:50:37.000000 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-01-08 15:50:38.000000 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 15:50:37.000000 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-08 15:50:37.000000 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-08 15:50:37.000000 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-08 15:50:37.000000 molecule-plugins-23.0.0/src/molecule_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.069610 molecule-plugins-23.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/test/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/test/azure/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/functional/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/azure/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/azure/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.093611 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/azure/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/containers/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/functional/test_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/containers/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/containers/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/containers/scenarios/driver/containers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/containers/scenarios/driver/containers/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/containers/scenarios/driver/containers/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/scenarios/driver/containers/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/scenarios/driver/containers/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/containers/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/docker/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/docker/scenarios/env-substitution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/docker/scenarios/env-substitution/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/docker/scenarios/env-substitution/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/scenarios/env-substitution/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/scenarios/env-substitution/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/docker/scenarios/with-context/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/docker/scenarios/with-context/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/docker/scenarios/with-context/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/scenarios/with-context/molecule/default/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/scenarios/with-context/molecule/default/FOO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/scenarios/with-context/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/scenarios/with-context/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/docker/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.097612 molecule-plugins-23.0.0/test/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/ec2/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/functional/test_ec2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/ec2/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/ec2/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.065610 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/ec2/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/gce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/gce/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/functional/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.069610 molecule-plugins-23.0.0/test/gce/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/gce/scenarios/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.101612 molecule-plugins-23.0.0/test/gce/scenarios/linux/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/gce/scenarios/linux/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/handlers/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/gce/scenarios/linux/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/linux/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/gce/scenarios/windows/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/gce/scenarios/windows/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/gce/scenarios/windows/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/handlers/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/gce/scenarios/windows/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/scenarios/windows/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/gce/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/podman/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/podman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/podman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/podman/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/podman/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/vagrant/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/functional/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.069610 molecule-plugins-23.0.0/test/vagrant/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.069610 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/config_options/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/config_options/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/config_options/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/config_options/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.105612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/hostname/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/hostname/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/hostname/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/hostname/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/invalid/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/invalid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/multi-node/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/network/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/network/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/network/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/network/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/provider_config_options/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/provider_config_options/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/provider_config_options/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/vagrant_root/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/vagrant_root/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/test/vagrant/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 15:50:38.109612 molecule-plugins-23.0.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/tools/Vagrantfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/tools/create_testbox.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6414 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/tools/test-setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-08 15:50:16.000000 molecule-plugins-23.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.080648 molecule-plugins-23.4.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/doc/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/doc/ec2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/doc/ec2/platforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/doc/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/doc/vagrant/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.080648 molecule-plugins-23.4.0/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.128649 molecule-plugins-23.4.0/molecule/test-podman/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/molecule/test-podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/molecule/test-podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/molecule/test-podman/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:37:02.204650 molecule-plugins-23.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.080648 molecule-plugins-23.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.128649 molecule-plugins-23.4.0/src/molecule_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 13:37:01.000000 molecule-plugins-23.4.0/src/molecule_plugins/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.084648 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.084648 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.084648 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/delete_network.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.088648 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.088648 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.092648 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.096648 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/vagrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.112648 molecule-plugins-23.4.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/test/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/test/azure/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/functional/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.096648 molecule-plugins-23.4.0/test/azure/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/azure/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.164649 molecule-plugins-23.4.0/test/containers/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/test_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/containers/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/containers/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.164649 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.164649 molecule-plugins-23.4.0/test/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.168649 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/with-context/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.168649 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/FOO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.168649 molecule-plugins-23.4.0/test/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/test_ec2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.176649 molecule-plugins-23.4.0/test/gce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.176649 molecule-plugins-23.4.0/test/gce/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.112648 molecule-plugins-23.4.0/test/gce/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/handlers/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/handlers/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.188649 molecule-plugins-23.4.0/test/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.188649 molecule-plugins-23.4.0/test/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.188649 molecule-plugins-23.4.0/test/vagrant/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/functional/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.112648 molecule-plugins-23.4.0/test/vagrant/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.116648 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.192649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.192649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.192649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/invalid/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/invalid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tools/Vagrantfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tools/create_testbox.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6414 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tools/test-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tox.ini
```

### Comparing `molecule-plugins-23.0.0/.github/workflows/release.yml` & `molecule-plugins-23.4.0/.github/workflows/release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 
     env:
       FORCE_COLOR: 1
       PY_COLORS: 1
       TOX_PARALLEL_NO_SPINNER: 1
 
     steps:
-    - name: Switch to using Python 3.9 by default
-      uses: actions/setup-python@v4
-      with:
-        python-version: 3.9
-
-    - name: Install tox
-      run: >-
-        python3 -m
-        pip install
-        --user
-        tox
-
-    - name: Check out src from Git
-      uses: actions/checkout@v3
-      with:
-        fetch-depth: 0  # needed by setuptools-scm
-
-    - name: Build dists
-      run: python -m tox -e pkg
-
-    - name: Publish to pypi.org
-      if: >-  # "create" workflows run separately from "push" & "pull_request"
-        github.event_name == 'release'
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.pypi_password }}
+      - name: Switch to using Python 3.9 by default
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.9
+
+      - name: Install tox
+        run: >-
+          python3 -m
+          pip install
+          --user
+          tox
+
+      - name: Check out src from Git
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0 # needed by setuptools-scm
+
+      - name: Build dists
+        run: python -m tox -e pkg
+
+      - name: Publish to pypi.org
+        if: >- # "create" workflows run separately from "push" & "pull_request"
+          github.event_name == 'release'
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.pypi_password }}
```

### Comparing `molecule-plugins-23.0.0/.github/workflows/tox.yml` & `molecule-plugins-23.4.0/.github/workflows/tox.yml`

 * *Files 11% similar despite different names*

```diff
@@ -40,20 +40,14 @@
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
 
-      - name: Install system dependencies
-        run: |
-          sudo apt-get update \
-          && sudo apt-get install -y  ansible \
-          && ansible-doc -l | grep gce
-
       - name: Install Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python_version }}
 
       - name: Install dependencies
         run: |
```

### Comparing `molecule-plugins-23.0.0/.gitignore` & `molecule-plugins-23.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/.pre-commit-config.yaml` & `molecule-plugins-23.4.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -7,36 +7,46 @@
   (?x)^(
     src/molecule_plugins/_version.py
   )$
 default_language_version:
   python: python3
 minimum_pre_commit_version: "1.14.0"
 repos:
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    # keep it before yamllint
+    rev: "v3.0.0-alpha.6"
+    hooks:
+      - id: prettier
+        # Temporary excludes so we can gradually normalize the formatting
+        exclude: >
+          (?x)^(
+            .*\.md|
+            .*\{\{.*
+          )$
   - repo: https://github.com/PyCQA/doc8.git
     rev: v1.1.1
     hooks:
       - id: doc8
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.262"
     hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-black
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/ansible/ansible-lint.git
-    rev: v6.10.2
+    rev: v6.14.6
     hooks:
       - id: ansible-lint
```

### Comparing `molecule-plugins-23.0.0/LICENSE` & `molecule-plugins-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/PKG-INFO` & `molecule-plugins-23.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugins
-Version: 23.0.0
+Version: 23.4.0
 Summary: Molecule Plugins
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 Maintainer-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule-plugins
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule-plugins
@@ -15,41 +15,46 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: azure
 Provides-Extra: docker
 Provides-Extra: ec2
 Provides-Extra: gce
 Provides-Extra: podman
+Provides-Extra: selinux
 License-File: LICENSE
 
 # molecule-plugins
 
 This repository contains the following molecule plugins:
 
 - azure
+- containers
 - docker
+- ec2
 - gce
+- podman
+- vagrant
+
 
 Installing `molecule-plugins` does not install dependencies specific to each,
 plugin. To install these you need to install the extras for each plugin, like
 `pip3 install 'molecule-plugins[azure]'`.
 
 Before installing these plugins be sure that you uninstall their old standalone
 packages, like `pip3 uninstall molecule-azure`. If you fail to do so, you will
```

### Comparing `molecule-plugins-23.0.0/bindep.txt` & `molecule-plugins-23.4.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/conftest.py` & `molecule-plugins-23.4.0/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import contextlib
 import os
 import random
 import string
 
 import pytest
+
 from molecule import config, logger, util
 from molecule.scenario import ephemeral_directory
 
 LOG = logger.get_logger(__name__)
 
 
 @pytest.helpers.register
@@ -19,36 +20,36 @@
     return util.run_command(cmd, env=env)
 
 
 def _rebake_command(cmd, env, out=LOG.info, err=LOG.error):
     return cmd.bake(_env=env, _out=out, _err=err)
 
 
-@pytest.fixture
+@pytest.fixture()
 def random_string(length=5):
-    return "".join((random.choice(string.ascii_uppercase) for _ in range(length)))
+    return "".join(random.choice(string.ascii_uppercase) for _ in range(length))
 
 
 @contextlib.contextmanager
 def change_dir_to(dir_name):
     cwd = os.getcwd()
     os.chdir(dir_name)
     yield
     os.chdir(cwd)
 
 
-@pytest.fixture
+@pytest.fixture()
 def temp_dir(tmpdir, random_string, request):
     directory = tmpdir.mkdir(random_string)
 
     with change_dir_to(directory.strpath):
         yield directory
 
 
-@pytest.fixture
+@pytest.fixture()
 def resources_folder_path():
     resources_folder_path = os.path.join(os.path.dirname(__file__), "resources")
     return resources_folder_path
 
 
 @pytest.helpers.register
 def molecule_project_directory():
@@ -73,13 +74,13 @@
 @pytest.helpers.register
 def get_molecule_file(path):
     return config.molecule_file(path)
 
 
 @pytest.helpers.register
 def molecule_ephemeral_directory(_fixture_uuid):
-    project_directory = "test-project-{}".format(_fixture_uuid)
+    project_directory = f"test-project-{_fixture_uuid}"
     scenario_name = "test-instance"
 
     return ephemeral_directory(
-        os.path.join("molecule_test", project_directory, scenario_name)
+        os.path.join("molecule_test", project_directory, scenario_name),
     )
```

### Comparing `molecule-plugins-23.0.0/doc/ec2/README.rst` & `molecule-plugins-23.4.0/doc/ec2/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/doc/ec2/platforms.rst` & `molecule-plugins-23.4.0/doc/ec2/platforms.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/doc/vagrant/README.rst` & `molecule-plugins-23.4.0/doc/vagrant/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/pyproject.toml` & `molecule-plugins-23.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "setuptools_scm[toml] >= 7.0.5", # required for "no-local-version" scheme
 
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dynamic = ["version"]
 name = "molecule-plugins"
 description = "Molecule Plugins"
 readme = "README.md"
 authors = [{ "name" = "Sorin Sbarnea", "email" = "sorin.sbarnea@gmail.com" }]
 maintainers = [{ "name" = "Sorin Sbarnea", "email" = "sorin.sbarnea@gmail.com" }]
 license = { text = "MIT" }
@@ -22,29 +22,28 @@
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS",
   "Operating System :: POSIX",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python",
   "Topic :: System :: Systems Administration",
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 keywords = ["ansible", "testing", "molecule", "plugin"]
 dependencies = [
     # molecule plugins are not allowed to mention Ansible as a direct dependency
-    "molecule >= 4.0",
+    "molecule >= 5.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/ansible-community/molecule-plugins"
 documentation = "https://molecule.readthedocs.io/"
 repository = "https://github.com/ansible-community/molecule-plugins"
 changelog = "https://github.com/ansible-community/molecule-plugins/releases"
@@ -64,22 +63,63 @@
     'selinux; sys_platform=="linux"',
     "docker >= 4.3.1",
     "requests"  # also required by docker
 ]
 ec2 = []
 gce = []
 podman = [
-    # selinux python module is needed as least by ansible-podman modules
-    # and allows us of isolated (default) virtualenvs. It does not avoid need
-    # to install the system selinux libraries but it will provide a clear
-    # message when user has to do that.
+]
+selinux = [
+    # selinux python module is needed as least by podman and docker on systems
+    # that do have selinux enabled and where code is running inside of an
+    # isolated (default) virtualenv. It does not avoid need to install the
+    # system selinux libraries but it will provide a clear message when user
+    # has to do that.
     'selinux; sys_platform=="linux2"',
     'selinux; sys_platform=="linux"',
 ]
 
+[tool.ruff]
+ignore = [
+  "E501", # we use black
+  # we deliberately ignore these:
+  "EM102",
+  # temporary disabled until we either fix them or decide to ignore them:
+  "A001",
+  "ANN",
+  "ARG",
+  "B006",
+  "B028",
+  "BLE",
+  "C901",
+  "D",
+  "DTZ",
+  "EXE",
+  "FBT",
+  "INP",
+  "ISC",
+  "N",
+  "PGH",
+  "PLR",
+  "PT",
+  "PTH",
+  "RET",
+  "S",
+  "TRY",
+]
+select = ["ALL"]
+target-version = "py39"
+# Same as Black.
+line-length = 88
+
+[tool.ruff.flake8-pytest-style]
+parametrize-values-type = "tuple"
+
+[tool.ruff.isort]
+known-first-party = ["molecule_plugins"]
 
 [project.entry-points."molecule.driver"]
 azure = "molecule_plugins.azure.driver:Azure"
 containers = "molecule_plugins.containers.driver:Container"
 docker = "molecule_plugins.docker.driver:Docker"
 ec2 = "molecule_plugins.ec2.driver:EC2"
 gce = "molecule_plugins.gce.driver:GCE"
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,40 +11,40 @@
     ssh_user: molecule
     ssh_port: 22
     virtual_network_name: molecule_vnet
     subnet_name: molecule_subnet
     keypair_path: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}/ssh_key"
   tasks:
     - name: Create resource group
-      azure_rm_resourcegroup:
+      azure.azcollection.azure_rm_resourcegroup:
         name: "{{ resource_group_name }}"
         location: "{{ location }}"
 
     - name: Create virtual network
-      azure_rm_virtualnetwork:
+      azure.azcollection.azure_rm_virtualnetwork:
         resource_group: "{{ resource_group_name }}"
         name: "{{ virtual_network_name }}"
         address_prefixes: "10.10.0.0/16"
 
     - name: Create subnet
-      azure_rm_subnet:
+      azure.azcollection.azure_rm_subnet:
         resource_group: "{{ resource_group_name }}"
         name: "{{ subnet_name }}"
         address_prefix_cidr: 10.10.1.0/24
         virtual_network_name: "{{ virtual_network_name }}"
 
     - name: Create key pair
-      user:
+      ansible.builtin.user:
         name: "{{ lookup('env', 'USER') }}"
         generate_ssh_key: true
         ssh_key_file: "{{ keypair_path }}"
       register: key_pair
 
     - name: Create molecule instance(s)
-      azure_rm_virtualmachine:
+      azure.azcollection.azure_rm_virtualmachine:
         resource_group: "{{ resource_group_name }}"
         name: "{{ item.name }}"
         vm_size: Standard_A0
         admin_username: "{{ ssh_user }}"
         public_ip_allocation_method: Dynamic
         ssh_password_enabled: false
         ssh_public_keys:
@@ -57,48 +57,55 @@
           version: latest
       register: server
       with_items: "{{ molecule_yml.platforms }}"
       async: 7200
       poll: 0
 
     - name: Wait for instance(s) creation to complete
-      async_status:
+      ansible.builtin.async_status:
         jid: "{{ item.ansible_job_id }}"
       register: azure_jobs
       until: azure_jobs.finished
       retries: 300
       with_items: "{{ server.results }}"
+      notify:
+        - Populate instance config dict
+        - Convert instance config dict to a list
+        - Dump instance config
+        - Wait for SSH
 
-
-    # Mandatory configuration for Molecule to function.
-
+  handlers:
     - name: Populate instance config dict
-      set_fact:
-        instance_conf_dict: {
-          'instance': "{{ item.ansible_facts.azure_vm.name }}",
-          'address': "{{ item.ansible_facts.azure_vm.properties.networkProfile.networkInterfaces[0].properties.ipConfigurations[0].properties.publicIPAddress.properties.ipAddress }}",
-          'user': "{{ ssh_user }}",
-          'port': "{{ ssh_port }}",
-          'identity_file': "{{ keypair_path }}", }
+      ansible.builtin.set_fact:
+        instance_conf_dict:
+          {
+            "instance": "{{ item.ansible_facts.azure_vm.name }}",
+            "address": "{{ item.ansible_facts.azure_vm
+              .properties.networkProfile.networkInterfaces[0]
+              .properties.ipConfigurations[0]
+              .properties.publicIPAddress
+              .properties.ipAddress }}",
+            "user": "{{ ssh_user }}",
+            "port": "{{ ssh_port }}",
+            "identity_file": "{{ keypair_path }}",
+          }
       with_items: "{{ azure_jobs.results }}"
       register: instance_config_dict
-      when: server.changed | bool
 
     - name: Convert instance config dict to a list
-      set_fact:
+      ansible.builtin.set_fact:
         instance_conf: "{{ instance_config_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
-      when: server.changed | bool
 
     - name: Dump instance config
-      copy:
-        content: "{{ instance_conf | to_json | from_json | molecule_to_yaml | molecule_header }}"
+      ansible.builtin.copy:
+        content: "{{ instance_conf | to_json | from_json | to_yaml }}"
         dest: "{{ molecule_instance_config }}"
-      when: server.changed | bool
+        mode: 0664
 
     - name: Wait for SSH
-      wait_for:
+      ansible.builtin.wait_for:
         port: "{{ ssh_port }}"
         host: "{{ item.address }}"
         search_regex: SSH
         delay: 10
-      with_items: "{{ lookup('file', molecule_instance_config) | molecule_from_yaml }}"
+      with_items: "{{ instance_conf }}"
 {%- endraw %}
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files 24% similar despite different names*

```diff
@@ -7,25 +7,26 @@
   no_log: "{{ molecule_no_log }}"
   vars:
     resource_group_name: molecule
     virtual_network_name: molecule_vnet
     subnet_name: molecule_subnet
   tasks:
     - name: Destroy resource group and all associated resources
-      azure_rm_resourcegroup:
+      azure.azcollection.azure_rm_resourcegroup:
         name: "{{ resource_group_name }}"
         state: absent
         force_delete_nonempty: true
       register: rg
-
-    # Mandatory configuration for Molecule to function.
+      notify:
+        - Dump instance config
 
     - name: Populate instance config
-      set_fact:
+      ansible.builtin.set_fact:
         instance_conf: {}
 
+  handlers:
     - name: Dump instance config
-      copy:
-        content: "{{ instance_conf | to_json | from_json | molecule_to_yaml | molecule_header }}"
+      ansible.builtin.copy:
+        content: "{{ instance_conf | to_json | from_json | to_yaml }}"
         dest: "{{ molecule_instance_config }}"
-      when: rg.changed | bool
+        mode: 0644
 {%- endraw %}
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/azure/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/azure/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 import os
-from molecule import logger
-from molecule.api import Driver
 
-from molecule import util
+from molecule import logger, util
+from molecule.api import Driver
 
 LOG = logger.get_logger(__name__)
 
 
 class Azure(Driver):
     """
     The class responsible for managing `Azure`_ instances.  `Azure`_
@@ -68,18 +67,18 @@
 
         driver:
           name: azure
           safe_files:
             - foo
 
     .. _`Azure`: https://azure.microsoft.com
-    """  # noqa
+    """
 
-    def __init__(self, config=None):
-        super(Azure, self).__init__(config)
+    def __init__(self, config=None) -> None:
+        super().__init__(config)
         self._name = "azure"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -121,15 +120,15 @@
                 "ansible_port": d["port"],
                 "ansible_private_key_file": d["identity_file"],
                 "connection": "ssh",
                 "ansible_ssh_common_args": " ".join(self.ssh_connection_options),
             }
         except StopIteration:
             return {}
-        except IOError:
+        except OSError:
             # Instance has yet to be provisioned , therefore the
             # instance_config is not on disk.
             return {}
 
     def _get_instance_config(self, instance_name):
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/containers/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/containers/driver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Containers Driver Module."""
-from __future__ import absolute_import
 
 import inspect
 import os
 import shutil
-from typing import Dict
 
 from molecule import logger
 
 _logger = logger.get_logger(__name__)
 
 # Preference logic for picking backend driver to be used.
 drivers = os.environ.get("MOLECULE_CONTAINERS_BACKEND", "podman,docker").split(",")
@@ -30,25 +28,25 @@
 
 class Container(DriverBackend):
     """
     Container Driver Class.
 
     This class aims to provide an agnostic container enginer implementation,
     which should allow users to consume whichever enginer they have available.
-    """  # noqa
+    """
 
-    def __init__(self, config=None):
+    def __init__(self, config=None) -> None:
         """Construct Container."""
         super().__init__(config)
         self._name = "containers"
         # Assure that _path points to the driver we would be using, or
         # molecule will fail to find the embedded playbooks.
         self._path = os.path.abspath(os.path.dirname(inspect.getfile(DriverBackend)))
 
     @property
-    def required_collections(self) -> Dict[str, str]:
+    def required_collections(self) -> dict[str, str]:
         """Return collections dict containing names and versions required."""
         return {
             "ansible.posix": "1.3.0",
             "community.docker": "1.9.1",
             "containers.podman": "1.8.1",
         }
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Docker Driver Module."""
 
-from __future__ import absolute_import
 
 import os
-from typing import Dict
 
 from molecule import logger
 from molecule.api import Driver
 from molecule.util import sysexit_with_message
 
 log = logger.get_logger(__name__)
 
@@ -183,21 +181,21 @@
           name: docker
           safe_files:
             - foo
 
     .. _`Docker`: https://www.docker.com
     .. _`systemd`: https://www.freedesktop.org/wiki/Software/systemd/
     .. _`CMD`: https://docs.docker.com/engine/reference/builder/#cmd
-    """  # noqa
+    """
 
     _passed_sanity = False
 
-    def __init__(self, config=None):
+    def __init__(self, config=None) -> None:
         """Construct Docker."""
-        super(Docker, self).__init__(config)
+        super().__init__(config)
         self._name = "docker"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -265,11 +263,11 @@
         for c in result.get("ContainersDeleted") or []:
             log.info("Deleted container %s", c)
         for n in client.networks.list(filters={"label": "owner=molecule"}):
             log.info("Removing docker network %s ...", n.name)
             n.remove()
 
     @property
-    def required_collections(self) -> Dict[str, str]:
+    def required_collections(self) -> dict[str, str]:
         """Return collections dict containing names and versions required."""
         # https://galaxy.ansible.com/community/docker
         return {"community.docker": "3.0.2", "ansible.posix": "1.4.0"}
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2` & `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/create.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   vars:
     molecule_labels:
       owner: molecule
+  tags:
+    - always
   tasks:
     - name: Set async_dir for HOME env
       ansible.builtin.set_fact:
         ansible_async_dir: "{{ lookup('env', 'HOME') }}/.ansible_async/"
       when: (lookup('env', 'HOME'))
 
     - name: Log into a Docker registry
@@ -78,15 +80,15 @@
         key_path: "{{ item.key_path | default((lookup('env', 'DOCKER_CERT_PATH') + '/key.pem') if lookup('env', 'DOCKER_CERT_PATH') else omit) }}"
         tls_verify: "{{ item.tls_verify | default(lookup('env', 'DOCKER_TLS_VERIFY')) or false }}"
       with_items: "{{ platforms.results }}"
       when:
         - not item.pre_build_image | default(false)
       register: docker_images
 
-    - name: Build an Ansible compatible image (new)  # noqa: no-handler
+    - name: Build an Ansible compatible image (new) # noqa: no-handler
       when:
         - platforms.changed or docker_images.results | map(attribute='images') | select('equalto', []) | list | count >= 0
         - not item.item.pre_build_image | default(false)
       community.docker.docker_image:
         build:
           path: "{{ molecule_ephemeral_directory }}"
           dockerfile: "{{ item.invocation.module_args.dest }}"
@@ -170,14 +172,17 @@
         restart_retries: "{{ item.restart_retries | default(omit) }}"
         tty: "{{ item.tty | default(omit) }}"
         labels: "{{ molecule_labels | combine(item.labels | default({})) }}"
         container_default_behavior: "{{ item.container_default_behavior | default('compatibility' if ansible_version.full is version_compare('2.10', '>=') else omit) }}"
         stop_signal: "{{ item.stop_signal | default(omit) }}"
         kill_signal: "{{ item.kill_signal | default(omit) }}"
         cgroupns_mode: "{{ item.cgroupns_mode | default(omit) }}"
+        platform: "{{ item.platform | default(omit) }}"
+        comparisons:
+          platform: ignore
       register: server
       with_items: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
       no_log: false
       async: 7200
       poll: 0
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/destroy.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/destroy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ---
 - name: Destroy
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
+  tags:
+    - always
   tasks:
     - name: Set async_dir for HOME env
       ansible.builtin.set_fact:
         ansible_async_dir: "{{ lookup('env', 'HOME') }}/.ansible_async/"
       when: (lookup('env', 'HOME'))
 
     - name: Destroy molecule instance(s)
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,14 @@
                 if "name" in network:
                     name = network["name"]
                     if name not in network_names:
                         network_list.append({"name": name, "labels": labels})
     return network_list
 
 
-class FilterModule(object):
+class FilterModule:
     """Core Molecule filter plugins."""
 
     def filters(self):
         return {
             "molecule_get_docker_networks": get_docker_networks,
         }
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     platforms:
       # platforms supported as being managed by molecule/ansible, this does
       # not mean molecule itself can run on them.
       - image: alpine:edge
       - image: quay.io/centos/centos:stream8
       - image: ubuntu:latest
       - image: debian:latest
+  tags:
+    - always
   tasks:
-
     - name: Assure we have docker module installed
       ansible.builtin.pip:
         name: docker
 
     - name: Create temporary dockerfiles
       ansible.builtin.tempfile:
         prefix: "molecule-dockerfile-{{ item.image | replace('/', '-') }}"
@@ -27,15 +28,15 @@
       loop_control:
         label: "{{ item.image }}"
 
     - name: Expand Dockerfile templates
       ansible.builtin.template:
         src: Dockerfile.j2
         dest: "{{ temp_dockerfiles.results[index].path }}"
-        mode: 0600
+        mode: "0600"
       register: result
       with_items: "{{ platforms }}"
       loop_control:
         index_var: index
         label: "{{ item.image }}"
 
     - name: Test Dockerfile template
@@ -55,13 +56,13 @@
         label: "{{ item.item.image }}"
       register: result
 
     - name: Clean up temporary Dockerfile's
       ansible.builtin.file:
         path: "{{ item }}"
         state: absent
-        mode: 0600
+        mode: "0600"
       loop: "{{ temp_dockerfiles.results | map(attribute='path') | list }}"
 
     - name: Display results
       ansible.builtin.debug:
         var: result
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         security_groups: "{{ platform_security_groups }}"
         network:
           assign_public_ip: "{{ item.assign_public_ip }}"
         volumes: "{{ item.volumes }}"
         key_name: "{{ (item.key_inject_method == 'ec2') | ternary(item.key_name, omit) }}"
         tags: "{{ platform_tags }}"
         user_data: "{{ platform_user_data }}"
-        state: "started"
+        state: "running"
         wait: true
       vars:
         platform_security_groups: "{{ item.security_groups or [item.security_group_name] }}"
         platform_generated_image_id: "{{ (ami_info.results[index].images | sort(attribute='creation_date', reverse=True))[0].image_id }}"
         platform_image_id: "{{ item.image or platform_generated_image_id }}"
 
         platform_generated_cloud_config:
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/ec2/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/ec2/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from base64 import b64decode
 import os
 import sys
+from base64 import b64decode
 
 try:
     from cryptography.hazmat.backends import default_backend
     from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
     from cryptography.hazmat.primitives.serialization import load_pem_private_key
 
     HAS_CRYPTOGRAPHY = True
@@ -34,19 +34,17 @@
 try:
     import boto3
 
     HAS_BOTO3 = True
 except ImportError:
     HAS_BOTO3 = False
 
-from molecule import logger
+from molecule import logger, util
 from molecule.api import Driver
 
-from molecule import util
-
 LOG = logger.get_logger(__name__)
 
 
 class EC2(Driver):
     """
     The class responsible for managing `EC2`_ instances.  `EC2`_
     is ``not`` the default driver used in Molecule.
@@ -149,18 +147,18 @@
 
         driver:
           name: ec2
           safe_files:
             - foo
 
     .. _`EC2`: https://aws.amazon.com/ec2/
-    """  # noqa
+    """
 
-    def __init__(self, config=None):
-        super(EC2, self).__init__(config)
+    def __init__(self, config=None) -> None:
+        super().__init__(config)
         self._name = "ec2"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -177,21 +175,20 @@
             LOG.error("Please specify instance via '--host'")
             sys.exit(1)
 
         ansible_connection_options = self.ansible_connection_options(hostname)
         if ansible_connection_options.get("ansible_connection") == "winrm":
             return (
                 "xfreerdp "
-                '"/u:%s" '
-                '"/p:%s" '
-                "/v:%s "
+                '"/u:{}" '
+                '"/p:{}" '
+                "/v:{} "
                 "/cert-tofu "
                 "+clipboard "
-                "/grab-keyboard"
-                % (
+                "/grab-keyboard".format(
                     ansible_connection_options["ansible_user"],
                     ansible_connection_options["ansible_password"],
                     ansible_connection_options["ansible_host"],
                 )
             )
 
         else:  # normal ssh connection
@@ -240,20 +237,21 @@
                 },
                 plat_conn_opts,
             )
             if conn_opts.get("ansible_connection") == "winrm" and (
                 not conn_opts.get("ansible_password")
             ):
                 conn_opts["ansible_password"] = self._get_windows_instance_pass(
-                    d["instance_ids"][0], d["identity_file"]
+                    d["instance_ids"][0],
+                    d["identity_file"],
                 )
             return conn_opts
         except StopIteration:
             return {}
-        except IOError:
+        except OSError:
             # Instance has yet to be provisioned , therefore the
             # instance_config is not on disk.
             return {}
 
     def _get_instance_config(self, instance_name):
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/driver.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
-from typing import Dict
 import os
-from molecule import logger
-from molecule.api import Driver
 
-from molecule import util
+from molecule import logger, util
+from molecule.api import Driver
 
 LOG = logger.get_logger(__name__)
 
 
 class GCE(Driver):
     """
     The class responsible for managing `GCE`_ instances.  `GCE`_
@@ -73,18 +71,18 @@
 
         driver:
           name: gce
           safe_files:
             - foo
 
     .. _`GCE`: https://cloud.google.com/compute/docs/
-    """  # noqa
+    """
 
-    def __init__(self, config=None):
-        super(GCE, self).__init__(config)
+    def __init__(self, config=None) -> None:
+        super().__init__(config)
         self._name = "gce"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -125,15 +123,15 @@
                     return {
                         "ansible_user": d["user"],
                         "ansible_host": d["address"],
                         "ansible_port": d["port"],
                         "ansible_private_key_file": d["identity_file"],
                         "ansible_connection": "ssh",
                         "ansible_ssh_common_args": " ".join(
-                            self.ssh_connection_options
+                            self.ssh_connection_options,
                         ),
                     }
 
                 if d["instance_os_type"] == "windows":
                     return {
                         "ansible_user": d["user"],
                         "ansible_host": d["address"],
@@ -144,15 +142,15 @@
                         "ansible_winrm_server_cert_validation": d[
                             "winrm_server_cert_validation"
                         ],
                         "ansible_become_method": "runas",
                     }
         except StopIteration:
             return {}
-        except IOError:
+        except OSError:
             # Instance has yet to be provisioned , therefore the
             # instance_config is not on disk.
             return {}
 
     def _get_instance_config(self, instance_name):
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
 
@@ -167,10 +165,10 @@
     def template_dir(self):
         """Return path to its own cookiecutterm templates. It is used by init
         command in order to figure out where to load the templates from.
         """
         return os.path.join(os.path.dirname(__file__), "cookiecutter")
 
     @property
-    def required_collections(self) -> Dict[str, str]:
+    def required_collections(self) -> dict[str, str]:
         # https://galaxy.ansible.com/google/cloud
         return {"google.cloud": "1.0.2", "community.crypto": "1.8.0"}
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/create.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/destroy.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import argparse
 import base64
 import copy
 import datetime
 import json
 import time
-import argparse
+
+# Google API Client Library for Python:
+# https://developers.google.com/api-client-library/python/start/get_started
+import google.auth
 
 # PyCrypto library: https://pypi.python.org/pypi/pycrypto
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.PublicKey import RSA
 from Crypto.Util.number import long_to_bytes
-
-# Google API Client Library for Python:
-# https://developers.google.com/api-client-library/python/start/get_started
-import google.auth
 from googleapiclient.discovery import build
 
 
 def GetCompute():
     """Get a compute object for communicating with the Compute Engine API."""
     credentials, project = google.auth.default()
     compute = build("compute", "v1", credentials=credentials)
@@ -72,15 +72,14 @@
     # between the time on the client and the time on the server.
     expire_time = utc_now + datetime.timedelta(minutes=5)
     return expire_time.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
 def GetJsonString(user, modulus, exponent, email):
     """Return the JSON string object that represents the windows-keys entry."""
-
     converted_modulus = modulus.decode("utf-8")
     converted_exponent = exponent.decode("utf-8")
 
     expire = GetExpirationTimeString()
     data = {
         "userName": user,
         "modulus": converted_modulus,
@@ -101,25 +100,31 @@
     new_metadata["items"] = [{"key": "windows-keys", "value": metadata_entry}]
     return new_metadata
 
 
 def UpdateInstanceMetadata(compute, instance, zone, project, new_metadata):
     """Update the instance metadata."""
     cmd = compute.instances().setMetadata(
-        instance=instance, project=project, zone=zone, body=new_metadata
+        instance=instance,
+        project=project,
+        zone=zone,
+        body=new_metadata,
     )
     return cmd.execute()
 
 
 def GetSerialPortFourOutput(compute, instance, zone, project):
     """Get the output from serial port 4 from the instance."""
     # Encrypted passwords are printed to COM4 on the windows server:
     port = 4
     cmd = compute.instances().getSerialPortOutput(
-        instance=instance, project=project, zone=zone, port=port
+        instance=instance,
+        project=project,
+        zone=zone,
+        port=port,
     )
     output = cmd.execute()
     return output["contents"]
 
 
 def GetEncryptedPasswordFromSerialPort(serial_port_output, modulus):
     """Find and return the correct encrypted password, based on the modulus."""
@@ -132,68 +137,79 @@
     for line in reversed(output):
         try:
             entry = json.loads(line)
             if converted_modulus == entry["modulus"]:
                 return entry["encryptedPassword"]
         except ValueError:
             pass
+    return None
 
 
 def DecryptPassword(encrypted_password, key):
     """Decrypt a base64 encoded encrypted password using the provided key."""
-
     decoded_password = base64.b64decode(encrypted_password)
     cipher = PKCS1_OAEP.new(key)
     password = cipher.decrypt(decoded_password)
     return password
 
 
 def Arguments():
     # Create the parser
     args = argparse.ArgumentParser(description="List the content of a folder")
 
     # Add the arguments
     args.add_argument(
-        "--instance", metavar="instance", type=str, help="compute instance name"
+        "--instance",
+        metavar="instance",
+        type=str,
+        help="compute instance name",
     )
 
     args.add_argument("--zone", metavar="zone", type=str, help="compute zone")
 
     args.add_argument("--project", metavar="project", type=str, help="gcp project")
 
     args.add_argument("--username", metavar="username", type=str, help="username")
 
     args.add_argument("--email", metavar="email", type=str, help="email")
 
-    # return arguments
     return args.parse_args()
 
 
 def main():
     config_args = Arguments()
 
     # Setup
     compute = GetCompute()
     key = GetKey()
     modulus, exponent = GetModulusExponentInBase64(key)
 
     # Get existing metadata
     instance_ref = GetInstance(
-        compute, config_args.instance, config_args.zone, config_args.project
+        compute,
+        config_args.instance,
+        config_args.zone,
+        config_args.project,
     )
     old_metadata = instance_ref["metadata"]
     # Create and set new metadata
     metadata_entry = GetJsonString(
-        config_args.username, modulus, exponent, config_args.email
+        config_args.username,
+        modulus,
+        exponent,
+        config_args.email,
     )
     new_metadata = UpdateWindowsKeys(old_metadata, metadata_entry)
 
     # Get Serial output BEFORE the modification
     serial_port_output = GetSerialPortFourOutput(
-        compute, config_args.instance, config_args.zone, config_args.project
+        compute,
+        config_args.instance,
+        config_args.zone,
+        config_args.project,
     )
 
     UpdateInstanceMetadata(
         compute,
         config_args.instance,
         config_args.zone,
         config_args.project,
@@ -202,23 +218,26 @@
 
     # Get and decrypt password from serial port output
     # Monitor changes from output to get the encrypted password as soon as it's generated, will wait for 30 seconds
     i = 0
     new_serial_port_output = serial_port_output
     while i <= 20 and serial_port_output == new_serial_port_output:
         new_serial_port_output = GetSerialPortFourOutput(
-            compute, config_args.instance, config_args.zone, config_args.project
+            compute,
+            config_args.instance,
+            config_args.zone,
+            config_args.project,
         )
         i += 1
         time.sleep(3)
 
     enc_password = GetEncryptedPasswordFromSerialPort(new_serial_port_output, modulus)
 
     password = DecryptPassword(enc_password, key)
     converted_password = password.decode("utf-8")
 
     # Display only the password
-    print(format(converted_password))
+    print(format(converted_password))  # noqa: T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/handlers/main.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/handlers/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 ---
 - name: Populate instance config dict Linux
-  ansible.builtin.set_fact:
-    instance_conf_dict: {
-      'instance': "{{ instance_info.name }}",
-      'address': "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-      'user': "{{ lookup('env','USER') }}",
-      'port': "22",
-      'identity_file': "{{ ssh_identity_file }}",
-      'instance_os_type': "{{ molecule_yml.driver.instance_os_type }}"
-    }
+  set_fact:
+    instance_conf_dict:
+      {
+        "instance": "{{ instance_info.name }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "{{ lookup('env','USER') }}",
+        "port": "22",
+        "identity_file": "{{ ssh_identity_file }}",
+        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
+      }
   loop: "{{ server.results }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Populate instance config dict Windows
-  ansible.builtin.set_fact:
-    instance_conf_dict: {
-      'instance': "{{ instance_info.name }}",
-      'address': "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-      'user': "molecule_usr",
-      'password': "{{ instance_info.password }}",
-      'port': "{{ instance_info.winrm_port | default(5986) }}",
-      'winrm_transport': "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
-      'winrm_server_cert_validation': "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
-      'instance_os_type': "{{ molecule_yml.driver.instance_os_type }}"
-    }
+  set_fact:
+    instance_conf_dict:
+      {
+        "instance": "{{ instance_info.name }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "molecule_usr",
+        "password": "{{ instance_info.password }}",
+        "port": "{{ instance_info.winrm_port | default(5986) }}",
+        "winrm_transport": "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
+        "winrm_server_cert_validation": "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
+        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
+      }
   loop: "{{ win_instances }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
-
 - name: Wipe out instance config
-  ansible.builtin.set_fact:
+  set_fact:
     instance_conf: {}
 
 - name: Convert instance config dict to a list
-  ansible.builtin.set_fact:
+  set_fact:
     instance_conf: "{{ instance_conf_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
 - name: Dump instance config
-  ansible.builtin.copy:
+  copy:
     content: "{{ instance_conf }}"
     dest: "{{ molecule_instance_config }}"
-    mode: '0600'
+    mode: "0600"
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-- name: create ssh keypair
+- name: Create ssh keypair
   community.crypto.openssh_keypair:
     comment: "{{ lookup('env','USER') }} user for Molecule"
     path: "{{ ssh_identity_file }}"
   register: keypair
 
-- name: create molecule Linux instance(s)
+- name: "Create molecule Linux instance(s)"
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     metadata:
       ssh-keys: "{{ lookup('env','USER') }}:{{ keypair.public_key }}"
     scheduling:
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-- name: create molecule Windows instance(s)
+- name: Create molecule Windows instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     scheduling:
       preemptible: "{{ item.preemptible | default(false) }}"
     disks:
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/podman/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/podman/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Podman Driver Module."""
 
-from __future__ import absolute_import
 
 import os
 import warnings
 from shutil import which
-from typing import Dict
 
 from ansible_compat.runtime import Runtime
+from packaging.version import Version
+
 from molecule import logger, util
 from molecule.api import Driver, MoleculeRuntimeWarning
 from molecule.constants import RC_SETUP_ERROR
 from molecule.util import sysexit_with_message
-from packaging.version import Version
 
 log = logger.get_logger(__name__)
 
 
 class Podman(Driver):
     """
     The class responsible for managing `Podman`_ containers.
@@ -151,17 +150,17 @@
           name: podman
           safe_files:
             - foo
 
     .. _`Podman`: https://podman.io/
     .. _`systemd`: https://www.freedesktop.org/wiki/Software/systemd/
     .. _`CMD`: https://docs.docker.com/engine/reference/builder/#cmd
-    """  # noqa
+    """
 
-    def __init__(self, config=None):
+    def __init__(self, config=None) -> None:
         """Construct Podman."""
         super().__init__(config)
         self._name = "podman"
         # To change the podman executable, set environment variable
         # MOLECULE_PODMAN_EXECUTABLE
         # An example could be MOLECULE_PODMAN_EXECUTABLE=podman-remote
         self.podman_exec = os.environ.get("MOLECULE_PODMAN_EXECUTABLE", "podman")
@@ -220,15 +219,14 @@
             return
 
         log.info("Sanity checks: '%s'", self._name)
         # TODO(ssbarnea): reuse ansible runtime instance from molecule once it
         # fully adopts ansible-compat
         runtime = Runtime()
         if runtime.version < Version("2.10.0"):
-
             if runtime.config.ansible_pipelining:
                 sysexit_with_message(
                     "Podman connections do not work with Ansible "
                     f"{runtime.version} when pipelining is enabled. "
                     "Disable pipelining or "
                     "upgrade Ansible to 2.11 or newer.",
                     code=RC_SETUP_ERROR,
@@ -238,10 +236,10 @@
                 "unsupported, upgrade to Ansible 2.11 or newer. "
                 "Do not raise any bugs if your tests are failing with current configuration.",
                 category=MoleculeRuntimeWarning,
             )
         self._sanity_passed = True
 
     @property
-    def required_collections(self) -> Dict[str, str]:
+    def required_collections(self) -> dict[str, str]:
         """Return collections dict containing names and versions required."""
         return {"containers.podman": "1.7.0", "ansible.posix": "1.3.0"}
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2` & `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2`

 * *Files 15% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 {% for var, value in item.env.items() %}
 {% if value %}
 ENV {{ var }} {{ value }}
 {% endif %}
 {% endfor %}
 {% endif %}
 
-RUN if [ $(command -v apt-get) ]; then export DEBIAN_FRONTEND=noninteractive && apt-get update && apt-get install -y python3 sudo bash ca-certificates iproute2 python3-apt aptitude && apt-get clean && rm -rf /var/lib/apt/lists/*; \
-    elif [ $(command -v dnf) ]; then dnf makecache && dnf --assumeyes install /usr/bin/python3 /usr/bin/python3-config /usr/bin/dnf-3 sudo bash iproute && dnf clean all; \
-    elif [ $(command -v yum) ]; then yum makecache fast && yum install -y /usr/bin/python /usr/bin/python2-config sudo yum-plugin-ovl bash iproute && sed -i 's/plugins=0/plugins=1/g' /etc/yum.conf && yum clean all; \
-    elif [ $(command -v zypper) ]; then zypper refresh && zypper install -y python3 sudo bash iproute2 && zypper clean -a; \
-    elif [ $(command -v apk) ]; then apk update && apk add --no-cache python3 sudo bash ca-certificates; \
-    elif [ $(command -v xbps-install) ]; then xbps-install -Syu && xbps-install -y python3 sudo bash ca-certificates iproute2 && xbps-remove -O; fi
+RUN if [ $(command -v apt-get) ]; then export DEBIAN_FRONTEND=noninteractive && apt-get update && apt-get install -y python3 sudo bash ca-certificates iproute2 python3-apt aptitude rsync && apt-get clean && rm -rf /var/lib/apt/lists/*; \
+    elif [ $(command -v dnf) ]; then dnf makecache && dnf --assumeyes install /usr/bin/python3 /usr/bin/python3-config /usr/bin/dnf-3 sudo bash iproute rsync && dnf clean all; \
+    elif [ $(command -v yum) ]; then yum makecache fast && yum install -y /usr/bin/python /usr/bin/python2-config sudo yum-plugin-ovl bash iproute rsync && sed -i 's/plugins=0/plugins=1/g' /etc/yum.conf && yum clean all; \
+    elif [ $(command -v zypper) ]; then zypper refresh && zypper install -y python3 sudo bash iproute2 rsync && zypper clean -a; \
+    elif [ $(command -v apk) ]; then apk update && apk add --no-cache python3 sudo bash ca-certificates rsync; \
+    elif [ $(command -v xbps-install) ]; then xbps-install -Syu && xbps-install -y python3 sudo bash ca-certificates iproute2 rsync && xbps-remove -O; fi
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/create.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   become: "{{ not (item.rootless|default(true)) }}"
   vars:
     podman_exec: "{{ lookup('env','MOLECULE_PODMAN_EXECUTABLE')|default('podman',true) }}"
   tasks:
-    - name: Get podman executable path  # noqa: command-instead-of-shell
+    - name: Get podman executable path # noqa: command-instead-of-shell
       ansible.builtin.shell: "command -v {{ podman_exec }}"
       register: _podman_path
       changed_when: false
 
     - name: Register podman executable path
       ansible.builtin.set_fact:
         podman_cmd: "{{ _podman_path.stdout }}"
@@ -35,14 +35,15 @@
         label: >-
           "{{ item.name }} registry username:
           {{ item.registry.credentials.username | default('None specified') }}"
       when:
         - item.registry is defined
         - item.registry.credentials is defined
         - item.registry.credentials.username is defined
+      changed_when: false
 
     - name: Check presence of custom Dockerfiles
       ansible.builtin.stat:
         path: "{{ molecule_scenario_directory + '/' + (item.dockerfile | default('Dockerfile.j2')) }}"
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "Dockerfile: {{ item.dockerfile | default('None specified') }}"
@@ -74,15 +75,15 @@
       with_items: "{{ platforms.results }}"
       loop_control:
         label: "{{ item.item.name | default('None specified') }}"
       when:
         - not item.pre_build_image | default(false)
       register: podman_images
 
-    - name: Build an Ansible compatible image  # noqa: no-handler
+    - name: Build an Ansible compatible image # noqa: no-handler
       ansible.builtin.command: >
         {{ podman_cmd }} build
         -f {{ item.dest }}
         -t molecule_local/{{ item.item.image }}
         {% if item.item.buildargs is defined %}{% for i, k in item.item.buildargs.items() %}--build-arg={{ i }}={{ k }}{% endfor %}{% endif %}
         {% if item.item.pull is defined %}--pull={{ item.item.pull }}{% endif %}
         {{ molecule_scenario_directory + '/' + (item.item.dockerfile | default( 'Dockerfile.j2')) | dirname }}
@@ -93,14 +94,15 @@
         - platforms.changed or podman_images.results | map(attribute='images') | select('equalto', []) | list | count >= 0
         - not item.item.pre_build_image | default(false)
       register: result
       until: result is not failed
       retries: 3
       delay: 30
       no_log: false
+      changed_when: false
 
     - name: Determine the CMD directives
       ansible.builtin.set_fact:
         command_directives_dict: >-
           {{ command_directives_dict | default({}) |
              combine({ item.name: item.command | default('bash -c "while true; do sleep 10000; done"') })
           }}
@@ -133,16 +135,15 @@
         - ansible_loop.first
       failed_when: false
 
     - name: Create podman network dedicated to this scenario
       containers.podman.podman_network:
         name: "{{ podman_network.results[0].ansible_loop.allitems[0].network }}"
         executable: "{{ podman_exec }}"
-        subnet:
-          "{{ podman_network.results[0].ansible_loop.allitems[0].subnet | default(omit) }}"
+        subnet: "{{ podman_network.results[0].ansible_loop.allitems[0].subnet | default(omit) }}"
       when:
         - podman_network.results[0].msg is defined
         # podman message changed at some point in time
         - "'no such network' in podman_network.results[0].msg or 'network not found' in podman_network.results[0].msg"
         - podman_network.results[0].networks is undefined
         - "podman_network.results[0].ansible_loop.allitems[0].network not in ['bridge', 'none', 'host', 'ns', 'private', 'slirp4netns']"
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/destroy.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 #!/usr/bin/env ansible-playbook
 ---
 - name: Validate dockerfile
   hosts: localhost
   connection: local
   gather_facts: false
-  collections:
-    - containers.podman
   vars:
     platforms:
       # platforms supported as being managed by molecule/ansible, this does
       # not mean molecule itself can run on them.
       - image: alpine:edge
       - image: centos:7
       # - image: centos:8
       - image: ubuntu:latest
       - image: debian:latest
   tasks:
-
     - name: Create isolated build directories for each image
       ansible.builtin.tempfile:
         prefix: "molecule-dockerfile-{{ item.image }}"
         state: directory
       register: temp_image_dirs
       with_items: "{{ platforms }}"
       loop_control:
         label: "{{ item.image }}"
 
     - name: Expand Dockerfile templates
       ansible.builtin.template:
         src: Dockerfile.j2
         dest: "{{ temp_image_dirs.results[index].path }}/Dockerfile"
-        mode: 0600
+        mode: "0600"
       register: result
       with_items: "{{ platforms }}"
       loop_control:
         index_var: index
         label: "{{ item.image }}"
 
     - name: Build Dockerfile(s)
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/vagrant/driver.py` & `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
 from shutil import which
 
-from molecule import logger
-from molecule import util
+from molecule import logger, util
 from molecule.api import Driver
 
-
 LOG = logger.get_logger(__name__)
 
 
 class Vagrant(Driver):
     """
     The class responsible for managing `Vagrant`_ instances.  `Vagrant`_ is
     `not` the default driver used in Molecule.
@@ -121,18 +119,18 @@
 
         driver:
           name: vagrant
           safe_files:
             - foo
 
     .. _`Vagrant`: https://www.vagrantup.com
-    """  # noqa
+    """
 
-    def __init__(self, config=None):
-        super(Vagrant, self).__init__(config)
+    def __init__(self, config=None) -> None:
+        super().__init__(config)
         self._name = "vagrant"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -187,15 +185,15 @@
                 "ansible_port": d["port"],
                 "ansible_private_key_file": d["identity_file"],
                 "connection": "ssh",
                 "ansible_ssh_common_args": " ".join(self.ssh_connection_options),
             }
         except StopIteration:
             return {}
-        except IOError:
+        except OSError:
             # Instance has yet to be provisioned , therefore the
             # instance_config is not on disk.
             return {}
 
     @property
     def vagrantfile(self):
         return os.path.join(self._config.scenario.ephemeral_directory, "Vagrantfile")
@@ -209,21 +207,17 @@
 
     def sanity_checks(self):
         if not which("vagrant"):
             util.sysexit_with_message("vagrant executable was not found!")
 
         # TODO(ssbarnea): Replace code below with variant that check if ansible
         # has vagrant module available.
-        # try:
         #     import vagrant  # noqa
-        # except ImportError:
         #     util.sysexit_with_message(
-        #         "Unable to import python vagrant module. Running "
         #         "'pip instgt .all python-vagrant' should fix it."
-        #     )
 
     def template_dir(self):
         """Return path to its own cookiecutterm templates. It is used by init
         command in order to figure out where to load the templates from.
         """
         return os.path.join(os.path.dirname(__file__), "cookiecutter")
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/vagrant/modules/vagrant.py` & `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/vagrant.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 #  Copyright (c) 2015-2018 Cisco Systems, Inc.
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to
 #  deal in the Software without restriction, including without limitation the
 #  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
@@ -18,26 +17,22 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 
-from __future__ import absolute_import, division, print_function
-
-__metaclass__ = type
-
-from ansible.module_utils.basic import AnsibleModule
 import contextlib
 import datetime
-import io
 import os
 import subprocess
 import sys
 
+from ansible.module_utils.basic import AnsibleModule
+
 import molecule
 import molecule.util
 
 try:
     import vagrant
 except ImportError:
     sys.exit("ERROR: Driver missing, install python-vagrant.")
@@ -314,15 +309,15 @@
           {% endif %}
         {% endif %}
       {% endif %}
     end
   end
 {% endfor %}
 end
-""".strip()  # noqa
+""".strip()
 
 RETURN = r"""
 rc:
     description: The command return code (0 means success)
     returned: always
     type: int
 cmd:
@@ -336,24 +331,24 @@
 stderr:
     description: Output on stderr
     returned: changed
     type: str
 """
 
 
-class VagrantClient(object):
-    def __init__(self, module):
+class VagrantClient:
+    def __init__(self, module) -> None:
         self._module = module
         self.provision = self._module.params["provision"]
         self.cachier = self._module.params["cachier"]
 
         # compat
         if self._module.params["instance_name"] is not None:
             self._module.warn(
-                "Please convert your playbook to use the instances parameter. Compat layer will be removed later."
+                "Please convert your playbook to use the instances parameter. Compat layer will be removed later.",
             )
             self.instances = [
                 {
                     "name": self._module.params["instance_name"],
                     "interfaces": self._module.params["instance_interfaces"],
                     "instance_raw_config_args": self._module.params[
                         "instance_raw_config_args"
@@ -373,15 +368,15 @@
                     "provider_options": self._module.params["provider_options"],
                     "provider_override_args": self._module.params[
                         "provider_override_args"
                     ],
                     "provider_raw_config_args": self._module.params[
                         "provider_raw_config_args"
                     ],
-                }
+                },
             ]
         else:
             self.instances = self._module.params["instances"]
 
         self._config = self._get_config()
         self._vagrantfile = self._config["vagrantfile"]
         self._vagrant = self._get_vagrant()
@@ -390,40 +385,36 @@
         self._datetime = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.result = {}
 
     @contextlib.contextmanager
     def stdout_cm(self):
         """Redirect the stdout to a log file."""
         with open(self._get_stdout_log(), "a+") as fh:
-            msg = "### {} ###\n".format(self._datetime)
+            msg = f"### {self._datetime} ###\n"
             fh.write(msg)
             fh.flush()
 
             yield fh
 
     @contextlib.contextmanager
     def stderr_cm(self):
         """Redirect the stderr to a log file."""
         with open(self._get_stderr_log(), "a+") as fh:
-            msg = "### {} ###\n".format(self._datetime)
+            msg = f"### {self._datetime} ###\n"
             fh.write(msg)
             fh.flush()
 
             try:
                 yield fh
             except subprocess.CalledProcessError as e:
                 self._has_error = True
-                # msg = "CMD: {} returned {}\n{}".format(
-                #     e.cmd, e.returncode, e.output or ""
-                # )
                 self.result["cmd"] = e.cmd
                 self.result["rc"] = e.returncode
                 self.result["stderr"] = e.output or ""
 
-                # fh.write(msg)
                 # raise
             except Exception as e:
                 self._has_error = True
                 if hasattr(e, "message"):
                     fh.write(e.message)
                 else:
                     fh.write(e)
@@ -431,37 +422,37 @@
                 raise
 
     def up(self):
         changed = False
         if self._running() != len(self.instances):
             changed = True
             provision = self.provision
-            try:
+            with contextlib.suppress(Exception):
                 self._vagrant.up(provision=provision)
-            except Exception:
-                # NOTE(retr0h): Ignore the exception since python-vagrant
-                # passes the actual error as a no-argument ContextManager.
-                pass
 
         # NOTE(retr0h): Ansible wants only one module return `fail_json`
         # or `exit_json`.
         if not self._has_error:
             # compat
             if self._module.params["instance_name"] is not None:
                 self._module.exit_json(
-                    changed=changed, log=self._get_stdout_log(), **self._conf()[0]
+                    changed=changed,
+                    log=self._get_stdout_log(),
+                    **self._conf()[0],
                 )
             self._module.exit_json(
-                changed=changed, log=self._get_stdout_log(), results=self._conf()
+                changed=changed,
+                log=self._get_stdout_log(),
+                results=self._conf(),
             )
 
         msg = "Failed to start the VM(s): See log file '{}'".format(
-            self._get_stderr_log()
+            self._get_stderr_log(),
         )
-        with io.open(self._get_stderr_log(), "r", encoding="utf-8") as f:
+        with open(self._get_stderr_log(), encoding="utf-8") as f:
             self.result["stderr"] = f.read()
         self._module.fail_json(msg=msg, **self.result)
 
     def destroy(self):
         changed = False
         if self._created() > 0:
             changed = True
@@ -480,30 +471,32 @@
         self._module.exit_json(changed=changed)
 
     def _conf_instance(self, instance_name):
         try:
             return self._vagrant.conf(vm_name=instance_name)
         except Exception:
             msg = "Failed to get vagrant config for {}: See log file '{}'".format(
-                instance_name, self._get_stderr_log()
+                instance_name,
+                self._get_stderr_log(),
             )
-            with io.open(self._get_stderr_log(), "r", encoding="utf-8") as f:
+            with open(self._get_stderr_log(), encoding="utf-8") as f:
                 self.result["stderr"] = f.read()
                 self._module.fail_json(msg=msg, **self.result)
 
     def _status_instance(self, instance_name):
         try:
             s = self._vagrant.status(vm_name=instance_name)[0]
 
             return {"name": s.name, "state": s.state, "provider": s.provider}
         except Exception:
             msg = "Failed to get status for {}: See log file '{}'".format(
-                instance_name, self._get_stderr_log()
+                instance_name,
+                self._get_stderr_log(),
             )
-            with io.open(self._get_stderr_log(), "r", encoding="utf-8") as f:
+            with open(self._get_stderr_log(), encoding="utf-8") as f:
                 self.result["stderr"] = f.read()
                 self._module.fail_json(msg=msg, **self.result)
 
     def _conf(self):
         conf = []
 
         for i in self.instances:
@@ -526,33 +519,33 @@
         return vms_status
 
     def _created(self):
         status = self._status()
         if len(status) == 0:
             return 0
 
-        count = sum(map(lambda s: s["state"] == "not_created", status))
+        count = sum(s["state"] == "not_created" for s in status)
         return len(status) - count
 
     def _running(self):
         status = self._status()
         if len(status) == 0:
             return 0
 
-        count = sum(map(lambda s: s["state"] == "running", status))
+        count = sum(s["state"] == "running" for s in status)
         return count
 
     def _get_config(self):
-        conf = dict()
+        conf = {}
         conf["workdir"] = os.getenv("MOLECULE_EPHEMERAL_DIRECTORY")
         if self._module.params["workdir"] is not None:
             conf["workdir"] = self._module.params["workdir"]
         if conf["workdir"] is None:
             self._module.fail_json(
-                msg="Either workdir parameter or MOLECULE_EPHEMERAL_DIRECTORY env variable has to be set"
+                msg="Either workdir parameter or MOLECULE_EPHEMERAL_DIRECTORY env variable has to be set",
             )
         conf["vagrantfile"] = os.path.join(conf["workdir"], "Vagrantfile")
         return conf
 
     def _write_vagrantfile(self):
         instances = self._get_vagrant_config_dict()
         template = molecule.util.render_template(
@@ -565,15 +558,15 @@
 
     def _write_configs(self):
         self._write_vagrantfile()
         try:
             self._vagrant.validate(self._config["workdir"])
         except subprocess.CalledProcessError as e:
             self._module.fail_json(
-                msg=f"Failed to validate generated Vagrantfile: {e.stderr}"
+                msg=f"Failed to validate generated Vagrantfile: {e.stderr}",
             )
 
     def _get_vagrant(self):
         vagrant_env = os.environ.copy()
         if self._module.params["parallel"] is False:
             vagrant_env["VAGRANT_NO_PARALLEL"] = "1"
         v = vagrant.Vagrant(
@@ -582,37 +575,36 @@
             root=self._config["workdir"],
             env=vagrant_env,
         )
 
         return v
 
     def _get_instance_vagrant_config_dict(self, instance):
-
         checksum = instance.get("box_download_checksum")
         checksum_type = instance.get("box_download_checksum_type")
         if bool(checksum) ^ bool(checksum_type):
             self._module.fail_json(
-                msg="box_download_checksum and box_download_checksum_type must be used together"
+                msg="box_download_checksum and box_download_checksum_type must be used together",
             )
 
         networks = []
         if "interfaces" in instance:
             for iface in instance["interfaces"]:
-                net = dict()
+                net = {}
                 net["name"] = iface["network_name"]
                 iface.pop("network_name")
                 net["options"] = iface
                 networks.append(net)
 
         # compat
         provision = instance.get("provision")
         if provision is not None:
             self.provision = self.provision or provision
             self._module.warn(
-                "Please convert your molecule.yml to move provision parameter to driver:. Compat layer will be removed later."
+                "Please convert your molecule.yml to move provision parameter to driver:. Compat layer will be removed later.",
             )
         d = {
             "name": instance.get("name"),
             "hostname": instance.get("hostname", instance.get("name")),
             "memory": instance.get("memory", 512),
             "cpus": instance.get("cpus", 2),
             "networks": networks,
@@ -633,27 +625,29 @@
             "provider_options": {},
             "provider_raw_config_args": instance.get("provider_raw_config_args", None),
             "provider_override_args": instance.get("provider_override_args", None),
         }
 
         d["config_options"].update(
             molecule.util.merge_dicts(
-                d["config_options"], instance.get("config_options", {})
-            )
+                d["config_options"],
+                instance.get("config_options", {}),
+            ),
         )
         if "cachier" in d["config_options"]:
             self.cachier = d["config_options"]["cachier"]
             self._module.warn(
-                "Please convert your molecule.yml to move cachier parameter to driver:. Compat layer will be removed later."
+                "Please convert your molecule.yml to move cachier parameter to driver:. Compat layer will be removed later.",
             )
 
         d["provider_options"].update(
             molecule.util.merge_dicts(
-                d["provider_options"], instance.get("provider_options", {})
-            )
+                d["provider_options"],
+                instance.get("provider_options", {}),
+            ),
         )
 
         return d
 
     def _get_vagrant_config_dict(self):
         config_list = []
         for instance in self.instances:
@@ -663,54 +657,58 @@
     def _get_stdout_log(self):
         return self._get_vagrant_log("out")
 
     def _get_stderr_log(self):
         return self._get_vagrant_log("err")
 
     def _get_vagrant_log(self, __type):
-        return os.path.join(self._config["workdir"], "vagrant.{}".format(__type))
+        return os.path.join(self._config["workdir"], f"vagrant.{__type}")
 
 
 def main():
     module = AnsibleModule(
-        argument_spec=dict(
-            instances=dict(type="list", required=False),
-            instance_name=dict(type="str", required=False, default=None),
-            instance_interfaces=dict(type="list", default=[]),
-            instance_raw_config_args=dict(type="list", default=None),
-            config_options=dict(type="dict", default={}),
-            platform_box=dict(type="str", required=False),
-            platform_box_version=dict(type="str"),
-            platform_box_url=dict(type="str"),
-            platform_box_download_checksum=dict(type="str"),
-            platform_box_download_checksum_type=dict(type="str"),
-            provider_memory=dict(type="int", default=512),
-            provider_cpus=dict(type="int", default=2),
-            provider_options=dict(type="dict", default={}),
-            provider_override_args=dict(type="list", default=None),
-            provider_raw_config_args=dict(type="list", default=None),
-            provider_name=dict(type="str", default="virtualbox"),
-            default_box=dict(type="str", default=None),
-            provision=dict(type="bool", default=False),
-            force_stop=dict(type="bool", default=False),
-            cachier=dict(type="str", default="machine"),
-            state=dict(type="str", default="up", choices=["up", "destroy", "halt"]),
-            workdir=dict(type="str"),
-            parallel=dict(type="bool", default=True),
-        ),
+        argument_spec={
+            "instances": {"type": "list", "required": False},
+            "instance_name": {"type": "str", "required": False, "default": None},
+            "instance_interfaces": {"type": "list", "default": []},
+            "instance_raw_config_args": {"type": "list", "default": None},
+            "config_options": {"type": "dict", "default": {}},
+            "platform_box": {"type": "str", "required": False},
+            "platform_box_version": {"type": "str"},
+            "platform_box_url": {"type": "str"},
+            "platform_box_download_checksum": {"type": "str"},
+            "platform_box_download_checksum_type": {"type": "str"},
+            "provider_memory": {"type": "int", "default": 512},
+            "provider_cpus": {"type": "int", "default": 2},
+            "provider_options": {"type": "dict", "default": {}},
+            "provider_override_args": {"type": "list", "default": None},
+            "provider_raw_config_args": {"type": "list", "default": None},
+            "provider_name": {"type": "str", "default": "virtualbox"},
+            "default_box": {"type": "str", "default": None},
+            "provision": {"type": "bool", "default": False},
+            "force_stop": {"type": "bool", "default": False},
+            "cachier": {"type": "str", "default": "machine"},
+            "state": {
+                "type": "str",
+                "default": "up",
+                "choices": ["up", "destroy", "halt"],
+            },
+            "workdir": {"type": "str"},
+            "parallel": {"type": "bool", "default": True},
+        },
         required_together=[
             ("platform_box_download_checksum", "platform_box_download_checksum_type"),
             ("instances", "default_box"),
         ],
         supports_check_mode=False,
     )
 
     if not (bool(module.params["instances"]) ^ bool(module.params["instance_name"])):
         module.fail_json(
-            msg="Either instances or instance_name parameters should be used and not at the same time"
+            msg="Either instances or instance_name parameters should be used and not at the same time",
         )
 
     v = VagrantClient(module)
 
     if module.params["state"] == "up":
         v.up()
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/create.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/create.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 - name: Create
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   tasks:
-    - name: Create molecule instance(s)  # noqa fqcn[action]
+    - name: Create molecule instance(s) # noqa fqcn[action]
       vagrant:
         instances: "{{ molecule_yml.platforms }}"
         default_box: "{{ molecule_yml.driver.default_box | default('generic/alpine316') }}"
         provider_name: "{{ molecule_yml.driver.provider.name | default(omit, true) }}"
         provision: "{{ molecule_yml.driver.provision | default(omit) }}"
         cachier: "{{ molecule_yml.driver.cachier | default(omit) }}"
         parallel: "{{ molecule_yml.driver.parallel | default(omit) }}"
@@ -19,30 +19,31 @@
 
     # NOTE(retr0h): Vagrant/VirtualBox sucks and parallelizing instance creation
     # causes issues.
 
     # Mandatory configuration for Molecule to function.
 
     - name: Create molecule instances configuration
-      when: server is changed  # noqa no-handler
+      when: server is changed # noqa no-handler
       block:
-
         - name: Populate instance config dict
           ansible.builtin.set_fact:
-            instance_conf_dict: {
-              'instance': "{{ item.Host }}",
-              'address': "{{ item.HostName }}",
-              'user': "{{ item.User }}",
-              'port': "{{ item.Port }}",
-              'identity_file': "{{ item.IdentityFile }}", }
+            instance_conf_dict:
+              {
+                "instance": "{{ item.Host }}",
+                "address": "{{ item.HostName }}",
+                "user": "{{ item.User }}",
+                "port": "{{ item.Port }}",
+                "identity_file": "{{ item.IdentityFile }}",
+              }
           with_items: "{{ server.results }}"
           register: instance_config_dict
 
         - name: Convert instance config dict to a list
           ansible.builtin.set_fact:
             instance_conf: "{{ instance_config_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
         - name: Dump instance config
           ansible.builtin.copy:
             content: "{{ instance_conf | to_json | from_json | to_yaml }}"
             dest: "{{ molecule_instance_config }}"
-            mode: 0600
+            mode: "0600"
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/destroy.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/destroy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 - name: Destroy
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   tasks:
-    - name: Destroy molecule instance(s)  # noqa fqcn[action]
+    - name: Destroy molecule instance(s) # noqa fqcn[action]
       vagrant:
         instances: "{{ molecule_yml.platforms }}"
         default_box: "{{ molecule_yml.driver.default_box | default('generic/alpine316') }}"
         provider_name: "{{ molecule_yml.driver.provider.name | default(omit, true) }}"
         cachier: "{{ molecule_yml.driver.cachier | default(omit) }}"
         force_stop: "{{ item.force_stop | default(true) }}"
         state: destroy
@@ -21,15 +21,15 @@
 
     # Mandatory configuration for Molecule to function.
 
     - name: Populate instance config
       ansible.builtin.set_fact:
         instance_conf: {}
 
-    - name: Dump instance config  # noqa no-handler
+    - name: Dump instance config # noqa no-handler
       ansible.builtin.copy:
         content: |
           # Molecule managed
           {{ instance_conf | to_json | from_json | to_yaml }}
         dest: "{{ molecule_instance_config }}"
-        mode: 0600
+        mode: "0600"
       when: server.changed | bool
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins/vagrant/playbooks/prepare.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/prepare.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 ---
 - name: Prepare
   hosts: all
   gather_facts: false
   tasks:
+    - name: Gather system info
+      ansible.builtin.raw: uname
+      register: raw_uname
+      changed_when: false
+      failed_when: false
+
     - name: Bootstrap python for Ansible
       ansible.builtin.raw: |
         command -v python3 python || (
         command -v apk >/dev/null && sudo apk add --no-progress --update python3 ||
         (test -e /usr/bin/dnf && sudo dnf install -y python3) ||
         (test -e /usr/bin/apt && (apt -y update && apt install -y python3-minimal)) ||
         (test -e /usr/bin/yum && sudo yum -y -qq install python3) ||
         (test -e /usr/sbin/pkg && sudo env ASSUME_ALWAYS_YES=yes pkg update && sudo env ASSUME_ALWAYS_YES=yes pkg install python3) ||
         (test -e /usr/sbin/pkg_add && sudo /usr/sbin/pkg_add -U -I -x python%3.9) ||
+        (test -e /usr/bin/pacman && sudo /usr/bin/pacman -Sy python3 --noconfirm --quiet) ||
         echo "Warning: Python not bootstrapped due to unknown platform."
         )
       become: true
       changed_when: false
+      when: raw_uname.rc == 0 and raw_uname.stdout | trim == "Linux"
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins.egg-info/PKG-INFO` & `molecule-plugins-23.4.0/src/molecule_plugins.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugins
-Version: 23.0.0
+Version: 23.4.0
 Summary: Molecule Plugins
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 Maintainer-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule-plugins
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule-plugins
@@ -15,41 +15,46 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: azure
 Provides-Extra: docker
 Provides-Extra: ec2
 Provides-Extra: gce
 Provides-Extra: podman
+Provides-Extra: selinux
 License-File: LICENSE
 
 # molecule-plugins
 
 This repository contains the following molecule plugins:
 
 - azure
+- containers
 - docker
+- ec2
 - gce
+- podman
+- vagrant
+
 
 Installing `molecule-plugins` does not install dependencies specific to each,
 plugin. To install these you need to install the extras for each plugin, like
 `pip3 install 'molecule-plugins[azure]'`.
 
 Before installing these plugins be sure that you uninstall their old standalone
 packages, like `pip3 uninstall molecule-azure`. If you fail to do so, you will
```

### Comparing `molecule-plugins-23.0.0/src/molecule_plugins.egg-info/SOURCES.txt` & `molecule-plugins-23.4.0/src/molecule_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/azure/functional/conftest.py` & `molecule-plugins-23.4.0/test/azure/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/azure/functional/test_azure.py` & `molecule-plugins-23.4.0/test/azure/functional/test_azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
 import os
 
+import pytest
+
 from molecule import logger
-from molecule.util import run_command
 from molecule.test.conftest import change_dir_to
-
-# import change_dir_to, temp_dir
+from molecule.util import run_command
 
 LOG = logger.get_logger(__name__)
 
 
 def test_command_init_scenario(temp_dir):
     role_directory = os.path.join(temp_dir.strpath, "test_init")
     cmd = ["molecule", "init", "role", "foo.test_init"]
```

### Comparing `molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py` & `molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 import testinfra.utils.ansible_runner
 
 testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-    os.environ["MOLECULE_INVENTORY_FILE"]
+    os.environ["MOLECULE_INVENTORY_FILE"],
 ).get_hosts("all")
 
 
 def test_hostname(host):
-    assert "instance" == host.check_output("hostname -s")
+    assert host.check_output("hostname -s") == "instance"
 
 
 def test_etc_molecule_directory(host):
     f = host.file("/etc/molecule")
 
     assert f.is_directory
     assert f.user == "root"
```

### Comparing `molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml` & `molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py` & `molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 
 import testinfra.utils.ansible_runner
 
 testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-    os.environ["MOLECULE_INVENTORY_FILE"]
+    os.environ["MOLECULE_INVENTORY_FILE"],
 ).get_hosts("all")
 
 
 def test_hostname(host):
     assert re.search(r"instance-[12].*", host.check_output("hostname -s"))
```

### Comparing `molecule-plugins-23.0.0/test/containers/functional/conftest.py` & `molecule-plugins-23.4.0/test/containers/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/containers/functional/test_containers.py` & `molecule-plugins-23.4.0/test/containers/functional/test_containers.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/docker/test_func.py` & `molecule-plugins-23.4.0/test/docker/test_func.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functional tests."""
 import os
 import pathlib
 import shutil
 import subprocess
+
 import pytest
 
 from molecule import logger
 from molecule.test.conftest import change_dir_to
 from molecule.util import run_command
 
 LOG = logger.get_logger(__name__)
@@ -26,15 +27,14 @@
     """Verify that init scenario works."""
     shutil.rmtree(tmp_path, ignore_errors=True)
     tmp_path.mkdir(exist_ok=True)
 
     scenario_name = "default"
 
     with change_dir_to(tmp_path):
-
         scenario_directory = tmp_path / "molecule" / scenario_name
         cmd = [
             "molecule",
             "init",
             "scenario",
             "--driver-name",
             DRIVER,
```

### Comparing `molecule-plugins-23.0.0/test/ec2/functional/conftest.py` & `molecule-plugins-23.4.0/test/ec2/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/ec2/functional/test_ec2.py` & `molecule-plugins-23.4.0/test/ec2/functional/test_ec2.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
 import os
 
+import pytest
+
 from molecule import logger
-from molecule.util import run_command
 from molecule.test.conftest import change_dir_to
 from molecule.test.functional.conftest import metadata_lint_update
-
-# import change_dir_to, temp_dir
+from molecule.util import run_command
 
 LOG = logger.get_logger(__name__)
 
 
 @pytest.mark.xfail(reason="need to fix template path")
 def test_command_init_scenario(temp_dir):
     role_directory = os.path.join(temp_dir.strpath, "test-init")
```

### Comparing `molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py` & `molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import testinfra.utils.ansible_runner
 
 testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-    os.environ["MOLECULE_INVENTORY_FILE"]
+    os.environ["MOLECULE_INVENTORY_FILE"],
 ).get_hosts("all")
 
 
 # EC2 provides unique random hostnames.
 def test_hostname(host):
     pass
```

### Comparing `molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml` & `molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py` & `molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import testinfra.utils.ansible_runner
 
 testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-    os.environ["MOLECULE_INVENTORY_FILE"]
+    os.environ["MOLECULE_INVENTORY_FILE"],
 ).get_hosts("all")
 
 
 # EC2 provides unique random hostnames.
 def test_hostname(host):
     pass
```

### Comparing `molecule-plugins-23.0.0/test/gce/functional/conftest.py` & `molecule-plugins-23.4.0/test/gce/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/gce/functional/test_func.py` & `molecule-plugins-23.4.0/test/gce/functional/test_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
 import os
 
+import pytest
+
 from molecule import logger
-from molecule.util import run_command
 from molecule.test.conftest import change_dir_to
 from molecule.test.functional.conftest import metadata_lint_update
+from molecule.util import run_command
 
 LOG = logger.get_logger(__name__)
 driver_name = __name__.split(".")[0].split("_")[-1]
 
 
 @pytest.mark.xfail(reason="need to fix template path")
 def test_command_init_scenario(temp_dir):
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/INSTALL.md` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/INSTALL.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/create.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
     - name: Make sure if linux or windows either specified
       assert:
         that:
           - molecule_yml.driver.instance_os_type | lower == "linux" or
             molecule_yml.driver.instance_os_type | lower == "windows"
         fail_msg: "instance_os_type is possible only to specify linux or windows either"
 
-    - name: get network info
+    - name: Get network info
       google.cloud.gcp_compute_network_info:
         filters:
           - name = "{{ molecule_yml.driver.network_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
         service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
         service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_network
 
-    - name: get subnetwork info
+    - name: Get subnetwork info
       google.cloud.gcp_compute_subnetwork_info:
         filters:
           - name = "{{ molecule_yml.driver.subnetwork_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
         region: "{{ molecule_yml.driver.region }}"
         service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
         service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_subnetwork
 
-    - name: set external access config
+    - name: Set external access config
       set_fact:
         external_access_config:
           - access_configs:
               - name: "External NAT"
                 type: "ONE_TO_NAT"
       when: molecule_yml.driver.external_access
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/destroy.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/files/windows_auth.py` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/files/windows_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import argparse
 import base64
 import copy
 import datetime
 import json
 import time
-import argparse
 
 # PyCrypto library: https://pypi.python.org/pypi/pycrypto
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.PublicKey import RSA
 from Crypto.Util.number import long_to_bytes
+from googleapiclient.discovery import build
 
 # Google API Client Library for Python:
 # https://developers.google.com/api-client-library/python/start/get_started
 from oauth2client.client import GoogleCredentials
-from googleapiclient.discovery import build
 
 
 def GetCompute():
     """Get a compute object for communicating with the Compute Engine API."""
     credentials = GoogleCredentials.get_application_default()
     compute = build("compute", "v1", credentials=credentials)
     return compute
@@ -72,15 +72,14 @@
     # between the time on the client and the time on the server.
     expire_time = utc_now + datetime.timedelta(minutes=5)
     return expire_time.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
 def GetJsonString(user, modulus, exponent, email):
     """Return the JSON string object that represents the windows-keys entry."""
-
     converted_modulus = modulus.decode("utf-8")
     converted_exponent = exponent.decode("utf-8")
 
     expire = GetExpirationTimeString()
     data = {
         "userName": user,
         "modulus": converted_modulus,
@@ -101,25 +100,31 @@
     new_metadata["items"] = [{"key": "windows-keys", "value": metadata_entry}]
     return new_metadata
 
 
 def UpdateInstanceMetadata(compute, instance, zone, project, new_metadata):
     """Update the instance metadata."""
     cmd = compute.instances().setMetadata(
-        instance=instance, project=project, zone=zone, body=new_metadata
+        instance=instance,
+        project=project,
+        zone=zone,
+        body=new_metadata,
     )
     return cmd.execute()
 
 
 def GetSerialPortFourOutput(compute, instance, zone, project):
     """Get the output from serial port 4 from the instance."""
     # Encrypted passwords are printed to COM4 on the windows server:
     port = 4
     cmd = compute.instances().getSerialPortOutput(
-        instance=instance, project=project, zone=zone, port=port
+        instance=instance,
+        project=project,
+        zone=zone,
+        port=port,
     )
     output = cmd.execute()
     return output["contents"]
 
 
 def GetEncryptedPasswordFromSerialPort(serial_port_output, modulus):
     """Find and return the correct encrypted password, based on the modulus."""
@@ -132,68 +137,79 @@
     for line in reversed(output):
         try:
             entry = json.loads(line)
             if converted_modulus == entry["modulus"]:
                 return entry["encryptedPassword"]
         except ValueError:
             pass
+    return None
 
 
 def DecryptPassword(encrypted_password, key):
     """Decrypt a base64 encoded encrypted password using the provided key."""
-
     decoded_password = base64.b64decode(encrypted_password)
     cipher = PKCS1_OAEP.new(key)
     password = cipher.decrypt(decoded_password)
     return password
 
 
 def Arguments():
     # Create the parser
     args = argparse.ArgumentParser(description="List the content of a folder")
 
     # Add the arguments
     args.add_argument(
-        "--instance", metavar="instance", type=str, help="compute instance name"
+        "--instance",
+        metavar="instance",
+        type=str,
+        help="compute instance name",
     )
 
     args.add_argument("--zone", metavar="zone", type=str, help="compute zone")
 
     args.add_argument("--project", metavar="project", type=str, help="gcp project")
 
     args.add_argument("--username", metavar="username", type=str, help="username")
 
     args.add_argument("--email", metavar="email", type=str, help="email")
 
-    # return arguments
     return args.parse_args()
 
 
 def main():
     config_args = Arguments()
 
     # Setup
     compute = GetCompute()
     key = GetKey()
     modulus, exponent = GetModulusExponentInBase64(key)
 
     # Get existing metadata
     instance_ref = GetInstance(
-        compute, config_args.instance, config_args.zone, config_args.project
+        compute,
+        config_args.instance,
+        config_args.zone,
+        config_args.project,
     )
     old_metadata = instance_ref["metadata"]
     # Create and set new metadata
     metadata_entry = GetJsonString(
-        config_args.username, modulus, exponent, config_args.email
+        config_args.username,
+        modulus,
+        exponent,
+        config_args.email,
     )
     new_metadata = UpdateWindowsKeys(old_metadata, metadata_entry)
 
     # Get Serial output BEFORE the modification
     serial_port_output = GetSerialPortFourOutput(
-        compute, config_args.instance, config_args.zone, config_args.project
+        compute,
+        config_args.instance,
+        config_args.zone,
+        config_args.project,
     )
 
     UpdateInstanceMetadata(
         compute,
         config_args.instance,
         config_args.zone,
         config_args.project,
@@ -202,23 +218,26 @@
 
     # Get and decrypt password from serial port output
     # Monitor changes from output to get the encrypted password as soon as it's generated, will wait for 30 seconds
     i = 0
     new_serial_port_output = serial_port_output
     while i <= 30 and serial_port_output == new_serial_port_output:
         new_serial_port_output = GetSerialPortFourOutput(
-            compute, config_args.instance, config_args.zone, config_args.project
+            compute,
+            config_args.instance,
+            config_args.zone,
+            config_args.project,
         )
         i += 1
         time.sleep(1)
 
     enc_password = GetEncryptedPasswordFromSerialPort(new_serial_port_output, modulus)
 
     password = DecryptPassword(enc_password, key)
     converted_password = password.decode("utf-8")
 
     # Display only the password
-    print(format(converted_password))
+    print(format(converted_password))  # noqa: T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/handlers/main.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/handlers/main.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 ---
 - name: Populate instance config dict Linux
   set_fact:
-    instance_conf_dict: {
-      'instance': "{{ instance_info.name }}",
-      'address': "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-      'user': "{{ lookup('env','USER') }}",
-      'port': "22",
-      'identity_file': "{{ ssh_identity_file }}",
-      'instance_os_type': "{{ molecule_yml.driver.instance_os_type }}"
-    }
+    instance_conf_dict:
+      {
+        "instance": "{{ instance_info.name }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "{{ lookup('env','USER') }}",
+        "port": "22",
+        "identity_file": "{{ ssh_identity_file }}",
+        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
+      }
   loop: "{{ server.results }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Populate instance config dict Windows
   set_fact:
-    instance_conf_dict: {
-      'instance': "{{ instance_info.name }}",
-      'address': "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-      'user': "molecule_usr",
-      'password': "{{ instance_info.password }}",
-      'port': "{{ instance_info.winrm_port | default(5986) }}",
-      'winrm_transport': "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
-      'winrm_server_cert_validation': "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
-      'instance_os_type': "{{ molecule_yml.driver.instance_os_type }}"
-    }
+    instance_conf_dict:
+      {
+        "instance": "{{ instance_info.name }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "molecule_usr",
+        "password": "{{ instance_info.password }}",
+        "port": "{{ instance_info.winrm_port | default(5986) }}",
+        "winrm_transport": "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
+        "winrm_server_cert_validation": "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
+        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
+      }
   loop: "{{ win_instances }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
-
 - name: Wipe out instance config
   set_fact:
     instance_conf: {}
 
 - name: Convert instance config dict to a list
   set_fact:
     instance_conf: "{{ instance_conf_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
 - name: Dump instance config
   copy:
     content: "{{ instance_conf }}"
     dest: "{{ molecule_instance_config }}"
-    mode: '0600'
+    mode: "0600"
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/molecule.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/molecule.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 dependency:
   name: galaxy
 driver:
   name: gce
-  project_id: change-to-id-of-the-gcp-project  # if not set, will default to env GCE_PROJECT_ID
-  auth_kind: null  # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
-  service_account_email: null  # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
-  service_account_file: null  # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
-  region: us-west1  # REQUIRED. example: us-central1
-  external_access: false  # chose whether to create a public IP for the VM or not - default is private IP only
-  instance_os_type: linux  # will be considered linux by default, but can be explicitely set to windows
+  project_id: change-to-id-of-the-gcp-project # if not set, will default to env GCE_PROJECT_ID
+  auth_kind: null # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
+  service_account_email: null # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
+  service_account_file: null # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
+  region: us-west1 # REQUIRED. example: us-central1
+  external_access: false # chose whether to create a public IP for the VM or not - default is private IP only
+  instance_os_type: windows # will be considered linux by default, but can be explicitely set to windows
 platforms:
-  - name: linuxgce-createdbymolecule  # is an instance name
-    machine_type: n1-standard-1  # define your machine type
-    zone: null  # example: us-west1-b, will default to zone b of driver.region
+  - name: linuxgce-createdbymolecule # is an instance name
+    machine_type: n1-standard-1 # define your machine type
+    zone: null # example: us-west1-b, will default to zone b of driver.region
 provisioner:
   name: ansible
 verifier:
   name: ansible
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-- name: create ssh keypair
-  openssh_keypair:
+- name: Create ssh keypair
+  community.crypto.openssh_keypair:
     comment: "{{ lookup('env','USER') }} user for Molecule"
     path: "{{ ssh_identity_file }}"
   register: keypair
 
-- name: create molecule Linux instance(s)
+- name: Create molecule Linux instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     metadata:
       ssh-keys: "{{ lookup('env','USER') }}:{{ keypair.public_key }}}"
     disks:
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-- name: create molecule Windows instance(s)
+- name: Create molecule Windows instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     disks:
       - auto_delete: true
         boot: true
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/INSTALL.md` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/INSTALL.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/create.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
     - name: Make sure if linux or windows either specified
       assert:
         that:
           - molecule_yml.driver.instance_os_type | lower == "linux" or
             molecule_yml.driver.instance_os_type | lower == "windows"
         fail_msg: "instance_os_type is possible only to specify linux or windows either"
 
-    - name: get network info
+    - name: Get network info
       google.cloud.gcp_compute_network_info:
         filters:
           - name = "{{ molecule_yml.driver.network_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
         service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
         service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_network
 
-    - name: get subnetwork info
+    - name: Get subnetwork info
       google.cloud.gcp_compute_subnetwork_info:
         filters:
           - name = "{{ molecule_yml.driver.subnetwork_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
         region: "{{ molecule_yml.driver.region }}"
         service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
         service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_subnetwork
 
-    - name: set external access config
+    - name: Set external access config
       set_fact:
         external_access_config:
           - access_configs:
               - name: "External NAT"
                 type: "ONE_TO_NAT"
       when: molecule_yml.driver.external_access
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/destroy.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/files/windows_auth.py` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/files/windows_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import argparse
 import base64
 import copy
 import datetime
 import json
 import time
-import argparse
 
 # PyCrypto library: https://pypi.python.org/pypi/pycrypto
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.PublicKey import RSA
 from Crypto.Util.number import long_to_bytes
+from googleapiclient.discovery import build
 
 # Google API Client Library for Python:
 # https://developers.google.com/api-client-library/python/start/get_started
 from oauth2client.client import GoogleCredentials
-from googleapiclient.discovery import build
 
 
 def GetCompute():
     """Get a compute object for communicating with the Compute Engine API."""
     credentials = GoogleCredentials.get_application_default()
     compute = build("compute", "v1", credentials=credentials)
     return compute
@@ -72,15 +72,14 @@
     # between the time on the client and the time on the server.
     expire_time = utc_now + datetime.timedelta(minutes=5)
     return expire_time.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
 def GetJsonString(user, modulus, exponent, email):
     """Return the JSON string object that represents the windows-keys entry."""
-
     converted_modulus = modulus.decode("utf-8")
     converted_exponent = exponent.decode("utf-8")
 
     expire = GetExpirationTimeString()
     data = {
         "userName": user,
         "modulus": converted_modulus,
@@ -101,25 +100,31 @@
     new_metadata["items"] = [{"key": "windows-keys", "value": metadata_entry}]
     return new_metadata
 
 
 def UpdateInstanceMetadata(compute, instance, zone, project, new_metadata):
     """Update the instance metadata."""
     cmd = compute.instances().setMetadata(
-        instance=instance, project=project, zone=zone, body=new_metadata
+        instance=instance,
+        project=project,
+        zone=zone,
+        body=new_metadata,
     )
     return cmd.execute()
 
 
 def GetSerialPortFourOutput(compute, instance, zone, project):
     """Get the output from serial port 4 from the instance."""
     # Encrypted passwords are printed to COM4 on the windows server:
     port = 4
     cmd = compute.instances().getSerialPortOutput(
-        instance=instance, project=project, zone=zone, port=port
+        instance=instance,
+        project=project,
+        zone=zone,
+        port=port,
     )
     output = cmd.execute()
     return output["contents"]
 
 
 def GetEncryptedPasswordFromSerialPort(serial_port_output, modulus):
     """Find and return the correct encrypted password, based on the modulus."""
@@ -132,68 +137,79 @@
     for line in reversed(output):
         try:
             entry = json.loads(line)
             if converted_modulus == entry["modulus"]:
                 return entry["encryptedPassword"]
         except ValueError:
             pass
+    return None
 
 
 def DecryptPassword(encrypted_password, key):
     """Decrypt a base64 encoded encrypted password using the provided key."""
-
     decoded_password = base64.b64decode(encrypted_password)
     cipher = PKCS1_OAEP.new(key)
     password = cipher.decrypt(decoded_password)
     return password
 
 
 def Arguments():
     # Create the parser
     args = argparse.ArgumentParser(description="List the content of a folder")
 
     # Add the arguments
     args.add_argument(
-        "--instance", metavar="instance", type=str, help="compute instance name"
+        "--instance",
+        metavar="instance",
+        type=str,
+        help="compute instance name",
     )
 
     args.add_argument("--zone", metavar="zone", type=str, help="compute zone")
 
     args.add_argument("--project", metavar="project", type=str, help="gcp project")
 
     args.add_argument("--username", metavar="username", type=str, help="username")
 
     args.add_argument("--email", metavar="email", type=str, help="email")
 
-    # return arguments
     return args.parse_args()
 
 
 def main():
     config_args = Arguments()
 
     # Setup
     compute = GetCompute()
     key = GetKey()
     modulus, exponent = GetModulusExponentInBase64(key)
 
     # Get existing metadata
     instance_ref = GetInstance(
-        compute, config_args.instance, config_args.zone, config_args.project
+        compute,
+        config_args.instance,
+        config_args.zone,
+        config_args.project,
     )
     old_metadata = instance_ref["metadata"]
     # Create and set new metadata
     metadata_entry = GetJsonString(
-        config_args.username, modulus, exponent, config_args.email
+        config_args.username,
+        modulus,
+        exponent,
+        config_args.email,
     )
     new_metadata = UpdateWindowsKeys(old_metadata, metadata_entry)
 
     # Get Serial output BEFORE the modification
     serial_port_output = GetSerialPortFourOutput(
-        compute, config_args.instance, config_args.zone, config_args.project
+        compute,
+        config_args.instance,
+        config_args.zone,
+        config_args.project,
     )
 
     UpdateInstanceMetadata(
         compute,
         config_args.instance,
         config_args.zone,
         config_args.project,
@@ -202,23 +218,26 @@
 
     # Get and decrypt password from serial port output
     # Monitor changes from output to get the encrypted password as soon as it's generated, will wait for 30 seconds
     i = 0
     new_serial_port_output = serial_port_output
     while i <= 30 and serial_port_output == new_serial_port_output:
         new_serial_port_output = GetSerialPortFourOutput(
-            compute, config_args.instance, config_args.zone, config_args.project
+            compute,
+            config_args.instance,
+            config_args.zone,
+            config_args.project,
         )
         i += 1
         time.sleep(1)
 
     enc_password = GetEncryptedPasswordFromSerialPort(new_serial_port_output, modulus)
 
     password = DecryptPassword(enc_password, key)
     converted_password = password.decode("utf-8")
 
     # Display only the password
-    print(format(converted_password))
+    print(format(converted_password))  # noqa: T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/handlers/main.yml` & `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/handlers/main.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 ---
 - name: Populate instance config dict Linux
-  set_fact:
-    instance_conf_dict: {
-      'instance': "{{ instance_info.name }}",
-      'address': "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-      'user': "{{ lookup('env','USER') }}",
-      'port': "22",
-      'identity_file': "{{ ssh_identity_file }}",
-      'instance_os_type': "{{ molecule_yml.driver.instance_os_type }}"
-    }
+  ansible.builtin.set_fact:
+    instance_conf_dict:
+      {
+        "instance": "{{ instance_info.name }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "{{ lookup('env','USER') }}",
+        "port": "22",
+        "identity_file": "{{ ssh_identity_file }}",
+        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
+      }
   loop: "{{ server.results }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Populate instance config dict Windows
-  set_fact:
-    instance_conf_dict: {
-      'instance': "{{ instance_info.name }}",
-      'address': "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-      'user': "molecule_usr",
-      'password': "{{ instance_info.password }}",
-      'port': "{{ instance_info.winrm_port | default(5986) }}",
-      'winrm_transport': "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
-      'winrm_server_cert_validation': "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
-      'instance_os_type': "{{ molecule_yml.driver.instance_os_type }}"
-    }
+  ansible.builtin.set_fact:
+    instance_conf_dict:
+      {
+        "instance": "{{ instance_info.name }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "molecule_usr",
+        "password": "{{ instance_info.password }}",
+        "port": "{{ instance_info.winrm_port | default(5986) }}",
+        "winrm_transport": "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
+        "winrm_server_cert_validation": "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
+        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
+      }
   loop: "{{ win_instances }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
-
 - name: Wipe out instance config
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf: {}
 
 - name: Convert instance config dict to a list
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf: "{{ instance_conf_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
 - name: Dump instance config
-  copy:
+  ansible.builtin.copy:
     content: "{{ instance_conf }}"
     dest: "{{ molecule_instance_config }}"
-    mode: '0600'
+    mode: "0600"
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/molecule.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/linux/molecule.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 dependency:
   name: galaxy
 driver:
   name: gce
-  project_id: change-to-id-of-the-gcp-project  # if not set, will default to env GCE_PROJECT_ID
-  auth_kind: null  # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
-  service_account_email: null  # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
-  service_account_file: null  # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
-  region: us-west1  # REQUIRED. example: us-central1
-  external_access: false  # chose whether to create a public IP for the VM or not - default is private IP only
-  instance_os_type: windows  # will be considered linux by default, but can be explicitely set to windows
+  project_id: change-to-id-of-the-gcp-project # if not set, will default to env GCE_PROJECT_ID
+  auth_kind: null # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
+  service_account_email: null # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
+  service_account_file: null # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
+  region: us-west1 # REQUIRED. example: us-central1
+  external_access: false # chose whether to create a public IP for the VM or not - default is private IP only
+  instance_os_type: linux # will be considered linux by default, but can be explicitely set to windows
 platforms:
-  - name: linuxgce-createdbymolecule  # is an instance name
-    machine_type: n1-standard-1  # define your machine type
-    zone: null  # example: us-west1-b, will default to zone b of driver.region
+  - name: linuxgce-createdbymolecule # is an instance name
+    machine_type: n1-standard-1 # define your machine type
+    zone: null # example: us-west1-b, will default to zone b of driver.region
 provisioner:
   name: ansible
 verifier:
   name: ansible
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-- name: create ssh keypair
-  openssh_keypair:
+- name: Create ssh keypair
+  community.crypto.openssh_keypair:
     comment: "{{ lookup('env','USER') }} user for Molecule"
     path: "{{ ssh_identity_file }}"
   register: keypair
 
-- name: create molecule Linux instance(s)
+- name: Create molecule Linux instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     metadata:
       ssh-keys: "{{ lookup('env','USER') }}:{{ keypair.public_key }}}"
     disks:
```

### Comparing `molecule-plugins-23.0.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml` & `molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-- name: create molecule Windows instance(s)
+- name: Create molecule Windows instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     disks:
       - auto_delete: true
         boot: true
```

### Comparing `molecule-plugins-23.0.0/test/podman/test_func.py` & `molecule-plugins-23.4.0/test/podman/test_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import pathlib
 import subprocess
 
 from molecule import logger
 from molecule.test.conftest import change_dir_to
 from molecule.util import run_command
-
 from molecule_plugins.podman import __file__ as module_file
 
 LOG = logger.get_logger(__name__)
 
 
 def format_result(result: subprocess.CompletedProcess):
     """Return friendly representation of completed process run."""
@@ -60,33 +59,31 @@
 
 
 def test_dockerfile():
     """Verify that our embedded dockerfile can be build."""
     result = subprocess.run(
         ["ansible-playbook", "--version"],
         check=False,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
         stdin=subprocess.DEVNULL,
         shell=False,
-        universal_newlines=True,
+        text=True,
     )
     assert result.returncode == 0, result
     assert "ansible-playbook" in result.stdout
 
     module_path = os.path.dirname(module_file)
     assert os.path.isdir(module_path)
     env = os.environ.copy()
     env["ANSIBLE_FORCE_COLOR"] = "0"
     result = subprocess.run(
         ["ansible-playbook", "-i", "localhost,", "playbooks/validate-dockerfile.yml"],
         check=False,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
         stdin=subprocess.DEVNULL,
         shell=False,
         cwd=module_path,
-        universal_newlines=True,
+        text=True,
         env=env,
     )
     assert result.returncode == 0, format_result(result)
     # , result
```

### Comparing `molecule-plugins-23.0.0/test/vagrant/functional/conftest.py` & `molecule-plugins-23.4.0/test/vagrant/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/vagrant/functional/test_func.py` & `molecule-plugins-23.4.0/test/vagrant/functional/test_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,40 +15,41 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
+import os
 import platform
 import shutil
+
 import pytest
-import os
-import vagrant
 
-from molecule import util
-from molecule import logger
+import vagrant
+from molecule import logger, util
 from molecule.scenario import ephemeral_directory
-from molecule.util import run_command
 from molecule.test.conftest import change_dir_to
+from molecule.util import run_command
 
 LOG = logger.get_logger(__name__)
 
 
 def is_vagrant_supported() -> bool:
     """Return True if vagrant is installed and current platform is supported."""
     if not shutil.which("vagrant"):
         return False
     if platform.machine() == "arm64" and platform.system() == "Darwin":
         return False
     return True
 
 
 @pytest.mark.skipif(
-    not is_vagrant_supported(), reason="vagrant not supported on this machine"
+    not is_vagrant_supported(),
+    reason="vagrant not supported on this machine",
 )
 def test_command_init_scenario(temp_dir):
     with change_dir_to(temp_dir):
         os.makedirs(os.path.join(temp_dir, "molecule", "default"))
         scenario_directory = os.path.join(temp_dir, "molecule", "test-scenario")
         cmd = [
             "molecule",
@@ -63,84 +64,91 @@
 
         assert os.path.isdir(scenario_directory)
         confpath = os.path.join(scenario_directory, "molecule.yml")
         conf = util.safe_load_file(confpath)
         env = os.environ
         if "TESTBOX" in env:
             conf["platforms"][0]["box"] = env["TESTBOX"]
-        if "vagrant-libvirt" in list(
-            map(lambda x: x.name, vagrant.Vagrant().plugin_list())
-        ):
+        if "vagrant-libvirt" in [x.name for x in vagrant.Vagrant().plugin_list()]:
             conf["driver"]["provider"] = {"name": "libvirt"}
         util.write_file(confpath, util.safe_dump(conf))
 
         cmd = ["molecule", "--debug", "test", "-s", "test-scenario"]
         result = run_command(cmd)
         assert result.returncode == 0
 
 
 @pytest.mark.skipif(
-    not is_vagrant_supported(), reason="vagrant not supported on this machine"
+    not is_vagrant_supported(),
+    reason="vagrant not supported on this machine",
 )
 def test_invalid_settings(temp_dir):
-
     scenario_directory = os.path.join(
-        os.path.dirname(util.abs_path(__file__)), os.path.pardir, "scenarios"
+        os.path.dirname(util.abs_path(__file__)),
+        os.path.pardir,
+        "scenarios",
     )
 
     with change_dir_to(scenario_directory):
         cmd = ["molecule", "create", "--scenario-name", "invalid"]
         result = run_command(cmd)
         assert result.returncode == 2
 
         assert "Failed to validate generated Vagrantfile" in result.stdout
 
 
 @pytest.mark.skipif(
-    not is_vagrant_supported(), reason="vagrant not supported on this machine"
+    not is_vagrant_supported(),
+    reason="vagrant not supported on this machine",
 )
 @pytest.mark.parametrize(
     "scenario",
     [
         ("vagrant_root"),
         ("config_options"),
         ("provider_config_options"),
         ("default"),
         ("default-compat"),
         ("network"),
         ("hostname"),
     ],
 )
 def test_vagrant_root(temp_dir, scenario):
-
     scenario_directory = os.path.join(
-        os.path.dirname(util.abs_path(__file__)), os.path.pardir, "scenarios"
+        os.path.dirname(util.abs_path(__file__)),
+        os.path.pardir,
+        "scenarios",
     )
 
     with change_dir_to(scenario_directory):
         cmd = ["molecule", "test", "--scenario-name", scenario]
         result = run_command(cmd)
         assert result.returncode == 0
 
 
 @pytest.mark.skipif(
-    not is_vagrant_supported(), reason="vagrant not supported on this machine"
+    not is_vagrant_supported(),
+    reason="vagrant not supported on this machine",
 )
 def test_multi_node(temp_dir):
-
     scenario_directory = os.path.join(
-        os.path.dirname(util.abs_path(__file__)), os.path.pardir, "scenarios"
+        os.path.dirname(util.abs_path(__file__)),
+        os.path.pardir,
+        "scenarios",
     )
 
     with change_dir_to(scenario_directory):
         cmd = ["molecule", "test", "--scenario-name", "multi-node"]
         result = run_command(cmd)
         assert result.returncode == 0
 
     molecule_eph_directory = ephemeral_directory()
     vagrantfile = os.path.join(
-        molecule_eph_directory, "scenarios", "multi-node", "Vagrantfile"
+        molecule_eph_directory,
+        "scenarios",
+        "multi-node",
+        "Vagrantfile",
     )
     with open(vagrantfile) as f:
         content = f.read()
         assert "instance-1" in content
         assert "instance-2" in content
```

### Comparing `molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/create.yml` & `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/create.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 - name: Create
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   tasks:
-    - name: Create molecule instance(s)  # noqa fqcn[action]
+    - name: Create molecule instance(s) # noqa fqcn[action]
       vagrant:
         instance_name: "{{ item.name }}"
         instance_interfaces: "{{ item.interfaces | default(omit) }}"
         instance_raw_config_args: "{{ item.instance_raw_config_args | default(omit) }}"
 
         config_options: "{{ item.config_options | default(omit) }}"
 
@@ -35,30 +35,31 @@
 
     # NOTE(retr0h): Vagrant/VBox sucks and parallelizing instance creation
     # causes issues.
 
     # Mandatory configuration for Molecule to function.
 
     - name: Create molecule instances configuration
-      when: server is changed  # noqa no-handler
+      when: server is changed # noqa no-handler
       block:
-
         - name: Populate instance config dict
           ansible.builtin.set_fact:
-            instance_conf_dict: {
-              'instance': "{{ item.Host }}",
-              'address': "{{ item.HostName }}",
-              'user': "{{ item.User }}",
-              'port': "{{ item.Port }}",
-              'identity_file': "{{ item.IdentityFile }}", }
+            instance_conf_dict:
+              {
+                "instance": "{{ item.Host }}",
+                "address": "{{ item.HostName }}",
+                "user": "{{ item.User }}",
+                "port": "{{ item.Port }}",
+                "identity_file": "{{ item.IdentityFile }}",
+              }
           with_items: "{{ server.results }}"
           register: instance_config_dict
 
         - name: Convert instance config dict to a list
           ansible.builtin.set_fact:
             instance_conf: "{{ instance_config_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
         - name: Dump instance config
           ansible.builtin.copy:
             content: "{{ instance_conf | to_json | from_json | to_yaml }}"
             dest: "{{ molecule_instance_config }}"
-            mode: 0600
+            mode: "0600"
```

### Comparing `molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml` & `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 - name: Destroy
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   tasks:
-    - name: Destroy molecule instance(s)  # noqa fqcn[action]
+    - name: Destroy molecule instance(s) # noqa fqcn[action]
       vagrant:
         instance_name: "{{ item.name }}"
         platform_box: "{{ item.box | default(omit) }}"
         provider_name: "{{ molecule_yml.driver.provider.name | default(omit, true) }}"
         provider_options: "{{ item.provider_options | default(omit) }}"
         provider_raw_config_args: "{{ item.provider_raw_config_args | default(omit) }}"
         force_stop: "{{ item.force_stop | default(true) }}"
@@ -26,15 +26,15 @@
 
     # Mandatory configuration for Molecule to function.
 
     - name: Populate instance config
       ansible.builtin.set_fact:
         instance_conf: {}
 
-    - name: Dump instance config  # noqa no-handler
+    - name: Dump instance config # noqa no-handler
       ansible.builtin.copy:
         content: |
           # Molecule managed
           {{ instance_conf | to_json | from_json | to_yaml }}
         dest: "{{ molecule_instance_config }}"
-        mode: 0600
+        mode: "0600"
       when: server.changed | bool
```

### Comparing `molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/hostname/verify.yml` & `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/verify.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml` & `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml` & `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/tools/create_testbox.sh` & `molecule-plugins-23.4.0/tools/create_testbox.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/tools/test-setup.sh` & `molecule-plugins-23.4.0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.0.0/tox.ini` & `molecule-plugins-23.4.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     gce
     podman
     test
     vagrant
 deps =
     py-{devel}: git+https://github.com/ansible-community/molecule.git@main#egg=molecule[test]
 commands =
+    ansible-galaxy install -r requirements.yml
     pytest --collect-only
     pytest --color=yes {tty:-s}
 setenv =
     ANSIBLE_FORCE_COLOR={env:ANSIBLE_FORCE_COLOR:1}
     ANSIBLE_INVENTORY={toxinidir}/tests/hosts.ini
     ANSIBLE_CONFIG={toxinidir}/ansible.cfg
     ANSIBLE_NOCOWS=1
```

