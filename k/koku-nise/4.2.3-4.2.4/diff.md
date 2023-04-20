# Comparing `tmp/koku-nise-4.2.3.tar.gz` & `tmp/koku-nise-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.2.3.tar", last modified: Tue Apr 18 16:58:50 2023, max compression
+gzip compressed data, was "koku-nise-4.2.4.tar", last modified: Thu Apr 20 18:41:41 2023, max compression
```

## Comparing `koku-nise-4.2.3.tar` & `koku-nise-4.2.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.509495 koku-nise-4.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-18 16:58:28.000000 koku-nise-4.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 16:58:28.000000 koku-nise-4.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 16:58:50.509495 koku-nise-4.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-04-18 16:58:28.000000 koku-nise-4.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.497495 koku-nise-4.2.3/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 16:58:50.000000 koku-nise-4.2.3/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.501495 koku-nise-4.2.3/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/ocp-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.505495 koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:58:50.509495 koku-nise-4.2.3/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-18 16:58:28.000000 koku-nise-4.2.3/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:58:50.509495 koku-nise-4.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 16:58:28.000000 koku-nise-4.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-20 18:41:18.000000 koku-nise-4.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 18:41:18.000000 koku-nise-4.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 18:41:41.721258 koku-nise-4.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-20 18:41:18.000000 koku-nise-4.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.713257 koku-nise-4.2.4/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39500 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/ocp-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:41:41.721258 koku-nise-4.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-20 18:41:18.000000 koku-nise-4.2.4/setup.py
```

### Comparing `koku-nise-4.2.3/LICENSE` & `koku-nise-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/README.rst` & `koku-nise-4.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,120 +1,109 @@
-===========
-Nise README
-===========
-|license| |PyPI| |Build Status| |Unittests| |codecov| |Updates|
-
------
-About
------
+# Nise
+
+[![license](https://img.shields.io/github/license/project-koku/nise.svg)](https://github.com/project-koku/nise/blob/main/LICENSE)
+[![PyPI](https://badge.fury.io/py/koku-nise.svg)](https://badge.fury.io/py/koku-nise)
+[![Build
+Status](https://github.com/project-koku/nise/workflows/Publish/badge.svg?branch=main)](https://github.com/project-koku/nise/actions)
+[![Unittests](https://github.com/project-koku/nise/workflows/Unit%20Tests/badge.svg)](https://github.com/project-koku/nise/actions)
+[![codecov](https://codecov.io/gh/project-koku/nise/branch/main/graph/badge.svg)](https://codecov.io/gh/project-koku/nise)
+
+## About
 
 A tool for generating sample cost and usage data for testing purposes.
 
-To submit an issue please visit https://issues.redhat.com/projects/COST/
+To submit an issue please visit https://issues.redhat.com/projects/COST/.
 
----------------
-Getting Started
----------------
+## Getting Started
 
 This is a Python project developed using Python 3.8. Make sure you have at least this version installed.
 
-Development
-===========
+### Development
 
-To get started developing against Nise first clone a local copy of the git repository. ::
+To get started developing against Nise first clone a local copy of the git repository.
 
     git clone https://github.com/project-koku/nise
 
-Developing inside a virtual environment is recommended. A Pipfile is provided. Pipenv is recommended for combining virtual environment (virtualenv) and dependency management (pip). To install pipenv, use pip ::
+Developing inside a virtual environment is recommended. A Pipfile is provided. Pipenv is recommended for combining virtual environment (virtualenv) and dependency management (pip). To install pipenv, use pip
 
     pip3 install pipenv
 
-Then project dependencies and a virtual environment can be created using ::
+Then project dependencies and a virtual environment can be created using
 
     pipenv install --dev
 
-To activate the virtual environment run ::
+To activate the virtual environment run
 
     pipenv shell
 
-To build the command line tool run ::
+To build the command line tool run
 
     python setup.py install
 
-For generating sample data for developing or testing Koku, please refer to `Ingesting Nise data with Koku <https://github.com/project-koku/nise/blob/main/docs/working_with_masu.rst>`_.
+For generating sample data for developing or testing Koku, please refer to [Ingesting Nise data with Koku](docs/working_with_masu.md).
 
-Testing
--------
+#### Testing
 
-Nise uses tox to standardize the environment used when running tests. Essentially, tox manages its own virtual environment and a copy of required dependencies to run tests. To ensure a clean tox environment run ::
+Nise uses tox to standardize the environment used when running tests. Essentially, tox manages its own virtual environment and a copy of required dependencies to run tests. To ensure a clean tox environment run
 
     tox -r
 
 This will rebuild the tox virtual env and then run all tests.
 
 To run sanity tests
 
     tox -e sanity
 
-To run all unit tests specifically::
+To run all unit tests specifically:
 
     make test
 
-To run unit tests for a single provider::
+To run unit tests for a single provider:
 
     make test test_source=<aws|azure|gcp|ocp|oci>
 
-Linting
--------
-This repository uses `pre-commit`_ to check and enforce code style. It uses `Black`_ to reformat the Python code and `Flake8`_ to check it
-afterwards. Other formats and text files are linted as well.
 
-To run pre-commit checks::
+#### Linting
+
+This repository uses [pre-commit](https://pre-commit.com) to check and enforce code style. It uses [Black](https://github.com/psf/black) to reformat the Python code and [Flake8](http://flake8.pycqa.org) to check it afterwards. Other formats and text files are linted as well.
+
+To run pre-commit checks:
 
     pre-commit run --all-files
 
 
-Publishing
-----------
+#### Publishing
 
-Please remember to sync your updated dependecies to setup.py with ::
+Please remember to sync your updated dependecies to setup.py with :
 
     pipenv-setup sync -p
 
 After that, make sure to increment the version in setup.py. As soon as your PR is merged to main, a new koku-nise package will built, tagged, and deployed to PyPI.
 
-Finer Publishing Details
-________________________
+##### Finer Publishing Details
 
-All of the deployment is driven entirely by a Github Action workflow, so if issues ever crop up, start in ``publish-to-pypi.yml``. When a branch is merged into main, the Action will kick off. There are three things that must happen before a deployment is successful, a successful artifact build, dependencies verified in sync between the requirements files, and setup.py, and the tag must not yet exist in git. The dependency syncing/verification is done with the `pipenv-setup <https://github.com/Madoshakalaka/pipenv-setup>`_ tool. After the artifact is deployed, it'll be available at `PyPI <https://pypi.org/project/koku-nise/#history>`_.
+All of the deployment is driven entirely by a Github Action workflow, so if issues ever crop up, start in `publish-to-pypi.yml`. When a branch is merged into main, the Action will kick off. There are three things that must happen before a deployment is successful, a successful artifact build, dependencies verified in sync between the requirements files, and setup.py, and the tag must not yet exist in git. The dependency syncing/verification is done with the [pipenv-setup](https://github.com/Madoshakalaka/pipenv-setup) tool. After the artifact is deployed, it\'ll be available at [PyPI](https://pypi.org/project/koku-nise/#history).
 
+#### Nise, Koku, and IQE Integration
 
-
-Nise, Koku, and IQE Integration
--------------------------------
-
-The iqe tests use nise to generate mock data; therefore, we need to ensure that our nise changes do not break the iqe tests. To do this you will need to copy the `.env.example` to a `.env` file.
-After the `.env` file is configured you will then need to run ::
+The iqe tests use nise to generate mock data; therefore, we need to ensure that our nise changes do not break the iqe tests. To do this you will need to copy `.env.example` to `.env` and customize as necessary. After the `.env` file is configured you will then need to run
 
     make run-iqe
 
-The `make run-iqe` command by default will run the smoke tests. However, if you want to run a specific iqe test command you can pass it in through the `IQE_CMD` parameter ::
+The `make run-iqe` command by default will run the smoke tests. However, if you want to run a specific iqe test command you can pass it in through the `IQE_CMD` parameter
 
     make run-iqe IQE_CMD='iqe tests plugin hccm -k test_api_aws_provider_create_foo_resource_name'
 
-
-Prereqs
-=======
+### Prereqs
 
 - AWS population requires prior setup of AWS Cost and Usage Report of same name to be created, as well as associated Bucket, Policy, Role, etc.
 
------
-Usage
------
-nise is a command line tool::
+## Usage
+
+`nise` is a command line tool.
 
     Usage:
         nise ( report | yaml )
         nise report ( aws | azure | gcp | ocp | oci ) [options]
         nise yaml ( aws | azure | ocp | ocp-on-cloud | oci ) [options]
 
     Report Options:
@@ -176,57 +165,46 @@
                                                 only; default is 1)
 
     OCP-on-Cloud Options:
         -c, --config ( CONFIG | default )       REQUIRED, Config file path. If "default" is provided,
                                                 use internal config file
         -n, --num-nodes INT                     optional, Number of nodes to generate (default is 1)
 
-Notes
-=====
-1. If ``--aws-s3-report-name`` or ``--aws-s3-report-prefix`` are specified they should match what is configured in the AWS cost usage report settings.
-
-2. For ``--aws-finalize``:
-
-   - ``copy`` will create a local copy of the data with a ``-finalized`` suffix and invoice id populated.
-   - ``overwrite`` will generate a regular report with the invoice id populated.
-
-3. If ``--insights-upload`` is specified and pointing to a URL endpoint, you must have ``INSIGHTS_USER`` and ``INSIGHTS_PASSWORD`` set in your environment. Payloads for insights uploads will be split on a per-file basis.
-
-4. If ``--static-report-file`` is used start_date will default to first day of current month.  ``start_date: last_month`` will be first day of previous month.  ``start_date: today`` will start at the first hour of current day.  ``end_date`` can support relative days from the ``start_date``. i.e ``end_date: 2`` is two days after start date.
-
-5. ``--static-report-file`` usage dates has a special ``full_period`` key value which will specify a usage for the entire ``start_date - end_date`` range.
-
-6. ``--ros-ocp-info`` when we generate ros data along with this parameter then we will be getting ros-ocp metrix too.
-
---------
-Examples
---------
 
-`Example cost and usage report generation.`_
+### Notes
 
-`Example yaml generation.`_
+1.  If `--aws-s3-report-name` or `--aws-s3-report-prefix` are specified
+    they should match what is configured in the AWS cost usage report
+    settings.
+1.  For `--aws-finalize`:
+    -   `copy` will create a local copy of the data with a `-finalized`
+        suffix and invoice id populated.
+    -   `overwrite` will generate a regular report with the invoice id
+        populated.
+1.  If `--insights-upload` is specified and pointing to a URL endpoint,
+    you must have `INSIGHTS_USER` and `INSIGHTS_PASSWORD` set in your
+    environment. Payloads for insights uploads will be split on a
+    per-file basis.
+1.  If `--static-report-file` is used start_date will default to first
+    day of current month. `start_date: last_month` will be first day of
+    previous month. `start_date: today` will start at the first hour of
+    current day. `end_date` can support relative days from the
+    `start_date`. i.e `end_date: 2` is two days after start date.
+1.  `--static-report-file` usage dates has a special `full_period` key
+    value which will specify a usage for the entire
+    `start_date - end_date` range.
+1.  `--ros-ocp-info` when we generate ros data along with this parameter
+    then we will be getting ros-ocp metrix too.
+
+
+## Examples
+
+[Example cost and usage report
+generation.](docs/cost_usage_report_generation.md)
 
-------------
-Contributing
-------------
+[Example YAML generation.](docs/yaml_generation.md)
 
-Please refer to Contributing_.
 
-.. _Contributing: https://github.com/project-koku/nise/blob/main/CONTRIBUTING.rst
-.. _pre-commit: https://pre-commit.com
-.. _Black: https://github.com/psf/black
-.. _Flake8: http://flake8.pycqa.org
-.. _Example cost and usage report generation.: docs/cost_usage_report_generation.rst
-.. _Example yaml generation.: docs/yaml_generation.rst
+## Contributing
 
-.. |license| image:: https://img.shields.io/github/license/project-koku/nise.svg
-   :target: https://github.com/project-koku/nise/blob/main/LICENSE
-.. |Build Status| image:: https://github.com/project-koku/nise/workflows/Publish/badge.svg?branch=main
-   :target: https://github.com/project-koku/nise/actions
-.. |Unittests| image:: https://github.com/project-koku/nise/workflows/Unit%20Tests/badge.svg
-   :target: https://github.com/project-koku/nise/actions
-.. |codecov| image:: https://codecov.io/gh/project-koku/nise/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/project-koku/nise
-.. |Updates| image:: https://pyup.io/repos/github/project-koku/nise/shield.svg?t=1524249231720
-   :target: https://pyup.io/repos/github/project-koku/nise/
-.. |PyPI| image:: https://badge.fury.io/py/koku-nise.svg
-   :target: https://badge.fury.io/py/koku-nise
+Please refer to
+[Contributing](CONTRIBUTING.md).
```

### Comparing `koku-nise-4.2.3/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.2.4/koku_nise.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.py
 koku_nise.egg-info/PKG-INFO
 koku_nise.egg-info/SOURCES.txt
 koku_nise.egg-info/dependency_links.txt
 koku_nise.egg-info/entry_points.txt
 koku_nise.egg-info/not-zip-safe
 koku_nise.egg-info/requires.txt
```

### Comparing `koku-nise-4.2.3/nise/__main__.py` & `koku-nise-4.2.4/nise/__main__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/aws-template-manifest.json` & `koku-nise-4.2.4/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/copy.py` & `koku-nise-4.2.4/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/extract.py` & `koku-nise-4.2.4/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/__init__.py` & `koku-nise-4.2.4/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/aws_constants.py` & `koku-nise-4.2.4/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/aws_generator.py` & `koku-nise-4.2.4/nise/generators/aws/aws_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.2.4/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/ebs_generator.py` & `koku-nise-4.2.4/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/ec2_generator.py` & `koku-nise-4.2.4/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.2.4/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/rds_generator.py` & `koku-nise-4.2.4/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/route53_generator.py` & `koku-nise-4.2.4/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/s3_generator.py` & `koku-nise-4.2.4/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/aws/vpc_generator.py` & `koku-nise-4.2.4/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/__init__.py` & `koku-nise-4.2.4/nise/generators/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/azure_generator.py` & `koku-nise-4.2.4/nise/generators/azure/azure_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.2.4/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.2.4/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.2.4/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/storage_generator.py` & `koku-nise-4.2.4/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.2.4/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.2.4/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/__init__.py` & `koku-nise-4.2.4/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/gcp/project_generator.py` & `koku-nise-4.2.4/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/generator.py` & `koku-nise-4.2.4/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/__init__.py` & `koku-nise-4.2.4/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.2.4/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.2.4/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/oci_constants.py` & `koku-nise-4.2.4/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.2.4/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/oci_generator.py` & `koku-nise-4.2.4/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.2.4/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/ocp/__init__.py` & `koku-nise-4.2.4/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.2.4/nise/generators/ocp/ocp_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,32 +133,50 @@
     OCP_STORAGE_USAGE: OCP_STORAGE_COLUMNS,
     OCP_NODE_LABEL: OCP_NODE_LABEL_COLUMNS,
     OCP_NAMESPACE_LABEL: OCP_NAMESPACE_LABEL_COLUMNS,
     OCP_ROS_USAGE: OCP_ROS_USAGE_COLUMN,
 }
 
 OCP_OWNER_WORKLOAD_CHOICES = (
-    ("<none>", "<none>", None, None),  # manually created Pod
+    # ("<none>", "<none>", None, None),  # manually created Pod - recommendation won't be generated
     (None, "ReplicaSet", None, "deployment"),
     (None, "ReplicaSet", "<none>", "deployment"),  # manually created ReplicaSet
     (None, "ReplicationController", "<none>", "deploymentconfig"),  # manually created ReplicationController
     (None, "ReplicationController", None, "deploymentconfig"),
     (None, "StatefulSet", None, "statefulset"),
     (None, "DaemonSet", None, "daemonset"),
-    (None, "Job", None, "job"),
+    # (None, "Job", None, "job"), # not supported by Kruize
 )
 
 
 def get_owner_workload(pod):
     on, ok, wl, wt = choice(OCP_OWNER_WORKLOAD_CHOICES)
-    if on == "<none>" or wl == "<none>":
+    if on == "<none>" and wl == "<none>":  # manually created Pod
         return on, ok, wl, wt
+    elif wl == "<none>":  # manually created ReplicaSet or ReplicationController
+        return pod, ok, wl, wt
     return pod, ok, pod, wt
 
 
+def generate_randomized_ros_usage(usage_dict, limit_value):
+    # if usage value is provided in yaml -> avg_value = +- 5% of that specified usage value
+    if usage_value := usage_dict.get("full_period"):
+        avg_value = min(round(uniform(usage_value * 0.95, usage_value * 1.05), 5), limit_value)
+    # if usage value is not specified in yaml -> random avg_usage from 10% to 100% of the limit
+    else:
+        avg_value = round(uniform(limit_value * 0.1, limit_value), 5)
+
+    # min value - random float derived from avg_value,
+    min_value = round(uniform(avg_value * 0.8, avg_value), 5)
+    # max_value - random float derived from avg_value, but max of limit_value
+    max_value = min(round(uniform(avg_value, avg_value * 1.2), 5), limit_value)
+
+    return avg_value, min_value, max_value
+
+
 class OCPGenerator(AbstractGenerator):
     """Defines a abstract class for generators."""
 
     def __init__(self, start_date, end_date, attributes, ros_ocp_info=False):
         """Initialize the generator."""
         self._nodes = None
         self.ros_ocp_info = ros_ocp_info
@@ -365,48 +383,56 @@
                         "mem_limit_gig": mem_limit_gig,
                         "pod_labels": specified_pod.get("labels", None),
                         "cpu_usage": cpu_usage,
                         "mem_usage_gig": memory_usage_gig,
                         "pod_seconds": specified_pod.get("pod_seconds"),
                     }
                     owner_name, owner_kind, workload, workload_type = get_owner_workload(pod)
+
+                    cpu_usage_avg, cpu_usage_min, cpu_usage_max = generate_randomized_ros_usage(cpu_usage, cpu_limit)
+                    memory_usage_gig_avg, memory_usage_gig_min, memory_usage_gig_max = generate_randomized_ros_usage(
+                        memory_usage_gig, mem_limit_gig
+                    )
+                    memory_rss_ratio = 1 / round(uniform(1.01, 1.9), 2)
+                    cpu_throttle = choices([0, round(cpu_usage_avg / randint(10, 20), 5)], weights=(3, 1))[0]
+
                     ros_ocp_data_pods[pod] = {
                         "namespace": namespace,
                         "node": node.get("name"),
                         "resource_id": node.get("resource_id"),
                         "pod": pod,
                         "container_name": pod,
                         "owner_name": owner_name,
                         "owner_kind": owner_kind,
                         "workload": workload,
                         "workload_type": workload_type,
                         "image_name": self.fake.word() + "-" + self.fake.word(),
-                        "cpu_request_container_avg": randint(75, 100),
-                        "cpu_request_container_sum": randint(25, 75),
-                        "cpu_limit_container_avg": randint(25, 75),
-                        "cpu_limit_container_sum": randint(25, 75),
-                        "cpu_usage_container_avg": randint(25, 75),
-                        "cpu_usage_container_min": randint(0, 25),
-                        "cpu_usage_container_max": randint(75, 100),
-                        "cpu_usage_container_sum": randint(25, 75),
-                        "cpu_throttle_container_avg": randint(25, 75),
-                        "cpu_throttle_container_max": randint(75, 100),
-                        "cpu_throttle_container_sum": randint(25, 75),
-                        "memory_request_container_avg": randint(25, 75),
-                        "memory_request_container_sum": randint(25, 75),
-                        "memory_limit_container_avg": randint(25, 75),
-                        "memory_limit_container_sum": randint(25, 75),
-                        "memory_usage_container_avg": randint(25, 75),
-                        "memory_usage_container_min": randint(0, 25),
-                        "memory_usage_container_max": randint(75, 100),
-                        "memory_usage_container_sum": randint(25, 75),
-                        "memory_rss_usage_container_avg": randint(25, 75),
-                        "memory_rss_usage_container_min": randint(0, 25),
-                        "memory_rss_usage_container_max": randint(75, 100),
-                        "memory_rss_usage_container_sum": randint(25, 75),
+                        "cpu_request_container_avg": cpu_request,
+                        "cpu_request_container_sum": cpu_request,
+                        "cpu_limit_container_avg": cpu_limit,
+                        "cpu_limit_container_sum": cpu_limit,
+                        "cpu_usage_container_avg": cpu_usage_avg,
+                        "cpu_usage_container_min": cpu_usage_min,
+                        "cpu_usage_container_max": cpu_usage_max,
+                        "cpu_usage_container_sum": cpu_usage_avg,
+                        "cpu_throttle_container_avg": cpu_throttle,
+                        "cpu_throttle_container_max": cpu_throttle,
+                        "cpu_throttle_container_sum": cpu_throttle,
+                        "memory_request_container_avg": round(mem_request_gig * GIGABYTE),
+                        "memory_request_container_sum": round(mem_request_gig * GIGABYTE),
+                        "memory_limit_container_avg": round(mem_limit_gig * GIGABYTE),
+                        "memory_limit_container_sum": round(mem_limit_gig * GIGABYTE),
+                        "memory_usage_container_avg": round(memory_usage_gig_avg * GIGABYTE),
+                        "memory_usage_container_min": round(memory_usage_gig_min * GIGABYTE),
+                        "memory_usage_container_max": round(memory_usage_gig_max * GIGABYTE),
+                        "memory_usage_container_sum": round(memory_usage_gig_avg * GIGABYTE),
+                        "memory_rss_usage_container_avg": round(memory_usage_gig_avg * memory_rss_ratio * GIGABYTE),
+                        "memory_rss_usage_container_min": round(memory_usage_gig_min * memory_rss_ratio * GIGABYTE),
+                        "memory_rss_usage_container_max": round(memory_usage_gig_max * memory_rss_ratio * GIGABYTE),
+                        "memory_rss_usage_container_sum": round(memory_usage_gig_avg * memory_rss_ratio * GIGABYTE),
                     }
 
             else:
                 num_pods = randint(2, 20)
                 for _ in range(num_pods):
                     pod_suffix = "".join(choices(ascii_lowercase, k=5))
                     pod_type = choice(("build", "deploy", pod_suffix))
@@ -415,14 +441,15 @@
                     cpu_cores = node.get("cpu_cores")
                     cpu_limit = round(uniform(0.02, cpu_cores), 5)
                     cpu_request = round(uniform(0.02, cpu_limit), 5)
                     memory_bytes = node.get("memory_bytes")
                     memory_gig = memory_bytes / GIGABYTE
                     mem_limit_gig = round(uniform(25.0, memory_gig), 2)
                     mem_request_gig = round(uniform(25.0, mem_limit_gig), 2)
+
                     pods[pod] = {
                         "namespace": namespace,
                         "node": node.get("name"),
                         "resource_id": node.get("resource_id"),
                         "pod": pod,
                         "node_capacity_cpu_cores": cpu_cores,
                         "node_capacity_cpu_core_seconds": cpu_cores * HOUR,
@@ -431,48 +458,55 @@
                         "cpu_request": cpu_request,
                         "cpu_limit": cpu_limit,
                         "mem_request_gig": mem_request_gig,
                         "mem_limit_gig": mem_limit_gig,
                         "pod_labels": self._gen_openshift_labels(),
                     }
                     owner_name, owner_kind, workload, workload_type = get_owner_workload(pod)
+                    cpu_usage_avg, cpu_usage_min, cpu_usage_max = generate_randomized_ros_usage({}, cpu_limit)
+                    memory_usage_gig_avg, memory_usage_gig_min, memory_usage_gig_max = generate_randomized_ros_usage(
+                        {}, mem_limit_gig
+                    )
+                    memory_rss_ratio = 1 / round(uniform(1.01, 1.9), 2)
+                    cpu_throttle = choices([0, round(cpu_usage_avg / randint(10, 20), 5)], weights=(3, 1))[0]
+
                     ros_ocp_data_pods[pod] = {
                         "namespace": namespace,
                         "node": node.get("name"),
                         "resource_id": node.get("resource_id"),
                         "pod": pod,
                         "container_name": pod,
                         "owner_name": owner_name,
                         "owner_kind": owner_kind,
                         "workload": workload,
                         "workload_type": workload_type,
                         "image_name": self.fake.word() + "-" + self.fake.word(),
-                        "cpu_request_container_avg": randint(75, 100),
-                        "cpu_request_container_sum": randint(25, 75),
-                        "cpu_limit_container_avg": randint(25, 75),
-                        "cpu_limit_container_sum": randint(25, 75),
-                        "cpu_usage_container_avg": randint(25, 75),
-                        "cpu_usage_container_min": randint(0, 25),
-                        "cpu_usage_container_max": randint(75, 100),
-                        "cpu_usage_container_sum": randint(25, 75),
-                        "cpu_throttle_container_avg": randint(25, 75),
-                        "cpu_throttle_container_max": randint(75, 100),
-                        "cpu_throttle_container_sum": randint(25, 75),
-                        "memory_request_container_avg": randint(25, 75),
-                        "memory_request_container_sum": randint(25, 75),
-                        "memory_limit_container_avg": randint(25, 75),
-                        "memory_limit_container_sum": randint(25, 75),
-                        "memory_usage_container_avg": randint(25, 75),
-                        "memory_usage_container_min": randint(0, 25),
-                        "memory_usage_container_max": randint(75, 100),
-                        "memory_usage_container_sum": randint(25, 75),
-                        "memory_rss_usage_container_avg": randint(25, 75),
-                        "memory_rss_usage_container_min": randint(0, 25),
-                        "memory_rss_usage_container_max": randint(75, 100),
-                        "memory_rss_usage_container_sum": randint(25, 75),
+                        "cpu_request_container_avg": cpu_request,
+                        "cpu_request_container_sum": cpu_request,
+                        "cpu_limit_container_avg": cpu_limit,
+                        "cpu_limit_container_sum": cpu_limit,
+                        "cpu_usage_container_avg": cpu_usage_avg,
+                        "cpu_usage_container_min": cpu_usage_min,
+                        "cpu_usage_container_max": cpu_usage_max,
+                        "cpu_usage_container_sum": cpu_usage_avg,
+                        "cpu_throttle_container_avg": cpu_throttle,
+                        "cpu_throttle_container_max": cpu_throttle,
+                        "cpu_throttle_container_sum": cpu_throttle,
+                        "memory_request_container_avg": round(mem_request_gig * GIGABYTE),
+                        "memory_request_container_sum": round(mem_request_gig * GIGABYTE),
+                        "memory_limit_container_avg": round(mem_limit_gig * GIGABYTE),
+                        "memory_limit_container_sum": round(mem_limit_gig * GIGABYTE),
+                        "memory_usage_container_avg": round(memory_usage_gig_avg * GIGABYTE),
+                        "memory_usage_container_min": round(memory_usage_gig_min * GIGABYTE),
+                        "memory_usage_container_max": round(memory_usage_gig_max * GIGABYTE),
+                        "memory_usage_container_sum": round(memory_usage_gig_avg * GIGABYTE),
+                        "memory_rss_usage_container_avg": round(memory_usage_gig_avg * memory_rss_ratio * GIGABYTE),
+                        "memory_rss_usage_container_min": round(memory_usage_gig_min * memory_rss_ratio * GIGABYTE),
+                        "memory_rss_usage_container_max": round(memory_usage_gig_max * memory_rss_ratio * GIGABYTE),
+                        "memory_rss_usage_container_sum": round(memory_usage_gig_avg * memory_rss_ratio * GIGABYTE),
                     }
 
         return pods, namespace2pod, ros_ocp_data_pods
 
     def _gen_volumes(self, namespaces, namespace2pods):  # noqa: R0914,C901
         """Create volumes on specific namespaces and keep relationship."""
         volumes = []
@@ -603,22 +637,23 @@
         pod_seconds = user_pod_seconds if user_pod_seconds else randint(2, HOUR)
         pod = kwargs.get("pod")
         cpu_limit = pod.pop("cpu_limit")
         mem_limit_gig = pod.pop("mem_limit_gig")
 
         cpu_request = min(pod.pop("cpu_request"), cpu_limit)
         mem_request_gig = min(pod.pop("mem_request_gig"), mem_limit_gig)
-
         cpu_usage = self._get_usage_for_date(kwargs.get("cpu_usage"), start)
         cpu = round(uniform(0.02, cpu_limit), 5)
+        # ensure that cpu usage is not higher than cpu_limit
         if cpu_usage:
             cpu = min(cpu_limit, cpu_usage)
 
         mem_usage_gig = self._get_usage_for_date(kwargs.get("mem_usage_gig"), start)
         mem = round(uniform(1, mem_limit_gig), 2)
+        # ensure that mem usage is not higher than mem_limit
         if mem_usage_gig:
             mem = min(mem_limit_gig, mem_usage_gig)
 
         pod["pod_usage_cpu_core_seconds"] = pod_seconds * cpu
         pod["pod_request_cpu_core_seconds"] = pod_seconds * cpu_request
         pod["pod_limit_cpu_core_seconds"] = pod_seconds * cpu_limit
         pod["pod_usage_memory_byte_seconds"] = pod_seconds * mem * GIGABYTE
```

### Comparing `koku-nise-4.2.3/nise/manifest.py` & `koku-nise-4.2.4/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/report.py` & `koku-nise-4.2.4/nise/report.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/upload.py` & `koku-nise-4.2.4/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/util/__init__.py` & `koku-nise-4.2.4/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/util/log.py` & `koku-nise-4.2.4/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_gen.py` & `koku-nise-4.2.4/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.2.4/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/aws/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.2.4/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/aws/regions.py` & `koku-nise-4.2.4/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/azure/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/oci/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.2.4/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.2.4/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.2.4/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.2.4/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.2.4/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.2.4/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.2.4/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.2.4/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.2.4/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.2.4/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/nise/yaml_generators/utils.py` & `koku-nise-4.2.4/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.3/setup.py` & `koku-nise-4.2.4/setup.py`

 * *Files identical despite different names*

